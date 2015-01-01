One of the areas in which MediaBrowser shines as a media server is the metadata management. The server has a metadata manager which allows you to view all of the metadata for every item in your library in one place.

The metadata manager can be accessed via the slideout in the web client in the top left hand corner of the screen.

![](images/server/metadatamanager1.png)

Another way to access the metadata manager is via **Options**->**Edit** of the item you would like to edit. This method will take you directly to the item in the editor.

![](images/server/metadatamanager2.png)

##Using the Metadata Manager

Once you are in the metadata manager, you can edit whatever fields you would like. Be sure to select **Save**; otherwise, all of your changes will be lost. If you wish for the changes that you made to be persistent through a refresh of the item, you will need to either lock the metadata field you changed, or lock the entire item.

![](images/server/metadatamanager3.png)

![](images/server/metadatamanager4.png)

All media can get their information from online databases such as TheMovieDB and TheTVDB. If an item is misidentified by the server, you can manually identify the item using the **Identify** button, or, if you already know the database IDs for your incorrectly identified item, simply insert the correct IDs into the database fields and refresh the item.

The advanced refresh option can be used to force images to be redownloaded in addition to the text metadata.

##Tags and Parental Controls

One trick that you can use to prevent a user from accessing certain content is to use the **Tags** metadata field.

![](images/server/metadatamanager7.png)

To keep a user profile from accessing certain content

- Tag each item that you want to prevent access to with a unique tag.
- Go to the **Users**->**Parental Control** in the server dashboard.
- Add the unique tag to the **Block content with these tags** field.
- Save the changes to the user profile and media tags.

To make sure the tags don't disappear in a library refresh, lock the **Tags** field in the item's metadata.

![](images/server/metadatamanager6.png)

## Subtitles

For your movies and TV shows, the metadata manager is the place to manage subtitles . You can see which subtitles you have, whether they are graphical or text, and what languages the subtitles are in.

![](images/server/metadatamanager8.png)

To enable access to the OpenSubtitles database, you will need to enter your account information in **Metadata**->**Subtitles** in the dashboard. This area is also the place to manage what will be automatically downloaded when the **Download missing subtitles** task in **Advanced**->**Scheduled tasks** is run.

## Images

MediaBrowser can automatically download images to improve the presentation of media in each client. To enable automatic image downloading, you will need to have the **Download artwork and metadata from the internet** option checked in **Metadata**->**Basics** in the dashboard.

![](images/server/metadatamanager5.png)

Images are downloaded from Fanart.tv, TheMovieDB, The Open Movie Database, and TheTVDB. The images tab in the metadata manager can be used to modify what images the server presents for your MediaBrowser clients.

To change the image used, simply click on the cloud underneath each image and the server will search all of the databases for new images.

![](images/server/metadatamanager9.png)