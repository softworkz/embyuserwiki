###Installation:

We recommend you install directly from the [Docker Hub](hub.docker.com) by issuing the following command from within a terminal:
```
docker run -it --rm -v /usr/local/bin:/target \
    emby/emby-server:testing install_emby
```

Optionally, you can also install a systemd service file to control Emby server using systemctl.
Before installing the systemd service file, you should specify which user you wish the deamon to run as. You can do this by reinstalling emby with the following command:
```
docker run -it --rm -v /usr/local/bin:/target -e "EMBYSERVER_USER=username" \
    emby/emby-server:testing install_emby
```
Above, change username to the name of the user you with to run the daemon as. Afterward, proceed with the service file installation:
```
docker run -it --rm -v /etc/systemd/system:/target \
   emby/emby-server:testing install_service
```
If you installed the systemd service file, you can enable Emby server to automatically start when the system boots by executing the following command:
```
sudo systemctl enable emby-server.service
```

###Setting up Emby:

Once Emby has been installed you can simply execute the binary from a terminal:
```
emby-server
```

The first time you run the Emby server docker it will prompt you for the locations of your media files. Enter one location per line. This will ensure that the container gets access to the host's file system from within the containerized environment.

###Updating:
If you have installed our systemd service file, you can simply update by executing the following command:
```
systemctl restart emby-server.service
```
Additionally you can update by:
```
docker exec emby-server update
```

Or by:
```
docker pull emby/emby-server:testing
docker stop emby-server
emby-server
```

### Technical information:
Our new image and installation process setups Emby server to run with the permissions of the user executing `emby-server`. So, Emby's data is set to save within the user's home directory under the name `.emby-server`. 

You may overwrite the default settings by passing the appropriate environment variable:
* EMBYSERVER_USER - user name of the user to run emby as. 
* EMBYSERVER_CONFIG - the directory which Emby should use to save metadata and configuration.

Please read Docker documentation on [environment variables](https://docs.docker.com/engine/reference/run/#env-environment-variables) for more information.

Manual setup:
Of course you can always run docker image manually. Please be aware that if you wish your data to remain persistent you need to provide a location for the `/config` volume. For example,
```
docker run -d -v /home/user/embydata:/config emby/emby-server:testing
``` 
All the information from above regarding user UID and GID still applies when executing a docker run command.
 
###Migrating your data from an existing installation:
Before proceeding please ensure you have made a backup of your emby data (i.e. ```tar cvf embydata.tar /var/lib/emby-server```). Additionally, please verify that you are mounting your emby data as described above. 

In the following example we will demonstrate how to migrate your database using the default setting that emby is deployed with. By default on Linux distributions Emby Server keeps it's data in ```/var/lib/emby-server```, while the Docker container keeps it's data in ```/config```. That being said one could migrate their database as follows:

```
docker exec -ti emby-server bash
s6-svc -d /run/s6/services/emby-server
migrate_db /config/data/library.db /var/lib/emby-server /config
s6-svc -u /run/s6/services/emby-server
exit
```