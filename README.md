# FiiO-playlist-generator

This is a tool to generate playlist files, enabling you to play music of a single interpret at random on FiiO X1 II or similar media players. This particular player can only play songs of a single folder at random. It can't play at random with subfolders.

Instructions
-
Copy all files to microSD card root.

Make sure the folder structure on microSD card is similar to this:

```
\
\Audio\
\Audio\() Streamripper
\Audio\() Streamripper\Electro Swing Revolution Radio
\Audio\Boney M\
\Audio\Boney M\Greatest Hits\
\Audio\Boney M\Greatest Hits\CD1
\Audio\Boney M\Greatest Hits\CD2
\Audio\Boney M\Greatest Hits\CD3
\Audio\Lindsey Stirling\
...
```

When executed with PHP, a new folder Playlists will show up in root. Do not insert anything to this folder manually as all playlists will be deleted when you run the generator again to refresh contents.

After running, two playlists will show up in Playlists folder:
```
Boney M.m3u
Lindsey Stirling.m3u
```

Contents of folder `() Streamripper` will be ignored. I have successfully tested this script even with diacritics and they seem to work fine on FiiO X1 II.

To set up PHPX files to be executed by PHP, follow this short guide: https://ashus.ashus.net/thread-134-post-845.html

Why is this needed
-
I record several internet radio stations and sometimes the cut between song-to-song is not precise - gapless playback and playing in order is needed.
To use these playlists, simply choose them in the player and turn shuffle on.
