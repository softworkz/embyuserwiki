Cloud sync allows you to copy content to cloud storage accounts, for backup as well as archiving in multiple resolutions.

When content is archived in multiple resolutions, Emby apps will automatically choose the version that is most efficient for them. This will help relieve stress on your internet connection as well as your server's CPU. Apps will browse the content through your Emby Server as normal, but will stream from the cloud during playback.

## Installation

To install folder sync, open the **Emby Server Dashboard** and navigate to **Sync** -> **Services**. 

Click on Google Drive underneath **Available Services**.

![](images/plugins/googledrive1.png)

Then proceed to install it on the installation page.

## Configuration

To configure Google Drive, open the **Emby Server Dashboard** and navigate to **Sync** -> **Services**.  Click on Google Drive underneath **Installed Services**. 

Configuring Google Drive is a two step process. 

### Create a Client Id and Secret

First you'll need to create a client Id and Secret. To do this, click on the link titled "Create a Google Drive Client Id and Secret". Follow the instructions in the popup message.

### Add Google Drive Accounts

After you're configured the Client Id and Secret, you'll need to add one or more Google Drive accounts. To do this, click the + button next to Google Drive Accounts. You'll then be guided through the process of adding a Google Drive account.

## Ready to Sync

Once a Google Drive account has been added, it will then show as as an available destination when creating sync jobs:

![](images/plugins/foldersync3.png) 

## Playback

Once synced, Emby apps will automatically use the additional media sources when possible. For example, suppose you have a high bitrate movie that requires transcoding to Roku. By syncing to the cloud and selecting a conversion profile that is compatible with Roku, the Roku app can then direct play the synced version rather than transcoding the original.