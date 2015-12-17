###Installation:

We recommend you install directly from the [Docker Hub](hub.docker.com) by issuing the following command from within a terminal:
```
docker run -it --rm -v /usr/local/bin:/target \
    emby/emby-server:testing install_emby
```

Optionally, you can also install a systemd service file if you wish to control Emby server from systemd.
```
docker run -it --rm -v /etc/systemd/system:/target \
   emby/emby-server:testing install_service
```
When installing the service it is important you ensure that you installed emby-server specifying the user you wish emby to run as. For example,
```
docker run -it --rm -v /usr/local/bin:/target -e "EMBYSERVER_USER=username" \
    emby/emby-server:testing install_emby
```
It perfectly fine to reissue to install command.

If you installed our systemd service file, you can enable Emby server to automatically start when the system boots by executing the following command:
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
 