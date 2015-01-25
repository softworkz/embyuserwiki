Hosting settings allow you to configure Media Browser's built-in web server. These settings are accessed by opening the server dashboard and navigating to **Advanced** -> **Hosting**.

For the purposes of this document we are defining local as within your home network, and external as outside your network away from home.

## Http Port

The http port settings allow you to specify both the local, system port that the server should bind to, as well as the external port that the server should use when reporting it's external url to clients.

![](images/server/hosting1.png)

Generally these two values will be the same, but they can be customized as needed.

## External WAN Address

The server will attempt to automatically detect your external address. The result is displayed on the front page of the server dashboard.

If for some reason you need to customize this value, or it is not detected properly, you can manually enter your external address here:

![](images/server/hosting2.png)

Most users can leave this blank and rely on the server's automatic detection. If you are using a DDNS, or the Https feature with a self-signed certificate, then you may prefer to customize it.

## Https Port

## Automatic Port Mapping