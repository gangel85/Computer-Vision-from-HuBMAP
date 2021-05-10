# Computer Vision from HuBMAP
Keggle competition: non sclerotic glomeruli in kidney tissue images

I have worked on this code for about one week, unfortunately due to my current work load (PhD defense coming and teaching two classes) I wasn't able to spend more time in improving my model and find better way to enhance the training set. Nevertheless, the CNN was cable of identify glomeruli at 91% using the public test sample. 

Here a quick summary of what I did:

Each image provided in the training data set is of high definition and includes many glomeruli.
I have then chopped each image in sub-images so to increase the data sample and keep one to two glomeruli in each training sample. The image has been resize of a factor 4, this has been common in many other notebooks providing a good compromise between sample size and resolution.

I have used OpenCV and Albumentations packages to enhance the images tweaking the contrast, brightness, sharpeness, and expanding the training sample with variations.

I have trained a Convolutional Neural Network using Resnet model. The network has been modelled studying what other Keggle users have done in previous computer visions competitions, using several hidden layers with ReLU as activation function for all the layers. 

I have tweeked the parameters in order to find the best score, but I didn't have time to play with the hidden layers as much as I wanted. Despite the time contraints I achieved a resasonable good score.
