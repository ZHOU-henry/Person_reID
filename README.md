# Person_reID
Person re-identification is usually regarded as an image retrieval problem of spotting the person in cameras.

Whole work is based on ([Person_reID_baseline_pytorch](https://github.com/layumi/Person_reID_baseline_pytorch/blob/master/README.md)) and ([person-reid-3d](https://github.com/layumi/person-reid-3d)), here just rerun these codes for practicing.

![Magic Mirror](https://github.com/layumi/3D-Magic-Mirror/raw/master/doc/rainbow_github.gif)

## Prerequisites

- Python 3.6+
- GPU Memory >= 6G
- Numpy
- Pytorch
- pip install timm
- pip install pretrainedmodels
- apex (for float16) 
- [pretrainedmodels](https://github.com/Cadene/pretrained-models.pytorch)

### Installation

- Install Pytorch 
- Install Torchvision 
- Install apex from the source
```
git clone https://github.com/NVIDIA/apex.git
cd apex
python setup.py install --cuda_ext --cpp_ext
```

### Dataset

Need download from the source and then store in the Market folder.

Download [Market1501 Dataset](https://zheng-lab.cecs.anu.edu.au/Project/project_reid.html) [[Google]](https://drive.google.com/file/d/0B8-rUzbwVRk0c054eEozWG9COHM/view)

python prepare.py


### Pre-train model

Use some pre-train model, e.g.: ResNet-50, Swin_transformer....

## Model

After run the train.py file, the training model details and NN parameters will be stored in the model folder.

## OG-Net

This folder is from ([person-reid-3d](https://github.com/layumi/person-reid-3d)), here just rerun these codes for practicing.

And we can rerun OG-Net code and compare with the baseline models.
