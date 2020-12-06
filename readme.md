Built with GB Studio 2.0.0 Beta 4

## How To Convert Music to .mod
1) Run software through either audacity and change the pitches to C1-C3 or GSXCC with Famicom music set in Config. Convert the audio file to MIDI via any web app.
2) Open OpenMTP software, open Setup, change MIDI File Import Pattern Size to 64.
3) Click the `File > Append MIDI` menu option and select the `project/assets/music/template.mod` file. Delete all channels except for 1-4 via General > change from 99 to 4 channels and remove everything after channel 4. Delete all content from channel 4 as this will cause screeches and beeps in the song. Save the .mod file to `project/assets/music`. If it doesn't automatically appear in GBStudio, close and re-open it.

## How To Convert Images to GB Colors
1) Open the image in Photoshop. Click Image > Mode > Index > Load Swatch > `gb-studio-photoshop no-transparent.aco` (It's the GB Studio colors without the transparent color).
2) You can now import the image to your scene, by switching Mode to RGB.
NOTE: Try not to reduce the image size once the swatch is applied as it may merge and change the colors. Apply size changes prior to the swatch color index.