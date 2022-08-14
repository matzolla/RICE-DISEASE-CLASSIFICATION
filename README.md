# RICE-DISEASE-CLASSIFICATION

## Problem statement

Rice is a staple crop in Egypt, but despite Egypt’s position as the top rice producer in Africa, it still relies on imports
to meet the demands of its population. One of the main causes of this gap in Egypt is rice blast disease, which is
responsible for 30% loss in rice production worldwide. Early detection is the best way to manage crop diseases like rice
blast, but rice blast is easily misclassified as brown spot disease - both are fungal diseases and have similar appearances
in their early stage. With the current scarcity of experienced agricultural extension officers in the country, there is a clear
case for recent technological advances in computer vision to help in early diagnosis, particularly by using multi-spectral
images of crops.

## Objective

The objective of this challenge is to predict the classes of disease of a rice plant in RGB and Infrared images.

## Method

- Transfer learning using [resnet34](https://arxiv.org/abs/1512.03385) and [resnet50](https://arxiv.org/abs/1512.03385) pretrained models using fastai
- Test time augmentation [TTA](https://openaccess.thecvf.com/content/ICCV2021/papers/Shanmugam_Better_Aggregation_in_Test-Time_Augmentation_ICCV_2021_paper.pdf)
- Hue augmentation
- Image side-cropping (didn't work)

## Results

| Models    | Image size      | Number of epoch | TTA |  Logloss|
| ------------- | ------------- | --------    | ------ | ------- |
| `ResNet34`       | 224        | `5`   |        `yes`|  `0.221`  |
| `ResNet50`         | 224         | `10`   |    `yes`|  `0.134`  |


## Contributors
- [Nken allassan](https://github.com/matzolla/)
- [Nancy Fosua Boakye](https://github.com/nancyfosua)
- [Megne Ornela](https://github.com/MEGNEOrnela)
- [Kouame Mathurin](https://)
