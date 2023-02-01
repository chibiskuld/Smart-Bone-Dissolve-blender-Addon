# Smart-Bone-Dissolve-blender-Addon
This addon is aimed to ease the process of removing excess bones from an already rigged mesh or collection of meshes, while also preserving their weights. A comon use case would be turning a model rigged for animation into a game-ready model with a less complex armature

## How it works
Applying the addon to any number of selected armature bones will dissolve them and add their weights to any remaining parent bones weights

This applies to all meshes that are parented to the selected armature and use it in an Armature modifier

If a mesh does not have a vertex group corersponding to a dissolved bone, it will not be affected

If a mesh has a vertex group corersponding to a dissolved bone, but not one of a parent bone, then it will be created and populated

Redundant vertex groups of all dissolved bones will be removed from affected meshes

## How to install
 - Download the included **SmartBoneDissolve.py** file
 - In blender, go to **Edit > Preferences > Add-ons**
 - Click the **Install** button and select the **SmartBoneDissolve.py** file
 - Enable the addon with the checkmark
 
 ## How to use
 - Once installed, the option will appear under the **Armature menu** in 3D View when in Armature Edit mode
 - Simply select the bones you want to dissolve in Edit mode and click **Armature > Smart Bone Disssolve**
