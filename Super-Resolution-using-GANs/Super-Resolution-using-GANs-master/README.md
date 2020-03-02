# Super Resolution GANS

SRGANs specialize in improving the resolution of the images.

Deep Convolutional GANs can super-resolve images but the finer texture details are often lost at large upscaling factors. An MSE based objective function can help in content loss minimization but still lead to low fidelity at higher resolutions.

The research paper 1609.04802 discusses Single Image Super Resolution GANs which can infer photo-realistic natural images for 4X upscaling factors.


![alt test](Screenshots/gen1.JPG)

SRGAN achieves this with a perceptual loss function which is a combination of an adversarial loss and a content loss. The new content loss optimizes perceptual similarity instead of pixel space similarity. The deep residual network of SRGAN is able to recover photo-realistic textures from deep downsampled images. A mean-opinion-score (human panel scoring) shows significant gains in perceptual resolution quality with SRGANs.
