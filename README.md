# IMAGE CAPTION GENERATOR USING LSTM

## Research Description
This research focuses on the implementation of the Long Short-Term Memory (LSTM) model for image captioning tasks. The model is designed to generate relevant and accurate text descriptions based on the visual content of images. This approach utilizes a combination of visual feature extraction using Convolutional Neural Network (CNN) models such as VGG16 and the sequence data processing capabilities of LSTM to generate meaningful descriptions.

## Image Feature Extraction
Feature extraction is performed using the VGG16 model, which is one of the popular CNN architectures that has been pre-trained on large image datasets such as ImageNet. The goal of using VGG16 is to transform images into a more abstract and informative numerical representation. This representation allows the visual information in the image to be used in the process of creating a corresponding text description. VGG16 was chosen for its ability to recognize patterns and complex visual features, such as edges, textures, and object shapes, thus supporting the quality of the generated descriptions.

## Dataset
The dataset used is Flicker8k_Dataset, which consists of:
- 8,000 images with text descriptions.
- Each image has 5 descriptions in English, providing multiple perspectives for a single image.
- This dataset covers various categories such as humans, animals, and daily activities.

## Data Preprocessing
- Images are resized according to the needs of the model.
- Text descriptions are processed into tokens that the model can understand.
- The dataset is divided into training and test data to ensure fair evaluation.

## Model and Training Process
The LSTM model is used to process image features that have been extracted by VGG16 and generate descriptions in text form. The model was trained using the Flickr8k dataset, which consists of thousands of images with relevant text descriptions. The training process was carried out for 20 epochs to minimize the loss function and improve the description accuracy.

## Results and Evaluation
The model successfully generated accurate descriptions for simple images with clear objects and activities. Evaluation was conducted using BLEU scores, which showed that the generated descriptions were close to the quality of human descriptions in the dataset. However, there are shortcomings in understanding images that are complex or have a more complicated global context.

## Research Advantages
- Able to generate appropriate and relevant descriptions for images.
- Understand the visual content of images well.
- Practical applications include recommendation systems, image search, and assistance for users with visual disabilities.
- Flexibility in development, allowing modification and improvement of the model architecture.

## Research Weaknesses
- Difficulty understanding complex images or complicated inter-object relations.
- Depends on the quality and diversity of the training dataset.
- Requires high computation and large resources.
- Evaluation of descriptions is subjective, requiring improvement in evaluation metrics.
