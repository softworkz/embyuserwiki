The server has several settings that can be used to customize how it presents itself to users.

The **Friendly server name** can be used to set a custom name for the Media Browser Connect. If no friendly name is set, the hostname of the computer will be used instead.

The **Preferred display language** is used to set the language for the server. Currently, many translations are works in progress. If you wish to contribute, please refer to the forums for more information.

## Advanced settings

The **Local port number** refers to the port to which Media Browser will bind itself when it starts. If you change this setting, you will need to restart the server for changes to take effect, but when they do, you will then need to navigate to ```http://server-ip:local-port-number/mediabrowser``` to access the server's webclient. Do NOT change this setting unless you KNOW what you are doing.

The **Public port number** is the port on the router that Media Browser Connect will tell clients to use when accessing your server via the internet. You must forward this port number in your router to the **Local port number** if you wish to access your server from outside your home network.

**Automatic port mapping** takes advantage of UPnP to automatically forward the necessary ports in your router. One caveat for automatic port mapping to work is that your router will need to have UPnP capability.

**External DDNS** is for those who have a dynamic DNS address. Media Browser Connect will use the value in the external DDNS field to connect to your server so do NOT set this unless you have a properly configured dynamic DNS service on your computer.

**Cache path** is used to set a custom cache path if you do not want the cache to be located in the server default app data directory, e.g. you have the server installed on a small SSD drive and wish to move the cache to a larger hard drive.

## Branding

The **Login disclaimer** can be used to display a custom message on the login screen of the web client.

![](images/server/serversettings1.png)

![](images/server/serversettings2.png)