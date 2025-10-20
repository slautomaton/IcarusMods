# IcarusMods
A collection of ICARUS EXMODZ files I use.

ICARUS Modding Primer: Icarus is based on Unreal Engine and its game files are a collection of .json files that are pack using UE4 packing tools. The simplest method to mod the game is to extract .json files from .pak files from your game directory, modify values in said .json, re pack the files into a modded_P.pak file, place the modded .pak file into a "mods" folder within the /paks directory of the game, and then load the game.  The issue with this method is that if you use multiple mods that edit the same underlying .json file, only the latter mod will take effect, superseding the edits needed for an earlier loaded mod to work. Furthermore, since mods are generally loaded last altogether, if the modded .pak file is not based on the same weekly version of the base game, your gameplay risks excluding content since the mod was last created/updated. For example, if you modified or used a mod that was created with D_processingrecipes.json from w151, but you want to play in w202, newly added items or changes to processing times since w151 will be excluded from your gameplay. To compensate, you must merge your modded file with the current base game file to ensure you're playing the most current version. Also, merging or working with .json files is sensitive to whitespace so use visual studio or notepad++ or something coding IDE that lets you parse and edit .json files without adding whitespace (do not use Word or LibreOffice). 

This method of using a series of superseding .json files works just fine as long as you're cognizant of the delta's week over week. But that is also the problem, you have to update your mods to merge with the updated game week over week. 

Alternatively, you can use the EXMOD format instead. EXMOD packages take the extra step to capture only the changes to the games base .json file. So as long as what you modify tends to be static over time (avoid modding items and base gameplace that changes often like recipes), its least likely to break during week over week releases and allows only what has changed to be supplanted into the base game, without the tedious effort merge files week over week.

I have provided EXMODZ (EXMOD Zip) files for your consumption. Use jimk's Mod Manager (IMM) to I
1. Import EXMODZ files (which extracts them into a working directory)
2. Select and install which mods you'd like to play with
3. Installing using IMM will merge all relevant .json file into 1 singular _P.pak file and copy it into your /paks/mods/ directory.
4. Play the game.

Download Jimk's IMM here:
https://github.com/Jimk72/Icarus_Software



