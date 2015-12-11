### Linux Troubleshooting Guide and FAQ:

#### Emby Server does not restart from the web interface:
Emby on Linux does not have the built in capability to restart itself. Thus, for Emby to restart a helper script is used. The helper script named ```restart.sh``` can be found on most distributions at ```/usr/lib/emby-server```. The script can only restart Emby, if it was started by a service manager program such as systemctl, service, or invoke-rc.d. If for some reason the helper script does not successfully restart Emby for you, please check the following:
* Ensure helper script is executable.
* Ensure Emby was started via a service manager.