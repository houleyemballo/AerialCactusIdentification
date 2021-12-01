# Aerial Cactus Identification

Overview


Business and Data Understanding



Stakeholder Audience


Modeling

CNN

Initial Exploration:

A separate validation set of images was created due to the small size of the provided validation set (16 images). The folder of pneumonia verified x-ray images was just under four times larger than the folder for healthy x-rays and will be dealt with by transforming the normal images to increase the number of them in future model iterations. Due to computational limitations, images were reduced from an average height/width of 968 x 1320 pixels to 255 x 255 pixels. A test train split was used to separate image data into test, train, and validation (holdout) folders. training_image_count

Baseline Model:

The baseline model was a simple CNN consisting of one flatten and two dense layers. The baseline model resulted in a test loss of 0.6862 and a test accuracy of 0.6259.

Final Model:

The final model (Model 5) was a more complex CNN made up of nine layers. The CNN contained Dense (3), Conv2D (2), Flatten (1), Dropout (1), and Average Pooling (2) layers. The model had a precision score of 0.8026, recall of 0.9616, accuracy at 0.8280, and a loss of 0.3594.

Model Results

Parameter Tuning:

Made adjustments to prevent overfitting using Early Stopping and Dropout. Made sure all aspects of our model were set up to work in a binary classification model.

Recommendations:


Conclusion



Future Work:

