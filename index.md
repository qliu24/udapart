## CGPart: A Part Segmentation Dataset Based on 3D Computer Graphics Models

CGPart is a comprehensive part segmentation dataset that provides detailed annotations on 3D CAD models, synthetic images, and real test images. Below are some example segmentation annotations from the dataset. More detailed descriptions and experimental results of using CGPart as a benchmark for unsupervised domain adapatation for part segmentation could be found in the [paper](https://arxiv.org/abs/2103.14098).
![overview](images/cgpart_overview.pdf =750x)

### Part Annotation on 3D CAD Models [[Download](https://cs.jhu.edu/~qliu24/CGPart/cgpart_3d.zip)]
![car_3d_demo](images/demo.gif =300x) ![motorbike_3d_demo](images/demo_cruiser.gif =300x)

### Part Annotation on Synthetic Images [Download]

### Part Annotation on Real Test Images [[Download](https://cs.jhu.edu/~qliu24/CGPart/cgpart_real.zip)]
CGPart provides part segmentations on 200 real vehicle images (40 images per category) for evaluation purposes. The images are carefully selected from PASCAL3D+ dataset [1] to contain high-resolution and non-occluded objects from various subtypes and evenly distributed viewpoints. For original uncropped images, please download from the [PASCAL3D+](https://cvgl.stanford.edu/projects/pascal3d.html) website.

### Citation
If you find this project helpful, please consider citing our paper.
```
@article{liu2019semantic,
  author    = {Liu, Qing and Kortylewski, Adam and Zhang, Zhishuai and Li, Zizhang and Guo, Mengqi and Liu, Qihao and Yuan, Xiaoding and Mu, Jiteng and Qiu, Weichao and Yuille, Alan},
  title     = {CGPart: A Part Segmentation Dataset Based on 3D Computer Graphics Models},
  journal   = {arXiv preprint arXiv:2103.14098},
  year      = {2021},
}
```
### References
[1] Xiang, Yu, Roozbeh Mottaghi, and Silvio Savarese. "Beyond pascal: A benchmark for 3d object detection in the wild." IEEE winter conference on applications of computer vision. IEEE, 2014.
