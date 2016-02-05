This file naming guide applies to movies, home videos and music videos. For tv episode naming, see [TV naming](TV naming).

### Library Setup

When setting up the library, make sure to select **Movies**, **Home videos**, or **Music videos** as the content type.

For **movies**, it is recommended to have only the **title** and **year**, followed by the extension. To improve matching add the year within parenthesis to the end of the file or folder name (before the extension, if file name). This naming standard will generally yield the best results.

Examples:

```
\Movies\Pulp Fiction (1994).avi
\Movies\Reservoir Dogs (1992).avi
\Movies\The Usual Suspects (1995).avi
\Movies\Avatar (2009)-cd1.mkv
\Movies\Avatar (2009)-cd2.mkv
\Movies\Avatar (2009)\somefilename.mkv
\Movies\The Usual Suspects (1995)\somefilename.avi
\Movies\The Usual Suspects (1995)\somefilename-cd1.avi
\Movies\The Usual Suspects (1995)\somefilename-cd2.avi
\Movies\Avatar (2009)\Avatar (2009)-cd1.mkv
\Movies\Avatar (2009)\Avatar (2009)-cd2.mkv
```

### Dvd and Blu-ray

Dvd and Blu-ray folder structures are also supported. To be recognized as a dvd structure, the folder must contain either a VIDEO_TS subfolder, or a VIDEO_TS.ifo file. To be recognized as a blu-ray structure, the folder must contain a BDMV subfolder.

```
\Movies\Alien (1979)\VIDEO_TS.IFO
\Movies\Léon (1994)\VIDEO_TS.IFO
\Movies\Scarface (1983)\VIDEO_TS.IFO

Or:

 \Movies\Alien (1979)\VIDEO_TS\VIDEO_TS.IFO
 \Movies\Léon (1994)\VIDEO_TS\VIDEO_TS.IFO
 \Movies\Scarface (1983)\VIDEO_TS\VIDEO_TS.IFO
```

## Split video files (file stacking)

The following are default stacking extensions that can be added to file names. # can be 1 through 9 or A through D. Stacking is supported for video files as well as dvd and blu-ray folder structures.

* ​part#​
* ​cd#​
* ​dvd#​
* ​pt#​
* ​disk#​
* ​disc#​

You can also use:
* moviename#.ext

Where # can be A through D.

Examples:

```
\Movies\Avatar (2009)\Avatar (2009)-cd1.mkv
\Movies\Avatar (2009)\Avatar (2009)-cd2.mkv
\Movies\Scarface (1983)\Disc 1\VIDEO_TS\VIDEO_TS.IFO
\Movies\Scarface (1983)\Disc 2\VIDEO_TS\VIDEO_TS.IFO
```

## Multi-version movies
 
Multiple versions of the same content can be stored in a single movie folder.

```
/Movies
  /300
    /300 - 1080p.mkv
    /300 - 720p.mkv
```

Each version must begin with the folder name, followed by " - ". If this requirement is not met, they will be treated as separate videos. 

Alternatively they can be grouped together manually using the server's web interface.  

## Movie extras

Special features for movies can be stored in an extras folder under movie folders. Nested folders are not supported.
 
```
/Movies
   /Home Alone (1990)
      Home Alone (1990).mkv
      /extras
         deleted-scenes.mkv 
```

## Video images

Images are supported in video folders. Below is a table of the supported image file names. Supported image extensions are **jpg**, **jpeg**, **png** and **tbn**.

Several image types support multiple file names. They are listed in the order that they're checked for.

| Image Type | Supported file names  |
| ------------- |---------------|
| Primary      | {name}.ext |
|              | {name}-poster.ext |
|              | {name}-cover.ext |
|              | {name}-default.ext |
|              | {name}-movie.ext |
|              | folder.ext |
|              | poster.ext |
|              | cover.ext |
|              | default.ext |
|              | movie.ext |
| Art      | {name}-clearart.ext      |
|          | clearart.ext      |
| Backdrop  | backdrop.ext, backdropX.ext |
|           | fanart.ext, fanart-X.ext |
|           | background.ext, background-X.ext      |
|           | art.ext, art-X.ext      |
|           | extrafanart (subfolder)/fanartX.ext      |
| Banner   | {name}-banner.ext      |
|          | banner.ext      |
| Disc     | {name}-disc.ext      |
|          | {name}-cdart.ext      |
|          | disc.ext      |
|          | cdart.ext      |
| Logo     | {name}-logo.ext      |
|          | logo.ext      |
| Thumb     | {name}-thumb.ext      |
|           | {name}-landscape.ext      |
|           | thumb.ext      |
|           | landscape.ext      |

{name} represents the video file name, without extension. For videos that are not contained within their own folder, only the conventions using {name} are supported.

For backdrops, X represents a number, and you can have any amount of numbered backdrops. For example:

```
 \Movies
    \300
       backdrop.ext
       backdrop1.ext
       backdrop2.ext
       backdrop3.ext

```

## 3D videos

3D video files are supported. See [3D videos](3D Videos).

## Media stubs

Media stubs are supported. See [media stubs](Media stubs).

## Strm files

Strm files are supported. See [strm files](Strm files).

## Subtitles

Subtitles are supported. See [subtitles](Subtitles).

## Theme songs & videos

Theme songs & videos are supported. See [theme songs & videos](Theme songs & videos).

## Trailers

Trailers are supported. See [trailers](Trailers).