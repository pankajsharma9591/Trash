## Project Details
Pipeline based on EfficientDet project - https://github.com/yhenon/pytorch-retinanet

<br />
<br />
<br />

# Supported Models
  - Resnet18
  - Resnet34
  - Resnet50
  - Resnet101
  - Resnet152
    

<br />
<br />

## Installation

Supports 
- Python 3.6
- Cuda 9.0 (Other cuda version support is experimental)
    
`cd installation`

`cat requirements.txt | xargs -n 1 -L 1 pip install`

<br />
<br />
<br />

## Functional Documentation
[Link](https://abhi-kumar.github.io/5_pytorch_retinanet_docs/)

<br />
<br />
<br />

## Pipeline

- Load Dataset

`gtf.Train_Dataset(root_dir="../sample_dataset", coco_dir="kangaroo", img_dir="images", set_dir="Train", batch_size=8, image_size=512, use_gpu=True)`

- Load Model

`gtf.Model(model_name="resnet18");`

- Set Hyper Parameters

`gtf.Set_Hyperparams(lr=0.0001, val_interval=1, es_min_delta=0.0, es_patience=0)`

- Train

`gtf.Train(num_epochs=2, output_model_name="trained.pt");`



<br />
<br />
<br />

## TODO

- [x] Add support for Coco-Type Annotated Datasets
- [x] Add support for VOC-Type Annotated Dataset
- [x] Test on Kaggle and Colab 
- [ ] Add validation feature & data pipeline
- [ ] Add Optimizer selection feature
- [ ] Enable Learning-Rate Scheduler Support
- [ ] Enable Layer Freezing
- [ ] Set Verbosity Levels
- [ ] Add Project management and version control support (Similar to Monk Classification)
- [ ] Add Graph Visualization Support
- [ ] Enable batch proessing at inference
- [ ] Add feature for top-k output visualization
- [x] Add Multi-GPU training
- [ ] Auto correct missing or corrupt images - Currently skips them
- [ ] Add Experimental Data Analysis Feature


<br />
<br />
<br />

## External Contributors list 

- https://github.com/THEFASHIONGEEK: Multi GPU feature
"# Trash_detection" 
