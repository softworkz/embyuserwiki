Emby for iPhone and iPad is available in the [Apple App Store](https://itunes.apple.com/us/app/emby/id992180193?ls=1&mt=8).

Emby for iPhone and iPad can handle just about any type of media thanks to [Emby Server transcoding](Transcoding). If you would like to learn how to prepare your media for Direct Play, read below.

# Setup Guide

Install the app using one of the above methods, then use the startup wizard to connect to your Emby Server.

# Direct Play Media Formats

* Video — H.264/AVC/HEVC (.MP4, .MOV, .M4V)
* Subtitles - SRT and other text-based formats
* Audio – aac,mp3,mpa,wav,wma,mp2,ogg,oga,webma,ape,opus,flac

In many cases, even when direct play is not possible, a simple audio-only conversion can be performed without having to convert the video. 

# Best Practices for Direct Play

* Ensure your media meets the above criteria.

* Leave the app's streaming bitrate setting on the default value of Auto, if possible. The app will perform bandwidth tests with your Emby Server to determine the maximum playable bitrate.

* If you are customizing the bitrate setting, then you will need to compare the bitrate of your files to the bitrate setting in the app. You can find the bitrate of a file by checking the media info in the web interface. If the bitrate of a file is higher than the setting in the app, transcoding will be required. Increasing the bitrate setting in the app can help reduce transcoding, but may impact playback performance if your network connection is not fast enough to handle it.

![](images/apps/webbitrate.png)

# Chromecast

The app supports casting to Chromecast devices. To connect to your Chromecast device, simply click the cast icon in the top right corner of the app. You'll then be asked which device you'd like to connect to.

Once connected, any content you play will be sent to the Chromecast device. You're able to play individual files, entire folders, shuffle, instant mix, queue, and more.

For more information, see [Chromecast](Chromecast).