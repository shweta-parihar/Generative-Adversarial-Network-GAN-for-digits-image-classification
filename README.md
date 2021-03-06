# Generative-Adversarial-Network-GAN-for-digits-image-classification

Generative modeling is an unsupervised learning task in machine learning that involves automatically discovering and learning the regularities or patterns in input data in such a way that the model can be used to generate or output new examples that plausibly could have been drawn from the original dataset.  

GANs are a clever way of training a generative model by framing the problem as a supervised learning problem with two sub-models: the generator model that we train to generate new examples that look real, and the discriminator model that tries to classify examples as either real (from the domain) or fake (generated). The two models are trained together in a zero-sum game, ie. adversarial, until the discriminator model is fooled about half the time, meaning the generator model is generating plausible examples.
## About the problem and methodology
The most notable application is image-to-image translation tasks. Here also, we train the model to create digits image giving input as mnist dataset which has database of handwritten digits from 0 to 9. The generator tries to create images of digits that look as close as possible to the original images in the mnist dataset and the discriminator tries to identify the images as fake. This leads to generator generating more convincing images that look real.  

The generator and discriminator contains stacked convolutional layers, batch normalization and dropout layers. After about 50 epochs, we get digit images that look real as if they have come from original dataset even though they are created by the model.
