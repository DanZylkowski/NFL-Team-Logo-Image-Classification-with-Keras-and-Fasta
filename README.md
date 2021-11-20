# NFL-Team-Logo-Image-Classification-with-Keras-and-Fastai
Image classification is an exciting subclass of computer vision. Important uses cases for image classification include identifying cancer in X-rays or allowing self-driving cars to identify objects in the road. For this project the an example use case would be for online retailers to identify the name of the NFL team based on a picture of a logo. This project aims to classify the images of the logos of 31 of the 32 NFL teams. The Washington Football Team is not being included in this analysis since the team has no current logo and will not have a new logo until 2022. 

The project has three parts: data collection and cleaning, training a Convolutional Neural Network (CNN) from scratch in [Keras](https://keras.io/), and finally building a model on top of the ResNet50 model using the [fastai](https://www.fast.ai/) library. The goal of the project is to create a CNN model that will classify NFL team logo images with high accuracy. While the focus of the project is to classify NFL team logos, the project could be used as a template for creating CNN models that can classify other types of images with only slight modifications to the data collection and modeling steps.

The images used in the project can be downloaded from [google drive](https://drive.google.com/drive/folders/1aM-0xHmFzcPjx1pa0hImghVUhezYLkfa).

The final model that achieved 98.8% accuracy can also be downloaded [google drive](https://drive.google.com/file/d/1-depiOTcFrDxd2sOKo-RIsRfU6iCgjA9/view?usp=sharing)

---
### An important note on image curation.

The final stage of the image collection process is to manually review the images in each folder. I needed to make sure that there are no mislabeled images, and no repeated images of the same size. I found many duplicate sized images and images that were misclassified by the bing image search engine. I used domain knowledge of the team logos to ensure that all images were correctly labeled prior to model training. The curation of the images was by far the most time consuming step of the project, but was also the most critical. Failing to remove incorrectly labeled images would cause the model to propogate the misclassification, and would limit the accuracy of any model that is built using the data.
