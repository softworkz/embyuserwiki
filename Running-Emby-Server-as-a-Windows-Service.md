**IMPORTANT**: This guide applies to new server installations of version 3.2.31 or greater. If you are running an older installation that embeds a Windows Service, please continue using that.

To start, please [install Emby Server from the Emby website](https://emby.media/download.html).

To setup a Windows Service, we'll be using a program called [NSSM](http://nssm.cc/) that can turn any app into a Windows Service. To begin:

* Download [NSSM](http://nssm.cc/).
* Copy nssm.exe to C:\Windows\system32
* Open command prompt as admin and type "nssm install" to open the NSSM user interface.

Follow [this guide](http://nssm.cc/usage) to create your Windows Service, but incorporate the following changes:

* **Application path**: path to mediabrowser.serverapplication.exe
* **Startup directory**: folder containing mediabrowser.serverapplication.exe
* **Arguments**: -service
* **Service name**: Emby Server (or other name of your choice)

Then, on the exit actions tab, make sure to configure the exit action to **not** automatically restart:

![](images/server/nssm1.jpg)

This is important because without this, using the **Shutdown** button inside Emby Server will cause NSSM to automatically restart Emby Server.