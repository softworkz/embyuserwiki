The recommended folder structure for TV is Series\Season\Episode or Series\Episode.

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