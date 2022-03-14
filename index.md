## UDA-Part: A Part Segmentation Dataset Based on 3D Computer Graphics Models

UDA-Part is a comprehensive part segmentation dataset that provides detailed annotations on 3D CAD models, synthetic images, and real test images. Below are some example segmentation annotations from the dataset. More detailed descriptions and experimental results of using UDA-Part as a benchmark for unsupervised domain adapatation for part segmentation could be found in the [paper](https://arxiv.org/abs/2103.14098).  
<img src="images/cgpart_overview.jpg" alt="cgpart_overview" width="750"/>

### Part Annotation on 3D CAD Models [[Download](https://cs.jhu.edu/~qliu24/CGPart/cgpart_3d.zip)]
UDA-Part is composed of 3D CAD models from 5 vehicle categories: *car*, *motorbike*, *aeroplane*, *bus*, and *bicycle*. For each category, we select 4 to 5 high-quality 3D CAD models from ShapeNetCore [1]. Each CAD model represents a common prototype (i.e., subtype) of the category it belongs to. In total, we select 21 CAD models to be included and annotated in UDA-Part. Below are some example part annotations on 3D CAD models.  
  
<img src="images/demo.gif" alt="demo_car" width="300"/> <img src="images/demo_cruiser.gif" alt="demo_motorbike" width="300"/>  
  
<img src="images/demo_jet.gif" alt="demo_aeroplane" width="300"/> <img src="images/demo_utility.gif" alt="demo_bicycle" width="300"/>

### Part Annotation on Synthetic Images [[Download](https://livejohnshopkins-my.sharepoint.com/:u:/g/personal/qliu24_jh_edu/Ea_mSpbaU85LrCctmNlyCwgB8JMAVrzCJ56eXu-X2S0mRQ?e=AsnUSy)]
Based on the CAD models and their part annotations, we render a large-scale synthetic image dataset with automatically generated part segmentation ground-truth. We use Blender as our renderer and randomize the parameters, including lighting, background, object texture, and viewpoint, to enable nuisance factor control and facilitate domain generalization. Example code could be found at [here](https://github.com/qliu24/render-3d-segmentation). The files in the above download link are cropped and resized. The total file size is 67 GB.

### Part Annotation on Real Test Images [[Download](https://cs.jhu.edu/~qliu24/CGPart/cgpart_real.zip)]
UDA-Part also provides part segmentations on 200 real vehicle images (40 images per category) for evaluation purposes. The images are carefully selected from PASCAL3D+ dataset [3] to contain high-resolution and non-occluded objects from various subtypes and evenly distributed viewpoints. We use the VGG Image Annotator to manually label the parts on the images. Below are some example part annotations on real test images and comparisons with PascalPart [4]. For original uncropped images, please download from the [PASCAL3D+](https://cvgl.stanford.edu/projects/pascal3d.html) website.  
<img src="images/cgpart_vs_ppart.jpg" alt="cgpart_vs_ppart" width="750"/>

### Citation
If you find this project helpful, please consider citing our paper.
```
@inproceedings{liu2022learning,
  author = {Liu, Qing and Kortylewski, Adam and Zhang, Zhishuai and Li, Zizhang and Guo, Mengqi and Liu, Qihao and Yuan, Xiaoding and Mu, Jiteng and Qiu, Weichao and Yuille, Alan},
  title = {Learning Part Segmentation through Unsupervised Domain Adaptation from Synthetic Vehicles},
  booktitle = {CVPR},
  year = {2022},
}
```
### References
[1] Chang, Angel X., et al. "Shapenet: An information-rich 3d model repository." arXiv preprint arXiv:1512.03012 (2015).  
[2] Community, B. O. (2018). "Blender - a 3D modelling and rendering package." Stichting Blender Foundation, Amsterdam. Retrieved from http://www.blender.org.  
[3] Xiang, Yu, Roozbeh Mottaghi, and Silvio Savarese. "Beyond pascal: A benchmark for 3d object detection in the wild." IEEE winter conference on applications of computer vision. IEEE, 2014.  
[4] Chen, Xianjie, et al. "Detect what you can: Detecting and representing objects using holistic models and body parts." IEEE conference on computer vision and pattern recognition. 2014.
