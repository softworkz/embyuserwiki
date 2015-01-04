For a simple TV folder structure, the recommended folder layout is Series\Season\Episode or Series\Episode. When setting up the library make sure to select **TV** as the content type.

For example:

```
 \TV
    \Glee
       \Season 1
          Glee S01E01.mp4
          Glee S01E02.mp4

 \TV
    \Seinfeld
       Seinfeld S01E01.mp4
       Seinfeld S01E02.mp4

```

## Complex Folder Structure

In more complex situations where your top-level directory is further sub-divided before the show folders, there are two different approaches to setting up in Media Browser. The recommended option is to create a TV media folder and add the sub-folder locations instead of the top level folder. Alternatively, you can add the top-level as the main folder but leave the content type unset, and then set the content type to TV on each sub-folder.

For example:

```
 \TV
     \A-M
       \Glee
          \Season 1
             Glee S01E01.mp4
     \N-Z
       \Seinfeld
          \Season 1
             Seinfeld S01E01.mp4

```

In the above example, the recommended setup is to create a TV media folder, and then add the **A-M** and **N-Z** library paths. Or the "TV" folder can be left to content type **unset**, and both the A-M and N-Z folders would be set to a content type of **TV**.

For more information on setting up the library, see [Library Setup](Library Setup).

### Dvd and Blu-ray episodes

Dvd and Blu-ray folder structures are also supported. The folders can have any name, but using episode numbers will improve the ability to download and display metadata. 

To be recognized as a dvd structure, the folder must contain either a VIDEO_TS subfolder, or a VIDEO_TS.ifo file. To be recognized as a blu-ray structure, the folder must contain a BDMV subfolder.

```
 \TV
    \Glee
       \Season 1
          \Glee S01E01-E04
              \VIDEO_TS
          \Glee S01E05-E08
              VIDEO_TS.IFO
          \Glee S01E09-E10
              \BDMV

```

## Episode naming conventions

A number of naming conventions are supported:

* anything_s01e02.ext
* anything_s1e2.ext
* anything_s01.e02.ext
* anything_s01_e02.ext
* anything_1x02.ext
* anything_102.ext
* anything_1x02.ext
* 02 Episode Name.avi
* s01e02.avi
* 1x02.avi

### By date

Common for long-running daily shows, you can also use the date the episode aired.

* anything_1996.11.14.ext
* anything_1996-11-14.ext
* anything_14.11.1996.ext

## Multi-episode files

The following conventions are supported:

* 01x02x03 episode name.avi
* S01x02x03 episode name.avi
* S01E02E03 episode name.avi
* S01xE02xE03 episode name.avi
* S01E02-E03 episode name.avi
* S01E02-X03 episode name.avi
* 01x02 01x03 episode name.avi
* 01x02 - 01x03 episode name.avi
* 01x02 - x03 episode name.avi
* S01x02.S01x03 episode name.avi
* S01x02 - S01x03 episode name.avi
* show name 01x02x03 episode name.avi
* show name S01x02x03 episode name.avi
* show name S01E02E03 episode name.avi
* show name S01xE02xE03 episode name.avi
* show name S01E02-E03 episode name.avi
* show name S01E02-X03 episode name.avi
* show name 01x02 01x03 episode name.avi
* show name 01x02 - 01x03 episode name.avi
* show name 01x02 - x03 episode name.avi
* show name S01x02.S01x03 episode name.avi
* show name S01x02 - S01x03 episode name.avi

## Specials

Specials should be named using 0 as the season number. For example:

```
 \TV
    \Glee
       \Season 0
          Glee S00E01.mp4

```

## Series & Season Images

Images are supported in both series and season folders. Below is a table of the supported image file names. Supported image extensions are **jpg**, **jpeg**, **png** and **tbn**.

Several image types support multiple file names. They are listed in the order that they're checked for.

| Image Type | Supported file names  |
| ------------- |---------------|
| Primary      | folder.ext |
|              | poster.ext |
|              | cover.ext |
|              | default.ext |
|              | show.ext (series folder only) |
| Art      | clearart.ext      |
| Backdrop  | backdrop.ext, backdropX.ext |
|           | fanart.ext, fanart-X.ext |
|           | background.ext, background-X.ext      |
|           | art.ext, art-X.ext      |
|           | extrafanart (subfolder)/fanartX.ext      |
| Banner   | banner.ext      |
| Disc     | disc.ext      |
|          | cdart.ext      |
| Logo     | logo.ext      |
| Thumb     | thumb.ext      |
|           | landscape.ext      |

For backdrops, X represents a number, and you can have any amount of numbered backdrops. For example:

```
 \TV
    \Glee
       backdrop.ext
       backdrop1.ext
       backdrop2.ext
       backdrop3.ext

```

## Season images without season folder

If season folders are not used, season images can still be supplied directly in the series folder, using a naming convention to indicate the season.

| Image Type | Supported file names  |
| ------------- |---------------|
| Primary      | seasonXX-poster.ext |
|              | season-specials-poster.ext |
| Backdrop     | seasonXX-fanart.ext |
|              | season-specials-fanart.ext |
| Banner       | seasonXX-banner.ext |
|              | season-specials-banner.ext |
| Thumb        | seasonXX-landscape.ext |
|              | season-specials-landscape.ext |

For example:

```
 \TV
    \Glee
       season01-poster.jpg
       season-specials-poster.jpg
       season01-fanart.jpg
       season-specials-fanart.jpg
       season01-banner.jpg
       season-specials-banner.jpg
       season01-landscape.jpg
       season-specials-landscape.jpg

```

## Episode Images

The following naming conventions are supported for episode images:

* {name}-thumb.ext (in same folder)
* {name}.ext (in metadata sub-folder)

Supported image extensions are **jpg**, **jpeg**, **png** and **tbn**.

For example:

```
 \TV
    \Glee
       \Season 1
          Glee S01E01.mp4
          Glee S01E01-thumb.jpg
       \Season 2
          Glee S02E01.mp4
          /metadata
              Glee S02E01.jpg

```

## 3D episodes

3D episodes files are supported. See [3D videos](3D Videos).

## Media stubs

Media stubs are supported as episodes. See [media stubs](Media stubs).

## Strm files

Strm files are supported as episodes. See [strm files](Strm files).

## Subtitles

Subtitles for episode files are supported. See [subtitles](Subtitles).