# Paddy-pest-detection-using-detectron
This project applies deep learning and computer vision techniques to accurately **segment insects in paddy field images** using the **Mask Region-based Convolutional Neural Network (Mask-RCNN)** framework. It aims to enhance pest detection and enable efficient pest control through early and accurate insect identification.


Insects like rice leafhoppers and stem borers severely affect paddy crop yield. Traditional pest detection methods—such as manual inspection—are time-consuming, error-prone, and inefficient at scale. This project leverages **instance segmentation** using **polygonal annotations** to overcome these challenges and automate pest detection.

## Key Features

- Utilizes **Mask-RCNN** with a ResNet backbone for instance segmentation.
- Implements **polygonal annotations** for accurate boundary detection.
- Includes **data augmentation** to simulate diverse real-world conditions.
- Evaluates model performance using **IoU**, **mAP**, and **Pixel Accuracy**.
- Trained and tested using the **Paddy Pests Dataset** from Kaggle.

## Dataset

- **Source**: [Paddy Pests Dataset – Kaggle](https://www.kaggle.com)
- **Annotations**: Created using [MakeSense.ai](https://www.makesense.ai) with export in **COCO JSON format**.
- Includes various insect types in different lighting, scales, and orientations.

## Tools & Libraries

- [Detectron2](https://github.com/facebookresearch/detectron2)
- PyTorch
- NumPy, OpenCV, Matplotlib
- Google Colab (for training)

## Model Architecture

- **Backbone**: ResNet-50 FPN
- **ROI Pooling** for region extraction
- **Mask Head** for pixel-level binary mask prediction
- **Augmentation**: Random flips, rotations, brightness/contrast adjustment
