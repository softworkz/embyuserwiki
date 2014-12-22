The recommended folder structure for music is Artist\Album\Song

```
 \Music
    \Artist Name
       \Album Name
          1- Song.mp3
          2- Song.mp3
```

This is not a requirement and other structures will also work, but this is the most common method.

Any naming convention for audio files is acceptable. Track numbers are retrieved using embedded ID3 tag information. 

## Multi-Disc Albums

Albums can have disc sub-folders using any of the following folder names, where X represents the disc number:
 
- Disc X
- Disk X
- CD X
- Disc-X
- Disk-X
- CD-X
- DiscX
- DiskX
- CDX
- VolX
- Vol-X
- VolumeX
- Volume-X

For example:

```
 \Music
    \Artist Name
       \Album Name
         \Disc 1
            1- Song.mp3
            2- Song.mp3
         \Disc 2
            1- Song.mp3
            2- Song.mp3
```

## Music Images

Images are supported in both artist and album folders, as well as images embedded within audio files. Below is a table of the supported image file names:

Supported image extensions are **jpg**, **jpeg**, **png** and **tbn**.

Several image types support multiple file names. You can choose which ones to use. They are listed in the order that they're checked for.

| Image Type | Supported file names  |
| ------------- |---------------|
| Primary      | {foldername}-poster.ext |
|              | {foldername}-cover.ext |
|              | {foldername}-default.ext |
|              | folder.ext |
|              | cover.ext |
|              | poster.ext |
|              | default.ext |
| Art      | {foldername}-clearart.ext |
|          | clearart.ext      |
| Backdrop      | centered      |
| Banner | banner.ext      |
| Disc | disc.ext      
|      | cdart.ext      
| Logo | logo.ext      |
| Thumb | thumb.ext      |
|       | landscape.ext      |



## Music Videos

To add music videos, setup a library with the type "Music Videos". The naming conventions for music videos are identical to [movies](Movie naming).

To identify the artists and albums of music videos, use the [metadata manager](Metadata manager). Simply edit a music video and enter the artist(s) and/or album. Once complete, the artist and album pages will display links to the music videos.