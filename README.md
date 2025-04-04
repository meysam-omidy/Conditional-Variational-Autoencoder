## Overview

This repository contains the implementation of a Conditional Variational Autoencoder (CVAE) model. CVAEs are an extension of Variational Autoencoders (VAEs) that allow for the generation of data conditioned on certain attributes. This can be particularly useful for tasks where controlling the generated output is desirable, such as attribute-guided image synthesis and semi-supervised learning.

## Features

- **Conditional Generation**: Generate data conditioned on specific attributes.
- **Customizable Architecture**: Easily adjust the architecture to fit different datasets and tasks.
- **Training and Evaluation Scripts**: Includes scripts for training the model and evaluating its performance.
- **Visualization Tools**: Tools to visualize the latent space and generated samples.

## Requirements

- Python 3.x
- PyTorch
- NumPy
- Matplotlib

## About This Implemention

In this implementation, conditional variational autoencoder is used to generate images of MNIST dataset containing images of handwritten digits. Model succeeds in generating images with good overall structure, but it also generates blurry images often happens with this family of models comparing to GANs and Diffusion models. Generated images are sometimes not well structured, which is expected since generation is based on gaussian noise, but it may be possible to alleviate this issue in the future implementations.

## Results

Results on MNIST datasets, generating 50 images, 5 from each digit:
![results](https://github.com/user-attachments/assets/5c1a0ca6-4297-4b8d-a7ea-7f681e301589)


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## References

- Kingma, D. P., & Welling, M. (2013). Auto-Encoding Variational Bayes. arXiv preprint arXiv:1312.6114.
- Sohn, K., Lee, H., & Yan, X. (2015). Learning Structured Output Representation using Deep Conditional Generative Models. Advances in Neural Information Processing Systems, 28.
