# WGAN

WGAN is proposed to address the vanishing gradient problem in the original GAN loss when the discriminator is way ahead of the generator. One thing to change in WGAN is that the output of the discriminator should be now ‘unbounded’, namely you need to remove the sigmoid function at the output layer. And you need to clip the weights of the discriminator so that their L1 norm is not bigger than c.
