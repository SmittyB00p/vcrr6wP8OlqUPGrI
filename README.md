# MonReader

## About


'Flip' image
![flip training image](images/training/flip/0001_000000010.jpg?raw=true)


'Notflip' image
![notflip training image](images/training/notflip/0001_00000001.jpg?raw=true)

## Exploratory Data Analysis
The images in this dataset were fairly distributed, with the 'flip' images equalling ~48% of the 2989 total images and the 'notflip' images roughly equalling 52%.

All of the images had a size of 1920 x 1080 x 3. The last number indicating that they are colored images.

## Modeling
TNet, a custom Convolutional Neural Network (CNN) was implemented and tested upon the images of the dataset with over 65% accuracy.

Pre-trained ResNet18 and VGG16 models were used to compare to TNet.
* ResNet18 accuracy = 88% training and 93% validation
* VGG16 accuracy = 58% training and 67% validation

Going forward, the Resnet18 model will be used

### Text Extraction
coming soon...

## Setup
To run this notebook make sure to: 
* use a Python 3.9.13 kernel
* download the requirements.txt file by running in the console `pip install -r requirements.txt`
* uncomment the first code cell that will allow you to install a few of the necessary packages
* after the TNet CNN architecture block make sure the `SEED` is set to `14425870739644852099` for reproducibility