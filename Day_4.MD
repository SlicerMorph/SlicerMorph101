# Day 4

## Course evaluation (10 minutes)

[Please fill the course evaluation](https://forms.gle/egesfcdzQjmqfRCt9)

## Recap from Day 3
* ANTsPy works fine on windows and Mac, and the crash was specific to MorphoCloud. Quick demo of the functionality 

## MorphoDepot Practice:
There are two **personas** in MorphoDepot: The people who are assigned tasks and contributing (e.g., students, lab members, remote collaborators), and repository owners (people who created the original data). You will first be a **student assigned a task**. To do that, do these steps:
|Organ|Assignee|
|------| ----------------| 
| Liver	| Andres, Kaan, Pedro| 
| Left Lung	| Busra, Leigha, Richardo| 
| Right Lung| 	Domini, Marina| 
| Heart	| Isa, Michal, Roberta| 
| Kidneys| 	Jessica, Samuel, Ozlem| 
| Brain	| Jonas, Pedro| 

### Student Workflow
1. Go to https://github.com/amm554/E15-blank on the web browser, and open an issue. Your issue title should follow this convention:</br>
**FirstName LastName, assigned task** 
(See your assigned tasks in the table below). Then provide a short description of the task (e.g., I will segment liver)
2. I (the repository owner) will assign this task to you (This is the responsibility of the repo owner, and it is a necessary step)
3. Once you see in the issues page that the task is assigned to you, you can start using the MorphoDepot module in Slicer to retrieve your task and start segmenting. The tab you will be using for this is called **ANNOTATE**.  Segmentation doesn't need to be perfect. Just segment broadly, spend maybe 5-10 minutes max.
4. As you are progressing in your segmentation, if you feel like saving your work, you will NOT use the Save Data or Export As functionality. You have to use the button that says **Commit and Push**, and for that you need to provide a short commit message and a more detailed description of your work in the larger text box. 
5. When you are ready for me to review, you will hit the **Request PR (Pull Request) review** button.
6. I will make a comment about that you need to do more work, and send it back to you (your PR will be converted from Ready to Review state to draft).
7. You will make a few more changes and then repeat steps 4 and 5 to update your PR.
8. I will merge your work to the repository.

### Review Workflow
Murat will demo how things work on the reviewer side

### A new repo creation (Create tab).

## Photogrammetry in Slicer
* [Photogrammetry Extension User Guide and Tutorial](https://github.com/SlicerMorph/SlicerPhotogrammetry?tab=readme-ov-file#user-guide)
* [Photogrammetry Extension Video Tutorial](https://www.youtube.com/watch?v=YRHlb0dGyNc&t=9s)

### Our papers on an inexpensive setup (<$1000) to do photogrammetry
* [Zhang & Maga. 2023. Integrative Organismal Biology- Open access](https://academic.oup.com/iob/article/5/1/obad024/7221338#supplementary-data) 
* [Supplementary Instructions on the photogrammetry setup: Camera, lightbox, turntable, etc](https://docs.google.com/document/d/1YP72Q90UbsUUryi3Yeu8ccRSJuibTQni/)
* [Oshane, Zhang and Maga. 2025. SlicerMorph photogrammetry: an open-source photogrammetry workflow for reconstructing 3D models. Biology Open. 14 (8): bio062126.](https://journals.biologists.com/bio/article/14/8/bio062126/368988/SlicerMorph-photogrammetry-an-open-source?searchresult=1)


## Deep learning based segmentation models in Slicer:

* **NNInteractove:** AI Assisted interactive segmentation https://github.com/SlicerMorph/Tutorials/blob/main/MorphoCloud/NNInteractive.MD

### Other AI tools of interest:

* **TotalSegmentator:** For human clinical imaging: https://github.com/lassoan/SlicerTotalSegmentator
* **DentalSegmentator:** Cone-beam CT for dentistry: https://github.com/gaudot/SlicerDentalSegmentator
* **MonaiLabel:** A client/server approach for training custom deep-learning models, and making inference from them. https://docs.monai.io/projects/label/en/latest/quickstart.html
* **MEMOS:** E15 mice multi-organ segmentation model. https://github.com/SlicerMorph/SlicerMEMOS (works currently only with Slicer v5.8.1)

## If we have time:

* **ScriptEditor:** To develop, edit and execute python scripts inside Slicer
* **Scripting via Vibe Coding**


