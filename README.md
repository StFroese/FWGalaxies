# FWGalaxies
Fun with galaxies

## The data
[DECals dataset](https://astronn.readthedocs.io/en/stable/galaxy10.html) contains 17736 256x256 pixels colored galaxy images (g, r and z band) separated in 10 classes.

## The task
1. Find the galaxy that is most similar to this theoretical image of the milky way:
<img src="https://www.nasa.gov/images/content/188404main_hurt_Milky_Way_2005-590_lg.jpg" width="300">

2. Generate new galaxies that look like the milky way

## The approach
1. Use a Vision Transformer ([ViT](https://arxiv.org/pdf/2010.11929.pdf), [same task](https://arxiv.org/pdf/2110.01024.pdf)) to learn a latent representation of the dataset and compare all latent vectors to the latent vector of the milky way image.
2. Use the trained encoder-decoder structure to train a [stable diffusion network](https://arxiv.org/pdf/2112.10752.pdf) to generate new milky ways
