# MNIST_digits

As at 2019, it would be cliche to rehash how we classify the digits (0 to 9) from MNIST dataset. However I found that it should be a pre-requisite for those who wants to learn what is machine learning, how important it is to grasp the statistical modeling and how far we have marched towards to AI arena under the guise of neural net coated ML algorithm. 

In this project, I tested all the statistical tools to predict the MNIST Digits. There are a couple of things that we should be aware of. 

### 1. MNIST digit dataset is very clean and pre-processed. 
- each image is 28 x 28 pixels. 
- each image is trimmed in such a way that a digit appear in the middle of the image. 

### 2. K-nearest neighbor (KNN) 
- KNN works well, giving us the accuracy at 87%. 
- If we improve our training models by Gaussian blurring, the accuracy hits to 90%. 

### 3. Naive Bayes (NB) 
- Naive Bayes, which is based on conditional probability, gives 80% accuracy. 
- The model performs poorly than KNN because of the fundamental mechanism of statistics here. 
- While KNN is based upon the pixel value differences between the test image and all the training images, NB is based upon probability of a certain pixel given the digit is 0 or 1 or .... So with the difference in handwriting, it hugely affects the distribution of pixel values and Naive Bayes performs well when there's a normal distribution of data, in this case, pixel values. 

### 4. Tensorflow (TF) 
- I tested a number of tensorflow models. I cited the source. 
- I also tested tensorflow implementation in Google Cloud Platform (GCP) while taking the course from Coursera. 
- Neural networks gives us the accuracy at 98%. 

### 5. Keras
- I implemented Keras with the tensorflow in the backend. 
- The accuracy with neural net is 98%. 
