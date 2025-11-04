# Day 2

## Recap & Q&A from Day 1
Animator: Review how to set it up correctly.

If you want to fix the ffmpeg issue and be able to create mp4s both from Animator and ScreenCapture module. Do these steps on your MC instance:
1. Switch to `ScreenCapture` module
2. Expand the **Advanced** section
3. Find the field that says FFMPEG executable and paste this path `/media/share/MorphoCloudCephShare/ffmpeg/ffmpeg`
Note that this path is only available if you have mapped the shared data drive (MorphoCloudCephShare) to your instance. The instructions to do so are at the main course web page. 


## Segmentation ##
1. Use of consistent terminology and colors for segmentation: https://github.com/SlicerMorph/Tutorials/blob/main/Segmentation/colors-and-terms/README.md
1. Do a self-paced exercise, and everybody will use the BrainTumor data from the Slicer's SampleData module to do the tutorial as written, which is here: https://github.com/SlicerMorph/Tutorials/tree/main/Segmentation
3. Review some of the keyboard shortcuts available through SlicerMorph customizations. 
3. Then we will interactively explore the turtle data for more of the segmentation tools in Slicer.

Other modules we will investigate are:

* **Segment Statistics:** https://slicer.readthedocs.io/en/latest/user_guide/modules/segmentstatistics.html
* **Segment Cross Sectional Area (provided by Sandbox Extension)**
* **Colorize Volume (provided by Sandbox extension):** https://github.com/SlicerMorph/Tutorials/tree/main/ColorizeVolume
* **MorphoSourceImport:** https://github.com/SlicerMorph/Tutorials/blob/main/MorphoSourceImport/README.md


