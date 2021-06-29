# project-
# Project Name - Image classificatrion using CIFAR - 10 Dataset in Tensorflow
In this project I have used following liberaries
1 Tensorflow
2 Numpy
3 Matplotlib.pyplot for visualizing the data and to see the accuracy of our model
Than i have used tensorflow.keras.layes and tensorflow.keras.model for imorting batch normalization, model input, conv2d, Dense, Flatten, Dropout,GlobalMaxPooling2D, MaxPooling2D,a and model.
I have directly load the dataset as we already know that CIFAR - 10 dataset is already present in the keras so we dont need to download it from any other website
after that the dataset was distributed for the training and testing after distributing we got to know that the size of images is 32x32.
In the dataset tere are total 60000 images in which 50000 are for training and the rest 10000 for testing.
as we know now that size of the images is 32x32 so we reduse it by dividing from 255 to reduce it's range from 1 to 256 to range from 0 to 1 and then i have use the flatten funtion so that the simple words will be in the form of rows.
After all these i have visualise the dataset using the subplots so that i can see few  images of the dataset
Now i have made the model ussing CNN It includes the convolutional layer in which there is conv2Dlayer,pooling and normalization method.Than we will pass it to dense layer than the another dense layer which is our last layer of the model. here we will use relu as activation function and in final layer we will use softmax layer.
after this model was compiled using model.compile in which I have used  following parameters - 
. matrices for accuracy 
. sparse categorical crossentropy as loss fuction
. adam optimizer
And than i have fit the model 2 times first normally and than after the data augmentation so than ourn pridiction will be accurate .
and now we will start pridicting the data we will do following steps -
1 map the labels
2 select the image 
3 display the image
4 load the image in array
5 passing to network for pridiction and saving the label
6 load the orignal image
7 and than display the output
Now finally we will save the model using model.save() fuction.
