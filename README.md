## YOLOv5 for COT Starfish Detection and its predators 
This project utilizes YOLOv5, a state-of-the-art deep learning model, to automatically detect and localize Crown-of-Thorns (COT) Starfish and its predators in underwater images. Aimed at supporting marine conservation, it offers an efficient and accurate solution for identifying these species in coral reef ecosystems, enhancing monitoring and protection efforts

## Dataset 
The dataset for this project consists of 23,501 training images and 3 test images. A preliminary data quality check revealed no missing values (NaN) in the training data, as confirmed by an analysis using isnull().sum(), ensuring a clean and complete dataset for model training and evaluation
* Link to the Dataset: https://www.kaggle.com/competitions/tensorflow-great-barrier-reef

## YOLOv5 Model
The implementation processes 23,501 training images, filtering to 4,919 images with annotations, and splits them into 3,938 training and 981 validation images using an 80/20 split. Key configurations include the YOLOv5 small model (yolov5s), 10 training epochs, SGD optimizer, batch sizes of 4 and 16, and an image size of 256 pixels. The dataset, loaded from /kaggle/input/tensorflow-great-barrier-reef/train_images and /kaggle/input/tensorflow-great-barrier-reef/test_images, is preprocessed to generate YOLO-compatible labels and images, organized into barrier_reef/images and barrier_reef/labels directories. A custom data.yaml file is created to define the dataset structure, specifying one class (cots) for COT Starfish detection, enabling efficient training and validation on this marine conservation task.


## Results

