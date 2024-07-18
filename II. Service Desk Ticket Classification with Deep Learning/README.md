# Service Desk Ticket Classification with Deep Learning

![servicedesk](image.png)

## Introduction
CleverSupport is a company at the forefront of AI innovation, specializing in the development of AI-driven solutions to enhance customer support services. Their latest endeavor is to engineer a text classification system that can automatically categorize customer complaints. 

Our role as a data scientist involves the creation of a sophisticated machine learning model that can accurately assign complaints to specific categories, such as mortgage, credit card, money transfers, debt collection, etc.

## Implementation Path
Classify service desk tickets into categories using a CNN to streamline customer services.

- Define a CNN classifier with the following layers: an embedding layer, a 1D convolution layer, and a linear layer.
- Train a classifier on train_data using a suitable optimizer. Run the training for only 3 epochs.
- Test a classifier on test_data, storing the predictions in a list called predictions.
- Calculate the accuracy, per-class precision, and recall for your trained classifier on the test_data. Save the metrics as variables with the corresponding names: accuracy, precision, and recall, with precision and recall saved as lists.
