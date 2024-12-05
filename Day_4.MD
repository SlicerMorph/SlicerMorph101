# Day 4

## Course evaluation (15 minutes)

Please fill the course evaluation at https://forms.gle/c1sRaPztoimW335U9

## Deep learning based segmentation models in Slicer:

* **TotalSegmentator:** For human clinical imaging: https://github.com/lassoan/SlicerTotalSegmentator
* **DentalSegmentator:** Cone-beam CT for dentistry: https://github.com/gaudot/SlicerDentalSegmentator
* **AutoSeg3d:** Model farm for different clinical modalities. Based on MONAI. https://github.com/lassoan/SlicerMONAIAuto3DSeg/releases/tag/ModelsTestResults
* **MonaiLabel:** A client/server approach for training custom deep-learning models, and making inference from them. https://docs.monai.io/projects/label/en/latest/quickstart.html
* **MEMOS:** E15 mice multi-organ segmentation model. https://github.com/SlicerMorph/SlicerMEMOS

To try these we need to run Slicer from the command line with these steps. First open a terminal window in the MorphoCloud then copy and paste these two lines one by one:
1. ```export CUDA_ViSIBLE_DEVICES=0```
2. ```/media/volume/MyData/Slicer/Slicer```

Now Slicer should start and we can proceed normally and we will try to do a deep learning based segmentation of a mouse embryo. Search the extension catalogue for `MEMOS` and install SlicerMEMOS extension. After Slicer restarts, use the `Module Finder` (CTRL+F) to search for `PyTorch Utils`. We have to configure the deep-learning framework Torch (or pyTorch for it is python version) for our environment. Luckily this is fairly easy with this module. But before we do this, make sure your python window is visible (it is the little snake icon at the far right of the top tow of icons, or you can use CTRL+3). That way we can see if there are any errors associated with the libraries being installed. After enabling your python console, click on `Install PyTorch` in the module panel and the module will find and download all necessary libraries for your environment. This may take as long as 4-5 minutes. After that we will be ready to try the `MEMOS` extension. But first we need a volume to segment.

1. Go to `Sample Data` module, scroll down to find the MEMOS section of the Sample Data, and click `Sample E15 Embryo`. 
2. Search for MEMOS module (CTRL+F) in Slicer and switch to it.
3. First time you switch to MEMOS, it will also install bunch of libraries it needs, including the deep-learning model it will use. This may take about 1-2 minute, but it is a one-time thing. 

## Scripting in Slicer
* Install the `ScriptEditor` extension (to modify the scripts inside the Slicer)
* We will use code snippets from Script Repository (Slicer Developer's guide): https://slicer.readthedocs.io/en/latest/developer_guide/script_repository.html

Most of the time, all we have to do is to make sure the file paths are changed to correct spot, and/or make sure the specific objects/nodes (e.g., "F") exists

## If we have time:

* Open Anatomy Export
* Image Registration 
* Model Registration


