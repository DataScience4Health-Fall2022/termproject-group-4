## Group 4: Derm Classification 
### Members: Gokul Srinivasan, Avani Kuthe, William Chen, and Xingjian Diao
### Dataset: HAM100000

### Objective: 
Our objective here is two-fold. 
* First, train a CNN that is capable of classifying a wide range of dermatological conditions. 
* Second, train a GAN to improve performance of classifier by synthetic production of underrepresented samples. 

### Repo Structure Description
* Note that all of the classifiers used in this study are stored in the `Models` folder, stratified by their architecture. 
* GAN models are trained in the `GANs` folder. There are two GANs here, one that produces images of size 64 x 64, and the other that produces images of size 128 x 128. 
* Scripts used to generate visuals are stored in the `Visuals` folder. 
* Lastly, augmentation scripts are stored in the `Augmentation` folder. 
### Usage Notes
* Please note that if you attempt to run some of these files, you will encounter errors due to the fact differences in file structures/directories. To run these files, it is first necessary to install the HAM10000 dataset, and appropriately change  references to this dataset in code. 
* Furthermore, note that some of these files have been modified since writing up our study. 
* For example, in this [file](https://github.com/DataScience4Health-Fall2022/termproject-group-4/blob/main/Models/ResNet/DermClassifierDoubleAugmentation.ipynb), the ResNet model used is ResNet50, which we were further experimenting with. Switch this model to ResNet101 to match the methods described in the study. 
* Additionally, our testing was done in colab with access to their GPUs, and even still training the ResNet101 model in the least strenous condition for 35 epochs takes around ~ 60 minutes. 
