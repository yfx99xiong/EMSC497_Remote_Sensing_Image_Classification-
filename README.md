# Remote_Sensing_Image_Classification-

Perform image classification on a hyperspectral image, and assign a class label (land cover) to each pixel.

The image file (“data.tif”) is a hyperspectral airborne image acquired on November 17, 2008 by AISA-Eagle (AE) Hyperspectral Imager of CALMIT (Center for Advanced Land Management Information Technologies), University of Nebraska-Lincoln. The image covers part of the coast near Corpus Christi, Texas. It includes 63 narrow bands in the Visible and Near Infrared (VNIR) spectral range from 400 to 970 nm wavelength at a spatial resolution of 1 and 2 meters. The pixel value of each band is the surface reflectance multiplied by 10000.

The “training.csv” includes training data, each record has 65 attributes, including surface reflectance values (multiplied by 10000) of the 63 bands, land cover class (1 for Construction, 2 for Dock, 3 for Water, 4 for Building roof, 5 for Grass, 6 for Wetland), and classlabel. In this context, a classifier is a model that predicts land cover class from the surface reflectance values of those 63 bands.

Perform and document the following tasks in your notebook:

Use training.csv to train different classifiers you have learned above, evaluate the performance of each classifier, and discuss the difference of the classification performance.
Use k-fold cross validation method to tune the hyperparameter ‘k’ for the k nearest neighbor classifier, use GridSearchCV to tune the hyperparameters of ‘max_depth’ and ‘min_sample_leaf’ for the decision tree method, plot the classification measure (you choose a proper metric, such as kappa coefficient) varied with different hyperparameters for both training set and test set.
Use your trained model and best hyperparameter to classify the whole image (data.tif), which means that you need to assign a class label to each pixel. Plot the original image and the classification results of different classifiers.
Apply principal component analysis to X (the surface reflectance values of the 63 bands). Choose a subset of the principal components to perform classification tasks (kNN, decision tree, naïve bayes, SVM), plot the classification results, and discuss the advantages/disadvantages of using principal components to do image classification.

Note: This is a course lab for EMSC497 Environmental Data Analysis 
