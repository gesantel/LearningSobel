# Learning Sobel

See Substack post [here](https://georgesantellano.substack.com/publish/post/181097416).

The goal of this project was to see how well different architectures learn the size k Sobel filter for k = 3,5,7,9. We add gaussian noise w/ std deviations sigma =  0,.1, .5, .2. We construct phase diagrams for our architectures on the parameter spaces for k and noise. 

# Data processing

For my dataset I used the MNIST dataset of handwritten digits. For each image x I convolved with the Sobel kernel and added Gaussian noise. This was systematically varied. These transformed images were our “labels” y, and we trained each model on the image and label pairs (x,y) for an image-to-image regression task.

# Model and Fitting

For this project, the architectures I train are a 1 layer Transformer, a 1 layer CNN (convolutional neural network), and a 1 layer MLP (perceptron with no activation function). 


