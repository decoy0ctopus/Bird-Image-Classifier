# Bird-Image-Classifier
An image classifier project to practice setting up a input pipeline, training a deep learning model, comparing performance between 6 different CNN arhictectures, using Flask API to a simple frontend and containerising the whole project using Docker.

Thi was done using the tutorial provided by Patrick Brus https://towardsdatascience.com/full-deep-learning-portfolio-project-part-1-78df161214aa

# clean_dataset.ipynb

The open source birds species dataset from Kaggle is used in this notebook (source: https://www.kaggle.com/gpiosenka/100-bird-species). However, I first created a clean version of the Birds_Species.csv file, because the original file is missing some classes (only 285 of 300 classes were present -> see the Make_Clean_Dataset.ipynb notebook). 

# model_train.ipynb

Creating a reusable training pipeline to:

1. Check data distribution.
2. Create tensorflow input pipeline with normalization.
3. Compare different state-of-the-art CNN architectures to find best suited.
4. Check different images sizes on winning cnn.
5. Check oversampling vs. imblanced. 
6. Apply Bayesian Hyperparameter Search to find best hyperparameters.
7. Train final model.
8. Test the final model on the hold-out test set.

# app.py

Flask app rendering simple html template, allowing users to input an image, calling the model, then returning a label and a confidence percentage.


