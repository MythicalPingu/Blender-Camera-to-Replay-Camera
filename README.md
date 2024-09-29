# Blender-Camera-to-Replay-Camera
The script I use to convert selected blender cameras into replay mod's timeline


If you haven't used scripts in Blender, copy and paste the text into the Text Editor and click the Run Script.

First, have the camera you want to import selected.
Second, run the script and select the replay recording file you want to change. Files are normally located here: AppData\Roaming.minecraft\replay_recordings
Third, click Modify .json (it should only modify the timelines.json within this .mcpr)

**I recommended having Toggle Path Preview off**
It will lag otherwise.
**Make backups of important replay recordings**
Not responsible for corrupted files.

What the options do:

Density: Controls the percentage of keyframes transferred. At very low values you might be able to toggle path preview on.

Scale Time: Stretches the Blender timeline to Replay Mod’s timeline. A value of 1 means 1:1, 2 means 1:2, and so on. Very low values (<0.01) may cause keyframes to overlap, preventing the replay from loading.

Scene Start is Replay Start: Automatically aligns the start of your scene with the replay's start. Disable this if you want your first keyframe to appear later.

Enables Catmull Interpolation: By default it uses linear but it might be useful to use smoothing with low density values.
