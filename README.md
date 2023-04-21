
# Image Segmentation and Depth Estimation

As one of the most intricate tasks - capturing and deciphering meaning from light, the machine now shows astounding results on previously untouched problems, thanks to Deep Learning in Computer Vision. Image Segmentation and Depth Estimation stand as testaments to this advancement. The machine now adeptly partitions an image into different segments and extracts depth information of the foreground entities from a single image.

In Image Segmentation, the segments represent different entities. See the example below showcasing the model's skill of separating the image into segments.

![Segmentation before-after](images/bg_fg_mask.jpeg) ![Segmentation after](images/mask.jpeg)

In Depth Estimation, extract depth information with exceptional quality. See the below example showing depth extraction from an image.

![Depth estimation before](images/bg_fg_depth.jpeg) ![Depth estimation after](images/depth.jpeg)

In this project, the presented Fully-Convolutional Neural Network Model accepts a background and a background-foreground image. The model outputs the segmentation and depth mapping of the foreground object.

Check out the content structure below for more information:

- [Model Architecture](docs/architecture.md)
- [Dataset](docs/dataset.md)
- [Deciding Loss Function](docs/deciding_loss_function.md)
  - [Mask Prediction](docs/deciding_loss_function.md#mask-prediction)
  - [Depth and Segmentation Prediction](docs/deciding_loss_function.md#depth-and-segmentation-prediction)
- [Training](docs/training.md)
  - [RMSE + (BCE & Dice)](docs/training.md#rmse--bce--dice)
  - [SSIM + Dice](docs/training.md#ssim--dice)
  - [LR Range Test](docs/training.md#lr-range-test)
  - [RMSE + (BCE & Dice) with New LR and No Augmentation](docs/training.md#rmse--bce--dice-with-new-lr-and-no-augmentation)
- [Project Setup](docs/project_setup.md)