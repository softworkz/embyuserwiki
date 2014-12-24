There are two ways to identify a video as 3D.

## Using the web interface

## Video filenames flags

In order to properly detect 3D, two tags need to be present in the filename. First, a '3D' tag has to be present. Second, one of the following must also be present, hsbs, fsbs, sbs, htab, ftab.

Tags need be be surrounded be either a space ( ), hyphen -, dot . or underscore _. Tags are case-insensitive, so both 3d and 3D will work.

## Brackets

Older file naming conventions are still accepted  by placing one of the following tags within the filename:

* [fsbs] - Indicates full side by side
* [ftab] - Indicates full top and bottom
* [hsbs] - Indicates half side by side
* [htab] - Indicates half top and bottom
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