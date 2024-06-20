
# Generation of new faces using Variational Auto Encoder
## What is VAE?
Variational Autoencoders (VAEs) are a type of generative model that combine principles from variational inference and deep learning. They consist of an encoder, which maps input data to a probabilistic latent space, and a decoder, which reconstructs the data from this latent representation. Unlike traditional autoencoders that learn a deterministic mapping, VAEs learn the parameters of a probability distribution, typically Gaussian, allowing them to generate new data samples by sampling from the latent space. This probabilistic approach enables VAEs to produce more diverse and realistic outputs, making them powerful for tasks such as image generation, anomaly detection, and data compression.

## This Project
I tried to generate new faces using VAE. Model is trained on the LFW face dataset which contains 13143 samples provided by [JESSICA LI](https://www.kaggle.com/datasets/jessicali9530/lfw-dataset).
Data preprocessing is done with the help of work done by [SERGEI AVERKIEV](https://www.kaggle.com/code/averkij/variational-autoencoder-and-faces-generation#Explore-the-data)
for training batch size is taken 64 and number of epochs 50 and latent dimension of encoded image is 128

## Sample images from Data



## Generated images
Sampling vector of latent dimension from normal distribution and passing it to decoder generates new images.
10 new generated images are shown below.




## Acknowledgements

 - [Jessica li](https://www.kaggle.com/datasets/jessicali9530/lfw-dataset)
 - [SERGEI AVERKIEV](https://www.kaggle.com/code/averkij/variational-autoencoder-and-faces-generation#Explore-the-data)
 - [François Chollet](https://keras.io/examples/generative/vae/)

 - [Swami Punyeshwarananda](https://cs.rkmvu.ac.in/faculty/)