# What program do you use for X?
Most of my assets are made and used in the following programs (They're all free):
- [Davinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve)
- [GIMP](https://www.gimp.org/)
- [Blender](https://www.blender.org/)
- [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/)
- [VTFEdit](https://nemstools.github.io/pages/VTFLib-Download.html)
- [GCFScape](https://nemstools.github.io/pages/GCFScape-Download.html)
- [Crowbar](https://github.com/ZeqMacaw/Crowbar)
- Hammer (Included in any source engine game in the `bin/` directory)
- [BSPSource](https://github.com/ata4/bspsrc)
- And a text editor (I use [VSCode](https://code.visualstudio.com/))
# How do I open/use file type X?
Each program stores its data with a unique file extension. For the majority of the files in the repository, first open the relevant program, then click `File` > `Open`, and select the file.
### .png/.jpg/.gif/.mp3/.mp4
Really?
### .xcf
This is how GIMP stores its files.
### .comp
This is an exported Fusion composition from Davinci Resolve. In order to use it, create a new `Fusion Composition` and open it in the Fusion tab. Then click `File` > `Open` > `Fusion Composition`. This will paste the composition into the node window.
### .blend/.blend1
This is how Blender stores its files. (A .blend1 file is just a backup Blender will make whenever you save a .blend file, but I'll try to keep them out of this repository)
### .dmx
This is how Source Filmmaker stores its files.
### .vmt/.vtf
These are texture files used in the Source Engine, and are opened using VTFEdit. In order for them to show up properly in game, place them in the `tf/` or `usermod/` directory, following the exact file structure they have in this directory.
### .mdl
These are model files used in the Source Engine. To add these to a SFM scene, click `+` > `Add Animation Set for New Model`, then select the .mdl file. (.mdl files can also be viewed in the Half-Life Model Viewer (HLMV) which is located in the same directory as Hammer)
### .vtx/.vvd
These are vertex files used in the Source Engine, which tell the game how to render lights, reflections, bone weight, and textures on a model. As far as I know, they cannot be opened in a meaningful way.
### .qc/.smd
These are script files used as an intermediate step to compile 3d models from a modeling software like Blender into models that can be used in the Source Engine. Unless you're editing models and porting them to SFM, you won't need to touch these files.
### .vmf/.bsp
These are map files used in the Source Engine. .vmf files are uncompiled maps, which can be opened and are compiled into .bsp files in Hammer. .bsp files are compiled maps, can be loaded in any Source game and can be decompiled into .vmf files with BSPSource.
### .vpk
These are Valve Pack files, which are essentially zipped files used by the Source Engine. They can be extracted using GCFScape
# How do I convert file type X to file type Y?
There are already great guides for pretty much any kind of file conversion you can do with the files in this repo, but here are a few:
### .xcf to .png/.jpg/.gif
Open GIMP, click `File` > `Export As` > `Export`.
### .blend to .mdl
There are a couple of guides on the internet, a quick google search will find them for you. I personally think [this one](https://kicodora.com/?p=blendertosfm) is the most clear and concise.
### .mdl/.bsp to .blend
Again, do a quick google search to find a guide. I use [SourceIO](https://github.com/REDxEYE/SourceIO).
### .png/.jpg/.gif to .vtf
Open VTFEdit, click `File` > `Import`, accept the default settings, then click `File` > `Save As`.
### .vmf to .bsp
Open Hammer, click `File` > `Run Map...` > `OK`.
### .bsp to .vmf
Open BSPSource, click `Add`, then go to the `Other` tab, enable `Extract embedded files`, then click `Decompile`.
