# **Colourisation of black and white photos**

### **Haaris Hayat**

## **Introduction**
In this project I explore the use of several ML models utilising CNNs and GANs to convert old black and white photos to colour. The project report pdf ('Colourisation_Haaris_Hayat.pdf') contains details of the problem space as well as a closer look at the models used.

## **How to Run**
The colorizer models can be run from the notebook, which walks users through the entire process.

For the DeOldify model, the pre-trained weights need to be downloaded first (unless they are already in the models folder). The weights for the two models can be found here:
Artistic: https://data.deepai.org/deoldify/ColorizeArtistic_gen.pth

Stable: https://www.dropbox.com/s/usf7uifrctqw9rl/ColorizeStable_gen.pth?dl=0

These weights need to be saved in the models folder before the models are run. 

Note that you can download the weights for any one or both models as they are run independently in the notebook.

Apart from this, the notebook can be run and contains step-by-step instructions.

## **File Contents**
### **Code**
The main file in this project is the Jupyter Notebook file called 'colourisation.ipynb'. This contains all of
the code used to generate the results in the project report along with instructions.

### **Models**
The models folder contains the pre-trained weights for the DeOldify model. These can be downloaded from:
Artistic: https://data.deepai.org/deoldify/ColorizeArtistic_gen.pth

Stable: https://www.dropbox.com/s/usf7uifrctqw9rl/ColorizeStable_gen.pth?dl=0

### **Datasets**
There are two folders that contain the datasets used:
1. test_images - this contains 20 colour images used for testing of the colourisation (around 33mb)
2. old_images - this contains the old images that will be colourised (around 1.5mb)

### **Outputs**
Outputs of the code are stored in several folders:
1. test_images_bw - After the colour images in test_images are converted to greyscale, they are stored here
2. out_colorizer - This contains the outputs from the Colorizer model
3. out_deoldify - This contains the outputs from the DeOldify models. There are two sub-folders: 
   1. Artistic - Contains results from the Artistic DeOldify model
   2. Stable - Contains results from the Stable DeOldify model
   
### **DeOldify**
The deoldify folder and environment.yml are included since support for the DeOldify package appears to have ended and can no longer be installed in 2023!

### **Requirements**
The requirements file contains the list of packages that need to be installed. This is used by the notebook automatically.


