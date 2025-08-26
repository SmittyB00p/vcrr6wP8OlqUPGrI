# MonReader

## About


'Flip' image
<!-- ![flip training image](images/training/flip/0001_000000010.jpg?raw=true) -->
<img src="images/training/flip/0001_000000010.jpg?raw=true" width="50%" height="auto">


'Notflip' image
<!-- ![notflip training image](images/training/flip/0001_000000010.jpg?raw=true) -->
<img src="images/training/notflip/0001_000000001.jpg?raw=true" width="50%" height="auto">

## Exploratory Data Analysis
The images in this dataset were fairly distributed, with the 'flip' images equalling ~48% of the 2989 total images and the 'notflip' images roughly equalling 52%.

All of the images had a size of 1920 x 1080 x 3. The last number indicating that they are colored images.

## Modeling
TNet, a custom Convolutional Neural Network (CNN) was implemented and tested upon the images of the dataset with over 65% accuracy.

Pre-trained ResNet18 and VGG16 models were used to compare to TNet.
* ResNet18 accuracy = 88% training and 93% validation
* VGG16 accuracy = 58% training and 67% validation

More experimentation will be needed due to the fact that the pre-trained models are possibly overfitting, but for the time present the VGG16 model looks the best.

### Text Extraction
Using Google's Gemini model we will be able to extract text from uploaded images.

Please look at the text_extraction notebook for further work.

### Audio Generation
Using two new text-to-speech (TTS) models - DIA and Sesame - we will generate human like audio with the extracted text.

Please look at the dia_audio or sesame_audio notebook for further work.

## Setup
To run this notebook make sure to: 
* use a Python 3.9.13 or later kernel
* download the requirements.txt file by running in the console `pip install -r requirements.txt`
* after the TNet CNN architecture block make sure the `SEED` is set to `14425870739644852099` for reproducibility