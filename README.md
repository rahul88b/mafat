# mafat

Welcome to COFGA (Classification Of Fine-Grained Features In Aerial Images) dataset, 
the dataset of 'MAFAT Challenge - fine-grained classification of objects from aerial imagery'. 

This folder contains the following:
1. 'training imagery' - a folder containing 1,663 tiff and jpeg images.
2. 'train.csv' - A CSV file contining 11,617 tagged vehicles. 
Each object is represented by a tag ID, an ID of the image in which it is located, and a bounding polygon, which is a set of 4 x-y (pixel) coordinates. 
Additionally, each object in the training set includes fine-grained classification data: class, subclass, features and color. 
Please note that features are represented as boolean fields while “-1” represent a non-viable option.  
These files will enable you to start building and practicing your model.

The data folder also contains:
3. 'test imagery' - a folder containing 2,553 tiff and jpeg images.
4. 'test.csv' - A CSV file containing 11,879 tagged vehicles.
This file includes objects in the same form as in the training set (tag ID, image ID and a bounding polygon), but without the classification data.
These are the test files, according to which your code will be evaluated.


answer.csv - It is the final csv file which is to be submitted.

Each folder general_class, sub_class & color contains the code for classifying each respective class. Uptill now i have used ResNet50 architecture for each class. Further for classes on which accuracy is not good, i'll try other architecture accordingly.

This repo doesn't contain training and test images.
