
# Generation of new faces using Variational Auto Encoder
## What is VAE?
Variational Autoencoders (VAEs) are a type of generative model that combine principles from variational inference and deep learning. They consist of an encoder, which maps input data to a probabilistic latent space, and a decoder, which reconstructs the data from this latent representation. Unlike traditional autoencoders that learn a deterministic mapping, VAEs learn the parameters of a probability distribution, typically Gaussian, allowing them to generate new data samples by sampling from the latent space. This probabilistic approach enables VAEs to produce more diverse and realistic outputs, making them powerful for tasks such as image generation, anomaly detection, and data compression.

## This Project
I tried to generate new faces using VAE. Model is trained on the LFW face dataset which contains 13143 samples provided by [JESSICA LI](https://www.kaggle.com/datasets/jessicali9530/lfw-dataset).
Data preprocessing is done with the help of work done by [SERGEI AVERKIEV](https://www.kaggle.com/code/averkij/variational-autoencoder-and-faces-generation#Explore-the-data). Sergei implemented VAE using Pytorch on this dataset. but in my code implementaion is done using keras.
for training batch size is taken 64 and number of epochs 50 and latent dimension of encoded image is 128. Use **Google colab** to run the code


## Sample images from Data

![download](https://github.com/SameerSri72/Variational_auto_encoder/assets/142829103/d4965c4f-b6ad-4247-ba84-c03073b33a59)


## Generated images
Sampling vector of latent dimension from normal distribution and passing it to decoder generates new images (which are not present in training data).
10 new generated images are shown below.
![download (1)](https://github.com/SameerSri72/Variational_auto_encoder/assets/142829103/77f8efdc-f868-4c76-8ee4-dd22666cacc8)




## Acknowledgements

 - [Jessica li](https://www.kaggle.com/datasets/jessicali9530/lfw-dataset)
 - [SERGEI AVERKIEV](https://www.kaggle.com/code/averkij/variational-autoencoder-and-faces-generation#Explore-the-data)
 - [François Chollet](https://keras.io/examples/generative/vae/)

 - [Swami Punyeshwarananda](https://cs.rkmvu.ac.in/faculty/)
