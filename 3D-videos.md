There are two ways to identify a video as 3D.

## Using the web interface

## Video filenames flags

In order to properly detect 3D, two tags need to be present in the filename. First, a '3D' tag has to be present that matches the following regex: [-. _]3d[-. _]

In addition to this, either a 'SBS' tag [-. _]h?sbs[-. _] or a 'TAB' flag [-. _]h?tab[-. _] must be present in the filename.

Regex matching is done case-insensitive, so for example either .3d. and .3D. will work.

Note: the tags need be be surrounded be either a space ( ), hyphen -, dot . or underscore _.

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