# Operations Team
As part of an emergency hurricane response simulation, the Operations Team is responsible for performing computer vision tasks using deep learning and Structure from Motion (SfM). Our goal is to enhance situational awareness and assist disaster responders by analyzing post-hurricane imagery.

## Objectives
* Develop and train classifier to identify damage severity and infrastructure types (buildings, roads)
* Optimize model to improve performance
* Generate a GeoDataFrame with building footprints and their associated damage classifications
* Use OpenSfM to create a small-scale 3D representation of hurricane damage using craft materials, toys, Minecraft, or any other materials available

## Approach
* Implemented a convolutional neural network with an Attention U-Net architecture using ResNet-50 as a baseline
* Processed 4,000+ post-hurricane images from the RescueNet dataset for training
* Defined 11 classes to label infrastructure with varying damage levels (e.g., debris, building-no-damage, building-major-damage, road-clear, road-blocked)
* Model outputs segmentation masks to classify infrastructure and damage level

## Resources Used
* [RescueNet Dataset](https://www.dropbox.com/scl/fo/ntgeyhxe2mzd2wuh7he7x/AHJ-cNzQL-Eu04HS6bvBgcw?rlkey=6vxiaqve9gp6vzvzh3t5mz0vv&e=1&dl=0): 4494 high-resolution UAV images captured after Hurricane Michael
* [ResNet-50](https://docs.pytorch.org/vision/stable/models/generated/torchvision.models.resnet50.html): Pretrained backbone
* [Pytorch](https://pytorch.org/): Framework used for model development and data augmentation
