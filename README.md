# Blender-Camera-to-Replay-Camera
The script I use to convert selected blender cameras into replay mod's timeline

## BEFORE USING

**I recommended having Toggle Path Preview off**
It will lag otherwise.

**Make backups of important replay recordings**
Not responsible for corrupted files.

## How to use the script
If you haven't used scripts in Blender, copy and paste the text into the Text Editor and click the Run Script.

First, have the camera you want to import selected.

Second, run the script and select the replay recording file you want to change. Files are normally located here: AppData\Roaming.minecraft\replay_recordings

Third, click Modify .mcpr

## What the options do

Density: Controls the percentage of keyframes transferred. At very low values you might be able to toggle path preview on.

Scale Time: Stretches the Blender timeline to Replay Mod’s timeline. A value of 1 means 1:1, 2 means 1:2, and so on. Very low values (<0.01) may cause keyframes to overlap, preventing the replay from loading.

Scene Start is Replay Start: Automatically aligns the start of your scene with the replay's start. Disable this if you want your first keyframe to appear later.

Enables Catmull Interpolation: By default it uses linear but it might be useful to use smoothing with low density values.


## Quick video showing it https://youtu.be/2QIWRUhhq4I

All camera constraints should automatically be baked correctly but if you are doing something very weird and it doesnt work lmk.

## How do you know what position in Blender corresponds to Minecraft?
The easiest way to do this is by importing part of the map with Mineways. However, **unselect**  this option when exporting.
You can also try exporting a test camera path from Replay Mod but it might be more tedious 

![alt text]([http://url/to/img.png](https://media.discordapp.net/attachments/513734977146585091/1276301694157717556/Capture.PNG?ex=66fa7854&is=66f926d4&hm=b8b629b3c2d0dfba7f077c491e0219294f23b3e3a1ae6f4d7061a1ad8b2a9520&=&format=webp&quality=lossless&width=1089&height=418))
