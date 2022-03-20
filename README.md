# CNN--glimpse
This project is based on R language and written on Rstudio. I used keras library, tidyr and ggplot2.
First;  we load dataset fashion_mnist. And there are 10 outputs classes and we gave each of them names.
Then showed dataset as train and test and number of pictures. Pictures are 28*28 arrays.
For the model to work properly, these values need to be normalized to the range [0,1]. To perform the conversion we can divide each array by 255.The pixel values across all images range between 0 and 255
The Convolution 2D layers we're going to be using expect a 4 dimensional array (tensor) as input to accommodate the notion of images having channels. In our case, our images are grayscale and therefore only have one channel in the channel dimension. Our data must nonetheless be reshaped to shape (samples, rows, cols, channels). 
After plot images,
We built model with ReLU and softmax. 
ReLU: Rectified Linear Unit function, an additional step on top of Convolution. The reason why the ReLU is used is “to increase the non-linearity”.
The reason we want to increase non-linearity is because images are highly non-linear, that is why we want to break up linearity.
Softmax:In CNN, after the application of the Softmax Function, is to test the reliability of the model using as Loss Function, in order to maximize the performance of our neural network.
Then we compiled model, cause of increase accurate and loss function + optimize it.
