The Live TV feature allows you to stream live television and manage your DVR within Emby Apps. Live TV is setup in two steps:

* Configure your TV Tuner
* Add a TV Guide Data Source

## Configure Your TV Tuner

Out of the box, Emby Server currently supports the following TV Tuners:

* [HDHomerun Network Tuner](HDHomerun)
* Hauppauge TV Tuners (on Emby Server for Windows)
* [M3U files (or urls)](M3U%20Tuners). See examples of m3u files at http://xmtvplayer.com/build-m3u-file

Support for additional tuners can be added by installing a [Live TV Plugin](Live-TV-Plugins).

In most cases, Emby Server will automatically discover your HDHomerun on your network with no configuration required. If this does not happen for you, adding a tuner manually is very simple.  Simply open the server dashboard, navigate to **Live TV**, then click **Add** underneath tuner devices.

## Add a TV Guide Data Source

Out of the box, Emby Server currently supports the following TV Guide data sources:

* [Schedules Direct](Schedules%20Direct)
* [Xml TV](Xml%20Tv)

Support for additional sources can be added by installing a [Live TV Plugin](Live-TV-Plugins).

## Live TV Status

The status of your tv tuners is also displayed in the server dashboard by navigating to **Live TV**.

![](images/server/livetv3.png)

In addition, the reset button next to each tuner will allow you to reset the tuner as needed for troubleshooting.

There is also the ability to manually refresh Guide data. This is normally run automatically and it is generally not needed for manual use, but it is provided here as a convenience.

![](images/server/livetv2.png)

## Settings

The **Settings** tab allows you to configure how many days of guide data to download and display. More guide data provides a richer experience but may increase loading times.

![](images/server/livetv4.png)