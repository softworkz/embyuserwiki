There are mulitple ways to identify a video as 3D.

## Identify using the web interface

A video can be identified as 3D using the the [metadata manager](Metadata manager). Simply edit a video:

![](images/server/musicvideos1.png)

Then select the 3D format:

![](images/server/3dvideos1.png)


## Identify using video file name flags

In order to properly detect 3D, two tags need to be present in the filename. First, a '3D' tag has to be present. Second, one of the following must also be present, hsbs, fsbs, sbs, htab, ftab, or mvc.

Tags need be be surrounded be either a space ( ), hyphen -, dot . or underscore _. Tags are case-insensitive, so both 3d and 3D will work.

Examples:

* moviename (year).3d.hsbs.mkv
* moviename 3d sbs.mkv
* moviename.3D-HTAB.mkv
* moviename-3D.sbs-720p.mkv
* moviename-3D.mvc.mkv

## Identify using older conventions

Older file naming conventions are still accepted  by placing one of the following tags within the filename:

* [fsbs]
* [ftab]
* [hsbs]
* [htab]
* [3d] - Indicates half side by side
* [sbs3d] - Indicates half side by side

For example:

```
/Movies
   /300
     300 [hsbs].mkv
   /Home Alone (1990)
     Home Alone [fsbs].mkv
```