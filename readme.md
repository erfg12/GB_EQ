# About GB EQ
A fun project to re-create EverQuest elements in a new GameBoy game. Built specifically with [GB Studio 2.0.0 Beta 4](https://www.gbstudio.dev/). I personally have NO artistic talent, so drawing sprites is a huge problem. I mostly convert the models into images, then to the GameBoy's color palette. Same with the music and sound. They are very restricted to the instruments and sounds allowed on the plateform. I used MuseScore with the [EverQuest Midi Project](https://sites.google.com/site/everquestmidiproject/everquest-midi-files) along with other software. Instructions are below for all of the steps I used to create the assets.

## Using PhotoShop to Convert Images to GB Color Palette
1) Open the image in Photoshop. Click Image > Mode > Index > Load Swatch > `gb-studio-photoshop no-transparent.aco` (It's the GB Studio colors without the transparent color).
2) You can now import the image to your scene, by switching Mode to RGB.
NOTE: Try not to reduce the image size once the swatch is applied as it may merge and change the colors. Apply size changes prior to the swatch color index.

## How To Get EQ Zone Models
Download [EQZoneViewer](http://eqclassic.de/wiki/EverQuest_Zone_Viewer) and uncheck models you want to hide and click the top left button to hide terrain.

## How To Get EQ Character Models
Some models are viewable at http://eqtools.eqemu.io

## Using MuseScore to Make Sound & Music
Download [MuseScore](https://musescore.org) and [OpenMPT](https://openmpt.org/).
1) Click Format > Styles, Uncheck Hide Instrument if 1 instrument is present. Double click on the instrument.
2) Change instrument to Electronic > Sci-Fi Synthesizer.
3) Change instrument pitch range to C1-C3. Export as midi.
4) Open OpenMTP software, open Setup, change MIDI File Import Pattern Size to 64.
5) Click the `File > Append MIDI` menu option and select the `project/assets/music/template.mod` file. Delete all channels except for 1-4 via General > change from 99 to 4 channels and remove everything after channel 4. Delete all content from channel 4 as this will cause screeches and beeps in the song. Save the .mod file to `project/assets/music`. If it doesn't automatically appear in GBStudio, close and re-open it.
