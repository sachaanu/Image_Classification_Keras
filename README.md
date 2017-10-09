# Image_Classification_Keras

Utilizing TensorFlow & Keras capability based on Convolutional Neural Network model called Inception.
I will create a model with training images of Narendra Modi & a new image will be given to the model to identify as Modi.
An accuracy achieved is intersting as the model was tested with two separate new images.

This project is build by following steps from Siraj Raval's video --- https://youtu.be/QfNvhPx5Px8 for Image Classification using Keras. 

The steps are described as below:

1. Installing Docker -  A great tool that lets you use heavey computational algorithms of CNN based on Tensorflow iside the docker (essentially docker will have all the dependencies for Tf in it).

2. Installing Tensor Flow Docker image in the environment.

3. Creating folder for all images on which the model will be trained -- in tf_files.

4. Downloading the latest inception classifier by --  git pull (so that transfer learning can be applied).

5. Retraining the model with images.

6. Writing a script to test the new image versus the model.

7. Make a prediction by running the python script to use the trained model over the test picture.
