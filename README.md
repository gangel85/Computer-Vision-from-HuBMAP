# Computer Vision from HuBMAP
Keggle competition: non sclerotic glomeruli in kidney tissue images

I have worked on this code for about one week, in order to get more experience on computer vision, unfortunately due to my current work load I wasn't able to spend more time in improving my model and the preparation of the data sample. However I have finally achieved a 92 percent score in identifying glomeruli.

Here a quick summary of what I did:

Each image provided in the training data set is of high definition and includes many glomeruli.
I have then chopped each image in sub-images so to increase the data sample and keep one to two glomeruli in each training sample. The image has been resize of a factor 4, this has been common in many other notebooks providing a good compromise between sample size and resolution.

I have used CV and Augmentation packages to enhance the images tweaking the contrast, brightness and sharpeness. 

I have trained a Neural Network using Resnet model (pretrained weights so to speed up the process). The network has been modelled studying what other Keggle users have done in previous computer visions competisions. 

I have tweeked the parameters in order to find the best score.

Despite the time contraints I achieved a resasonable good score.
