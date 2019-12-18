# 3DPeople-Dataset
First dataset of dressed humans with specific geometry representation for the clothes. It contains ~2 Million images with 40 male/40 female performing 70 actions. Every subject-action sequence is captured from 4 camera views and annotated with: RGB, 3D skeleton, body part and cloth segmentation masks, depth map, optical flow, and camera parameters.

![GANimation](https://cv.iri.upc-csic.es/images/teaser_v3_lr.png)

### Train/Test Splits:
* Train: woman01-woman33  man01-man33
* Test:  woman34-woman40  man34-man40

### Visualize data:
Download jupyter notebook. You can use the [sample dataset](https://cv.iri.upc-csic.es/Dataset/3DPeople_sample.tar.xz).
```
conda create -n 3dpeople
source activate 3dpeople
conda install matplotlib opencv pillow scipy
conda install -c conda-forge ipywidgets=7.2.1
conda install -c plotly chart-studio
jupyter nbextension enable --py widgetsnbextension
jupyter notebook vis_dataset.ipynb 
```
Inside notebook select the sequence to visualize: "seq_name=..." in first cell


### Contact:
cvlab.iri@gmail.com


### If you use this data cite:
```
@inproceedings{pumarola20193dpeople,
    title={{3DPeople: Modeling the Geometry of Dressed Humans}},
    author={Pumarola, Albert and Sanchez, Jordi and Choi, Gary and Sanfeliu, Alberto and Moreno-Noguer, Francesc},
    booktitle={International Conference in Computer Vision (ICCV)},
    year={2019}
}
```
