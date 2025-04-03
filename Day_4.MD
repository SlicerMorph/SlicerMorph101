# Day 4

## Course evaluation (15 minutes)

[Please fill the course evaluation](https://docs.google.com/forms/d/e/1FAIpQLSdCJTn4fymDVSr-Sh3Q7wLMXSte_KqgxuN_JHutVE_zeCmCIA/viewform?usp=dialog)

## Photogrammetry in Slicer
* [Photogrammetry Extension User Guide and Tutorial](https://github.com/SlicerMorph/SlicerPhotogrammetry?tab=readme-ov-file#user-guide)
* [Photogrammetry Extension Video Tutorial](https://www.youtube.com/watch?v=YRHlb0dGyNc&t=9s)

### Our paper on an inexpensive setup to do photogrammetry
* [Zhang & Maga. 2023. Integrative Organismal Biology- Open access](https://academic.oup.com/iob/article/5/1/obad024/7221338#supplementary-data) 
* [Supplementary Instructions on the photogrammetry setup: Camera, lightbox, turntable, etc](https://docs.google.com/document/d/1YP72Q90UbsUUryi3Yeu8ccRSJuibTQni/)
* [Oshane, Zhang and Maga. 2025. Preprint that compares the models generated from previous workflow to the current extensions](https://www.biorxiv.org/content/10.1101/2025.03.07.641939v1)


## Deep learning based segmentation models in Slicer:

* **TotalSegmentator:** For human clinical imaging: https://github.com/lassoan/SlicerTotalSegmentator
* **DentalSegmentator:** Cone-beam CT for dentistry: https://github.com/gaudot/SlicerDentalSegmentator
* **AutoSeg3d:** Model farm for different clinical modalities. Based on MONAI. https://github.com/lassoan/SlicerMONAIAuto3DSeg/releases/tag/ModelsTestResults
* **MonaiLabel:** A client/server approach for training custom deep-learning models, and making inference from them. https://docs.monai.io/projects/label/en/latest/quickstart.html
* **MEMOS:** E15 mice multi-organ segmentation model. https://github.com/SlicerMorph/SlicerMEMOS

1. Go to `Sample Data` module, scroll down to find the MEMOS section of the Sample Data, and click `Sample E15 Embryo`. 
2. Search for MEMOS module (CTRL+F) in Slicer and switch to it.
3. First time you switch to MEMOS, it will also install bunch of libraries it needs, including the deep-learning model it will use. This may take about 1-2 minute, but it is a one-time thing. 


## If we have time:

* Scripting and AI. 


