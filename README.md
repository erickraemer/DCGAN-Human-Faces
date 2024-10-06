# Human Face Image Synthesis by using Deep Convolutional Generative Adversarial Networks

Implemention based on the "Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks" paper by Radford et. al.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1V6AZJMGBqD0-hVZ0nYAgcQ_FUxbYUHrs?usp=sharing)

## Explantation
The architecture consists of two competing neural networks. The generator takes random Gaussian noise as input and synthesizes an image from it. The Discriminator takes an image as input and classifies it as a fake or real image. The discriminator is trained with a random batch of the output of the generator and a separate dataset of real images. The discriminator has to guess which image is synthesized by the generator (fake) and which comes from the dataset (real). The generator tries to fool the discriminator by synthesizing images that are classified as real. The discriminator wants to expose every image synthesized by the generator. After training, the generator has learned how to synthesize images similar to the images in the dataset and can be used to generate new data.

## Results
After training for 5 epochs 25 images are generated.

![download](https://github.com/user-attachments/assets/1c6fdeab-8fda-4426-ab03-0388583fe020)
