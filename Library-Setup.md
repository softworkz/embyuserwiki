Setting up the library is handled within the startup wizard and also within the server dashboard, located by clicking on the **Library** tab.

### Prepare Your Media

It's important to first prepare your media. See other sections of the wiki for more information:

* [Movie naming](Movie naming)
* [TV naming](TV naming)
* [Music naming](Music naming)
* [Subtitles](Subtitles)

### Library Setup Page

The configuration will display the media folders you've configured and allow you to add, remove, rename or change the paths they're mapped to. 

> A media folder is a grouping of one or more physical folders on your file system.

The below example screenshot lists four media folders:

![](images/server/librarysetup1.png)

Clicking the "Add Media Folder" button will open a dialog to add a media folder, where you choose the content type and enter a name. 

### Content Type

Choosing the right content type is important. See the above guide on media preparation for best practices for Movie, TV and Music sections. 

Use the unset content type if you'd like to add a media folder that mixes different content. Please note that support for mixed content is limited.

![](images/server/librarysetup2.png)

### Library Paths

Each media folder can have one or more physical library paths. In the below example screenshot, the Movies folder contains two physical paths:

![](images/server/librarysetup3.png)

To add a library path, click the + button. A popup will be displayed allowing you to browse to the location in a visual manner.

>**Important**: If you are going to use one of the HTPC apps (Classic, Theater, or Kodi) it is very important to use the Path Substitution feature to translate the server's local paths to network ones or define your media locations with network UNC paths that those machines can see.

**Note**: On some networks the visual browser may fail to display network devices. If this occurs you can still complete the dialog by typing in the path manually and clicking OK.

![](images/server/librarysetup4.png)

## Path Substitution

Path substitutions are used for mapping a path on the server to a path that clients are able to access. By allowing clients direct access to media on the server they may be able to play them directly over the network and avoid using server resources to stream and transcode them.

Path substitutions are configured in the **Path Substitution** tab of the library setup area.