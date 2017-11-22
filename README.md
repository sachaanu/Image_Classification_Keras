# Image_Classification_Keras

Utilizing Keras as interface to TensorFlow for accessing Google's Inception model based on Deep Convolutional Neural Network.

I will create a model & train it with images of Narendra Modi.

Will test the model on a new image of Modi(but unseen by the model).

An interesting accuracy is achieved as the model was tested with two separate new images.

This project is build by following steps from Siraj Raval's video --- https://youtu.be/QfNvhPx5Px8 for Image Classification using Keras. 

The steps are described as below:

1. Installing Docker -  A great tool that lets you use heavey computational algorithms of CNN based on Tensorflow inside the docker (essentially docker will have all the dependencies for Tf in it).

2. Installing Tensor Flow Docker image in the environment.

3. Creating folder for all images on which the model will be trained -- in tf_files.

4. Downloading the latest inception classifier by --  git pull (so that transfer learning can be applied).

5. Re-training the model with my images:

<img width="564" alt="screen shot 2017-10-09 at 7 13 55 pm" src="https://user-images.githubusercontent.com/26288770/31362364-1bf80688-ad26-11e7-9f8f-0a5e8cb26a61.png">

6. Writing a script to test the new image on the model -- spit out an accuracy score.

7. Make a prediction by running the python script to use the trained model over the test picture.


** Testing with below image gives a score of 46% only:

![test](https://user-images.githubusercontent.com/26288770/31362162-14c57856-ad25-11e7-89e3-e8a629651094.jpg)
<img width="186" alt="screen shot 2017-10-09 at 5 31 07 pm" src="https://user-images.githubusercontent.com/26288770/31362172-22484ae4-ad25-11e7-91ba-f73f512fc1be.png">

** Understandably there is a whole arm & text as-well in the picture -- CNN's extracted & learned the most common features from trained pictures i.e. face shapes, texture, color.

** Using a simpler image for testing where only the facial aspect is the most prominent feature gives a score of 95%.

![test2](https://user-images.githubusercontent.com/26288770/31362259-8463b1d2-ad25-11e7-8449-18391c15254b.jpg)
<img width="201" alt="screen shot 2017-10-09 at 5 30 52 pm" src="https://user-images.githubusercontent.com/26288770/31362278-90aa87f4-ad25-11e7-95a2-de7daf9a7c46.png">
