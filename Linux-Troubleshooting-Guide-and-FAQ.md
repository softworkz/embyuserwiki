#### Emby Server does not restart from the web interface:
Emby on Linux does not have the built-in capability to restart itself. So to restart Emby uses a helper script. The helper script named ```restart.sh``` can be found on most distributions at ```/usr/lib/emby-server```. The script can only restart Emby if it was started by a service manager program such as systemctl, service, or invoke-rc.d. If for some reason the helper script does not successfully restart Emby for you, please check the following:
* Ensure helper script is executable.
* Ensure Emby was started via a service manager.
* Ensure permissions of /etc/sudoers.d/emby are 0640
* Ensure whatever user is running emby-server is part of group emby (usermod -a -G emby $USER_NAME)
* Ensure /etc/sudoers permissions is 0640

### Will you support Intel QSV on Linux:
Intel QSV on Linux is not widely supported. Yes, Intel has made the media sdk opensource, but it is only available for specific distros and kerenls. It would not be fruitful at this time for the Emby development team to dedicate any time on getting QSV working on Linux. Once Intel's media sdk is widely available the decision will be revisited. 

### What distros and kernel version are supported by Intel QSV:
At the time of writing, Intel officially supports QSV on [SLES 12 and Centos 7.1](https://software.intel.com/en-us/intel-mediasdk-supported-versions-server).

### If I want Intel QSV no matter what, what can I do:
Follow the guidelines from [Intel](https://software.intel.com/sites/default/files/media_server_studio_getting_started_guide.pdf) on installing the media sdk on one of the supported platforms. Then follow the [ffmpeg compiling guide](https://github.com/drocon11/ffmpeg-qsv) to enable QSV.

### I can not add media: