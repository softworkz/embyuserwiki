## Temporary Path

The server will need to create temporary files throughout the transcoding process. The location of these files can be configured.

![](images/server/transcoding2.png)

If you specify a custom path, please ensure the following conditions are met:

* The folder is writable
* The folder is not used for any other purpose, as the server will delete all contents to keep it clean.


## Audio Boost

When surround audio is converted to 2-channel stereo audio, this often results in a lower volume level. To offset this, you can configure an audio boost scale factor to increase the volume.

![](images/server/transcoding3.png)

The default value is **2**, meaning the volume will be doubled when converting surround audio to stereo.


## Debug Logging

Debug logging can be enabled as needed for troubleshooting.

![](images/server/transcoding4.png)

**Note**: Debug logging will significantly increase the size of transcoding log files, and therefore is only recommended as needed to resolve issues.