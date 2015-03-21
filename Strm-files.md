Various internet video and audio streams can be played back in Emby as if they were locally stored on your media center by using STRM files. As long as the format and streaming-method (network-protocol) is supported by Emby, stream can be added. These are basic text files that look like <name>.strm and contain a URL to the internet stream
 
### Usage

Create a normal text-file and rename the .txt extension to .strm then open it up with a text-editor (like Notepad in Microsoft Windows) and input the the direct URL-link of the stream.

This should look like:

```
http://host/path/stream
```

or 

```
mms://host/path/stream
```

or 

```
rtsp://host/path/stream
```


## Examples

A strm file as a movie:

```
\Movies
   \300
      300.strm
```

Strm files can be used for any kind of video, such as movies, episodes, music videos, home videos, etc.

The naming convention of the .strm file name should follow the convention used for the associated content type (movies, episodes, etc).