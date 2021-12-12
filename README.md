# MF-PSN

## A Deep-shallow and Global-local Multi-feature Fusion Network for Photometric Stereo

Yanru LIU, **Yakun JU(co-corresponding)**, Muwei JIAN, Feng GAO, Yuan RAO, Yeqi HU, Junyu DONG(co-corresponding)

## Environment

Implemented in PyTorch with Ubuntu 18.04.

Python: 3.6.9 

PyTorch 1.4.0 with scipy, numpy, etc.

GTX 1080 (8G)

## download these two training datasets:
Blobby shape dataset (4.7 GB), and Sculpture shape dataset (19 GB), via: 

```shell
sh scripts/download_synthetic_datasets.sh
```
## download these test datsets:

DiLiGenT main dataset (default) (850MB), via:
```shell
sh scripts/prepare_diligent_dataset.sh  
```
or   https://drive.google.com/file/d/1EgC3x8daOWL4uQmc6c4nXVe4mdAMJVfg/view

DiLiGenT test dataset (759MB), via:

https://drive.google.com/file/d/1LzRMwrxWMdV_ASYzUMm9ZlAmyBs-QJRs/view

Light Stage Data Gallery, via:

https://vgl.ict.usc.edu/Data/LightStage/

Apple&Gourd dataset, via:

http://vision.ucsd.edu/~nalldrin/research/

## Testing on your device:
```shell
python eval/run_model.py --retrain data/models/MF-PSN.pth.tar --in_img_num X 
```
You can change X to adjust the number of the input image. 

## Results on the DiLiGenT benchmark dataset:

We have provided the estimated surface normals and error maps on the DiLiGenT benchmark dataset (under 96 input images), in document ``results''



