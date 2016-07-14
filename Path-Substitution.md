By allowing Emby apps direct access to media folders on the server, they may be able to play them directly over the network and avoid using server resources to stream and transcode. Path substitution can help achieve this by mapping a path on the server to a network path that can be accessed by other devices.

Path substitutions are configured in the **Path Substitution** tab of the library setup area.

### Example:

You have a Movies library on the server as **D:\Movies**. This folder is also shared on the network as **\\\\Server\Movies**. You'd like to allow an Emby app on another machine direct access to the shared folder.

To do this, create a path substitution with the following values:

**From**: D:\Movies

**To**: \\\\Server\Movies

This will allow some Emby apps to access the media directly and avoid having to stream or transcode using Emby Server.