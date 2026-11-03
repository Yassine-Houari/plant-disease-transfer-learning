# Plant Disease Classification with Transfer Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

A comparison of training from scratch and transfer learning on a reduced PlantVillage subset: 15 classes, 1,000 training images and 300 validation images.

## Results

Validation accuracy after 2 epochs:

| Model | Initialization | Validation accuracy |
| --- | --- | --- |
| ResNet-34 | Random | 46.33% |
| ResNet-34 | ImageNet | **89.67%** |
| EfficientNet-B0 | ImageNet | 82.33% |

The experiment shows how much pretrained weights help on a small dataset. The notebook also supports VGG-19, DenseNet-121 and ViT-B/16.

## Getting started

Download PlantVillage, organize it into `train/` and `val/` folders, then set `data_dir` in the first cell.

```bash
pip install -r requirements.txt
jupyter notebook plant_disease_transfer_learning.ipynb
```

## Author

**Yassine Houari** · [LinkedIn](https://www.linkedin.com/in/yassine-houari-/)
