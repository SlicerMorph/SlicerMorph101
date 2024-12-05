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
2. ```/media/volume/Slicer/Slicer```

Now Slicer should start and we can proceed normally.


## Scripting in Slicer
* Install the `ScriptEditor` extension (to modify the scripts inside the Slicer)
* We will use code snippets from Script Repository (Slicer Developer's guide): https://slicer.readthedocs.io/en/latest/developer_guide/script_repository.html

Most of the time, all we have to do is to make sure the file paths are changed to correct spot, and/or make sure the specific objects/nodes (e.g., "F") exists

## If we have time:

* Open Anatomy Export
* Image Registration 
* Model Registration


