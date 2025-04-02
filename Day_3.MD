# Day 3

**Recap from Day 2:** Exporting to models, Animator exploding models, segmentation questions

* **Surface Toolbox:** https://github.com/SlicerMorph/Spr_2021/blob/main/Day_2/Surface_Toolbox/Mesh_edits.md
* **Dynamic Modeler:** https://github.com/SlicerMorph/Spr_2021/blob/main/Day_2/Surface_Toolbox/Mesh_edits.md
* **Markups:** https://github.com/SlicerMorph/Tutorials/tree/main/Markups_1
* Saving Scenes, MRB for sharing
* **Open Anatomy Export:** https://github.com/PerkLab/SlicerOpenAnatomy/blob/master/OpenAnatomyExport/README.md
* Sharing Models. 
* Registration: (Extension in development ANTsPy)

### Using MorphoCloud:
* If you are on the cloud, extension is in `/media/share/MorphoCloudCephShare/SlicerMorph101/SlicerANTsPy`
* Copyy **SlicerANTsPY** extension to your desktop, and then drag the folder onto the Slicer application
* In the popup window, Click the dropdown menu, and choose **Add Python scripted modules to the application** (it should be the second choice, after the ImageStacks option)
* Hit `CTRL+F` and search for **ANTS** and switch to ANTsRegistration module.
* Sample Data to use is in `/media/share/MorphoCloudCephShare/SlicerMorph101/ANTSamples` folder. (No need to copy)

## If using your own computer
* Go to https://github.com/SlicerMorph/SlicerANTsPy
* Click on the green **CODE** button (towards the top of the screen), then choose the `Download ZIP` option. This will download the repository to your computer. Unzip it somewhere easy to find (like your Desktop)
* Drag and drop the SlicerANTsPy-Main folder (which should be the folder uncompressed) onto the Slicer application window, and choose **Add Python scripted modules to the application** (it should be the second choice, after the ImageStacks option) 
* **Mac Users:** for unknown reasons sometimes this option does not work (i.e, there is no **Add Python scripted modules to the application** option inthe pop up menu). In that case cancel the window, and go these steps:
   * In Slicer, go to `Edit->Application Settings->Modules` 
   * Find the **Additional Module paths:** section (middle of the screen). Click the double-arrows on the right `>>`, then click `ADD'
   * Navigate to the unzipped SlicerANTsPy-Main folder and then to the ANTsRegistration folder and click OK. 
   * Repeat the steps above for the ITKANTsCommon folder (also under SlicerANTsPy-Main), and click OK. 
   * Confirm both these paths are added to the list of additional module paths (they should be the bottom entries). 
   * Restart Slicer.

## Sample Data. (for those using their own computer)
* goto https://github.com/muratmaga/ANTSamples
* Click on the green **CODE** button (towards the top of the screen), then choose the `Download ZIP` option. This will download the repository to your computer. Unzip it somewhere easy to find (like your Desktop)


We will use these two samples: **129S1_SVLMJ** and **C57BL_J** (and their landmarks) as interactive examples. 


