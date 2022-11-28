# il2_artillery_RC
Script to allow artillery to be called on any reachable point of the map, in multiplayer, using IL2 GB remote console. 
You can call the remote console directly using the binary executable available in the IL2 GB installation folder or you can also use discord if you use this tool: https://github.com/Super-truite/il2_discord_bot
Before using on your mission, make sure you keep a copy of your mission!

## Download
Download the .zip file from : https://github.com/Super-truite/il2_artillery_RC/releases/tag/v0.1
Extract anywhere on the machine where you will edit your mission 

## Configuration
Set the path of your mission file in :  dist/config.ini

## Add the group to your mission
In the mission editor, on your mission, import the ArtilleryRCgroup.Group (File -> Import From File)

## Define the map boundaries
Place the map_boundary object at the top right point of the map
![Alt text](img/map_boundary.PNG?raw=true "Title")

## Place the limits of the artillery zones for Axis and Allies
For Axis, place Artillery_Zone_Axis_1 and Artillery_Zone_Axis_2 and for allies,
place : Artillery_Zone_Allies_1 and Artillery_Zone_Allies_2. Those 
defines rectangles where the artillery will be able to fire.
![Alt text](img/boundary_rectangles.PNG?raw=true "Title")

## Run the exe
in the dist folder, run add_artillery_tp_map.
ReOpen the map in the editor. You should obtain all the necessary logic to launch the artillery: 
![Alt text](img/after_executing.PNG?raw=true "Title")
The max range of the artillery used in the editor is taken into account.
You can change the artillery type, but make sure to do it before running the script and do not change the name of the artillery before running the script! 
You can add later more artillery trigger linked to the leader.

