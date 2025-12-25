# Visual Entailment Using Deep Learning

## Project Overview
This project explores the task of visual entailment, which involves determining the logical relationship between an image and a natural language hypothesis. Given an image and a corresponding textual statement, the model predicts whether the hypothesis is entailed by the image, contradicts it, or is neutral.

The project combines computer vision and natural language processing techniques, using deep learning models to jointly reason over visual and textual information. This multimodal approach reflects real world reasoning tasks where understanding requires both visual context and language comprehension.

## Motivation
Visual entailment is a challenging problem at the intersection of vision and language understanding. It is relevant to applications such as visual question answering, image based reasoning systems, and assistive AI technologies.

Automating visual entailment enables machines to reason more effectively about images and supports the development of more robust multimodal intelligence systems.

## Dataset Description
The dataset consists of paired image and text samples, where each example includes:
- An image
- A textual hypothesis
- A ground truth label indicating entailment, contradiction, or neutrality

Textual data is tokenised and encoded, while images are preprocessed into a consistent format suitable for deep learning models. Labels are encoded numerically for training.

## Methodology

### Data Preprocessing
Images are resized and normalised before being passed to the vision model. Text inputs are cleaned, tokenised, and converted into numerical representations. The dataset is split into training and validation sets to evaluate generalisation performance.

### Model Architecture
The model follows a multimodal architecture consisting of:
- A vision encoder to extract visual features from images
- A text encoder to process natural language hypotheses
- A fusion layer that combines visual and textual representations
- A final classifier that predicts the entailment relationship

This design allows the model to jointly reason over both modalities when making predictions.

### Training Strategy
The model is trained using an appropriate optimiser and categorical cross entropy loss. Accuracy is used as the primary evaluation metric. Training progress is monitored through loss and accuracy curves to assess convergence and potential overfitting.

## Evaluation
Performance is evaluated on the validation set using classification accuracy. Additional analysis is conducted through confusion matrices and classification reports to better understand model behaviour across entailment classes.

Training and validation curves are analysed to assess generalisation and learning stability.

## Inference on Unseen Data
The notebook includes functionality to perform inference on unseen image and text pairs. Predictions are decoded back into human readable labels, enabling straightforward interpretation of the model outputs.

## Skills Demonstrated

- Multimodal deep learning
- Computer vision and natural language processing integration
- Neural network design with TensorFlow and Keras
- Text preprocessing and tokenisation
- Image feature extraction
- Model evaluation and analysis
- Reproducible machine learning workflows
