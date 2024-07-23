# Developing Multi-Input Models For OCR

![servicedesk](image.png)

## Introduction
DigiNsure Inc. is an innovative insurance company focused on enhancing the efficiency of processing claims and customer service interactions. Their newest initiative is digitizing all historical insurance claim documents, which includes improving the labeling of some IDs scanned from paper documents and identifying them as primary or secondary IDs.

To help them in their effort, you'll be using multi-modal learning to train an Optical Character Recognition (OCR) model. To improve the classification, the model will use **images** of the scanned documents as input and their **insurance type** (home, life, auto, health, or other). Integrating different data modalities (such as image and text) enables the model to perform better in complex scenarios, helping to capture more nuanced information. The **labels** that the model will be trained to identify are of two types: a primary and a secondary ID, for each image-insurance type pair.

## Implementation Path
Develop an Optical Character Recognition (OCR) model to sort categories of ID codes extracted from scanned insurance documents.

- Create a model named OCRModel in PyTorch. It should have the following specifications:

    - A network architecture with different layers to ingest both the image and the type. The layers relative to the image should be saved as a sequential module called image_layer, and compatible the input dimensions of the images (64x64 pixels size).
    - A Conv2d layer with kernel size 3x3, padding 1, and appropriate in/out channels.

- Train the Model: call the model as model and use an appropriate optimizer and loss function to train it. Iterate through your training for ten epochs.
