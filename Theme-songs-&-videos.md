###Theme Songs
 
Any folder (movie, series, season, game, etc) can have theme songs. Emby apps will play the songs in the background while browsing through the content.

There are two supported conventions, theme.ext, or the 'theme-music' sub-folder, where ext is any valid audio extension.

```
/Movies
   /Home Alone (1990)
      homealone.mp4
      theme.mp3
```

or

```
/Movies
   /Home Alone (1990)
      homealone.mp4
      /theme-music
          song1.mp3
          song2.wma
          song3.flac
```
 
###Theme Videos

Any folder (movie, series, season, game, etc) can have theme videos using a 'backdrops' sub-folder. Some Emby apps will play the videos in the background while browsing through the content.

```
/Movies
   /Home Alone (1990)
      homealone.mp4
      /backdrops
          video1.mkv
          video1.mp4
```