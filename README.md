# FakeVSReal-Detection
Image detection model

A model used to detect whether an image is real or AI-generated.
The data set I have selected is the CIFake: Real and AI Synthetic generated images, which I took from Kaggle.
I have split the data set into 3 folders:
Cfake: contains training data of about 99688 images in total, which has 2 folders of real and fake images.
Train: 296 images used for testing
Valid: 296 images which can be used for validation to check whether the model works.

The architecture I am using for my model is the Densenet 121 model.
I have chosen this architecture for various reasons
This architecture has 121 layers so it is capable of capturing small details to distinguish between real and fake images.
Densenet121 is known for its feature extraction hence I thought it would be a good fit for this problem statement.
It can work well with large datasets.

This pre-trained model will be combined with a sequential model for binary classification.

Set-Up: 
Downloaded the necessary libraries. (Keras, TensorFlow, numpy, pandas,cv2,etc)
Download the dataset
Change the paths in the code according to your setup.
Run the model.

To test images:
Copy the path of the image from the ‘valid’ folder. Then paste the path in the input and hit Enter.
It will print the prediction.

If the image is real it will print ‘Real’
If the image is AI generated it will print ‘Fake’
