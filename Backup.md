This guide will go over how to migrate your settings from Emby Server from one machine to another.

## Use the Emby Backup Plugin

We recommend using the Emby Backup plugin, which is designed to make this process really painless by doing the work for you. Emby Backup requires Emby Premiere and can be found in our plugin catalog.

To backup and restore using the Emby Backup plugin, simply do the following:
* Install the plugin into your existing Emby Server
* Configure the Backup plugin by setting a folder to save the backups within.
By default, this process will run every 12 hours and will retain at most 3 backups. You can monitor your folder to see that backups are created.
* Install the plugin on your new Emby Server installation, then configure to backup folder to the same folder that contains your backups.
* Click on a backup, you'll then be taken to the restore screen where you can run a restore.
You're done !

If you prefer to backup manually, read on....

## How to Backup Manually

The following instructions will detail how to manually backup or migrate an Emby Server installation.