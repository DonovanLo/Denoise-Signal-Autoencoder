# Denoise-Signal-Autoencoder

This tutorial is introductory to denoising signal with Autoencoders. We will mainly be focused on the application of autoencoder and will not go in the math specifics. We hope by the end of the tutorial you have a good idea what an autoencoder is, and how it can be used towards denoising signal.  

### Table of Contents:
* [What are Autoencoders ?](#definition)
* [Setup](#setup)
* [Vanilla Autoencoder](#v_ae)
* [Multilayer Autoencoder](#m_ae)
    * [Build/Train Multilayer Autoencoder](#build_mae)
    * [Acoustic Data](#acoustic_data)
* [Convolutional Autoencoder](#conv_ae)
* [Summary](#summary)
* [Next Steps](#next_steps)
* [Reference](#ref)

## What are Autoencoders ? <a class="anchor" id="definition"></a>

Autoencoder is an [Artificial Neural Network (ANN)](https://en.wikipedia.org/wiki/Artificial_neural_network) trained to learn an encoded representation of an input data. This unsupervised mechanism does not require labels, and instead maps the recognized patterns to a set of compressed features, at which can then be converted to the same or a different presentation. 

Autoencoder is made up two neural networks. The first half is called the encoder and the second half is called the decoder. Both neural networks are made up of single or multiple hidden layers with [activation functions](https://en.wikipedia.org/wiki/Activation_function). The encoder and decoder are normally symmetrical in the number of hidden layers to ensure that the output's dimension retains the input's shape. 
