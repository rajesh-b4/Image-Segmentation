# Image-Segmentation

#### Task 1: Dataset Preparation using Python
For this task, I decided to use the COCO dataset. I downloaded the annotations file from the official COCO website and used it to randomly select and download 18,000 images. I then wrote Python code to process these images and generate their corresponding segmentation masks, resizing both the images and masks to 256×256 pixels. These processed images and masks are saved in two separate folders: resized_images and resized_masks. These folders will be used in Task 2 for training a segmentation model. The accompanying Jupyter notebook contains the code for dataset preparation and also includes visualizations of a few image-mask pairs.

#### Task 2: Train an Image Segmentation Model
For this task, I choose the DeepLabV2 model with a ResNet50 backbone. I used the Cross Entropy Loss function for training, with the Adam optimizer and a learning rate of 0.001. Out of the 18,000 processed images, 12,000 were used for training, 3,000 for validation, and the remaining 3,000 for testing. Pixel Accuracy and Intersection over Union (IoU) were used as evaluation metrics. Although the final results were not very satisfactory, I visualized several predictions to assess model performance, which are included in the submitted Jupyter notebook.

