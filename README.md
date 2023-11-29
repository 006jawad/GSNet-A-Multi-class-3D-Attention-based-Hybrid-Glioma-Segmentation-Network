# GSNet: a multi-class 3D attention-based hybrid glioma segmentation network
`Optics Express Vol. 31, Issue 24, pp. 40881-40906 (2023)`<br>
`DOI:`https://doi.org/10.1364/OE.499054

## Our contribution
We have developed a hybrid end-to-end multi-class 3D CNN-based segmentation network named
GSNet (glioma segmentation network) for automating the segmentation process. Our network
consists of 5 levels in the encoder and 5 levels in the decoder, forming a 5-stage segmentation
network incorporating attention-based skip connections. Our simulation results demonstrate
a significant improvement, with GSNet performing on par with, if not surpassing, some of
the top-performing segmentation networks developed for glioma segmentation. The overall
contribution of our work is stated below:<br>
• Creating an end-to-end segmentation network (GSNet) capable of segmenting glioma
segments with high efficiency.<br>
• Developing a robust 3D network capable of pooling both low-level and high-level attributes
from MRIs.<br>
• Producing an overall lightweight model, that is able to perform quick segmentation while
dealing directly with 3D images, despite training with significantly imbalanced data.<br>
• Achieving high accuracy without utilizing extensive image pre-processing. Obtaining
performance scores that are large enough to establish GSNet as a state-of-the-art model.<br>
• Compressing the entire pipeline into a user-friendly GUI application, which can serve
as an automated tool enabling practitioners and medical personnel to efficiently segment
glioma ROIs.
![Alt Text](extra/get2.jpg)
## GSNet-based web app
To apply our model as a medical imaging tool, we have compressed the entire pipeline in an easy-to-use web-based application (web app) which takes in input as 3D MRI images in the format of ‘.nii’ files. With the input of FLAIR, t1, t1ce, and t2 MRI scans, our web app can produce the corresponding segmentation masks for WT, TC, and ET regions and further save them locally in the ‘.nii’ file format in under 20 seconds. Due to the lightweight size, the web app creates the segmentation masks very quickly. The pre-trained weight file corresponding to this web app created from training with the BraTS 2020 dataset is around 24.7MB. The total size of the web app including the weight file is 36.8MB. The outputs which are saved as ‘.nii’ files are around 8MB each so 24MB in total (3 outputs for 3 separate regions). We have deployed the web app on our local system, which runs through a web browser at `https://127.0.0.1:5000`. The web app creates the outputs and saves them in any local folder. The corresponding indication is shown (the red-marked lines at the bottom) on the next page of the web app. We have visualized the saved outputs using the software ITK-SNAP. An example of the saved outputs is shown below. The full installation process along with the necessary files is provided at the [GitHub link](https://github.com/006jawad/GSNet_/tree/main/WebApp).

![Alt Text](extra/Visualizingthesavedsegmentationmasks.gif)
*****************************************************************************************************************************************
# Citation Text
For attribution, please follow the citation format provided below:<br>

Md Tasnim Jawad, Ashfak Yeafi, and Kalyan Kumar Halder, "GSNet: a multi-class 3D attention-based hybrid glioma segmentation network," Opt. Express 31, 40881-40906 (2023)

# BibTeX
@article{jawad2023gsnet,<br>
  title={GSNet: a multi-class 3D attention-based hybrid glioma segmentation network},<br>
  author={Jawad, Md Tasnim and Yeafi, Ashfak and Halder, Kalyan Kumar},<br>
  journal={Optics Express},<br>
  volume={31},<br>
  number={24},<br>
  pages={40881--40906},<br>
  year={2023},<br>
  publisher={Optica Publishing Group}<br>
}

Or, 

@article{Jawad:23,<br>
author = {Md Tasnim Jawad and Ashfak Yeafi and Kalyan Kumar Halder},<br>
journal = {Opt. Express},<br>
keywords = {Edge detection; Genetic algorithms; Image restoration; Mathematical methods; Segmentation; Spatial resolution},<br>
number = {24},<br>
pages = {40881--40906},<br>
publisher = {Optica Publishing Group},<br>
title = {GSNet: a multi-class 3D attention-based hybrid glioma segmentation network},<br>
volume = {31},<br>
month = {Nov},<br>
year = {2023},<br>
url = {[https://opg.optica.org/oe/abstract.cfm?URI=oe-31-24-40881](https://opg.optica.org/oe/fulltext.cfm?uri=oe-31-24-40881)https://opg.optica.org/oe/fulltext.cfm?uri=oe-31-24-40881},<br>
doi = {10.1364/OE.499054},<br>
}
