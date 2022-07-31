# Child-Face-Generator
Name - Mainak Singha
Roll - 213310020

## Mentors 
(1) Kaivaly Daga
(2) Manav Doshi

## Seasons of Code (SoC), IIT Bombay

In the project Child Face Generator using GAN of Seasons of Code (SoC), I'm doing the progress with the following,
- Brush up with the Python basics.
- Detailed study about the Git and GitHub repos.
- 3 courses for Deep Learning in Coursera,
  - i) Neural Networks and Deep Learning
  - ii) Improving Deep Neural Networks: Hyperparameter Tuning, Regularization and Optimization
  - Convolutional Neural Networks
- Introduction to GANs
- Interactive Probability
- Watched referral videos in CNN provided by the mentors.

## Convolutional Neural Networks (CNN)
![CNN](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/cnn.jpeg)
Types of layer in a convolutional network :
- Convolution
- Pooling
- Fully Connected

## Generative Adversarial Networks (GAN)
They have generators and discriminators. They play min-max game to each other

### Deep Convolutional Generative Adversarial Networks (DCGAN)
![DCGAN](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/DCGAN.png)

### StyleGAN 
![stylegan](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/stylegan.png)

### CycleGAN
![cyclegan](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/cyclegan.png)

## Loss Functions
**Standard GAN loss function (min-max GAN loss) :**
![ganloss](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/gan_loss.png)

The generator tries to minimize this function while the discriminator tries to maximize it. Looking at it as a min-max game, this formulation of the loss seemed effective.

**Discriminator Loss :**
The discriminator is trained, it classifies both the real data and the fake data from the generator.

![discriminator](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/discriminator_loss.png)

 log(D(x)) refers to the probability that the generator is correctly classifying the real image, and maximizing log(1-D(G(z))) would help it to correctly label the fake image that comes from the generator.

**Generator Loss :**
While the generator is trained, it samples random noise and produces an output from that noise. The output then goes through the discriminator and gets classified as either “Real” or “Fake” based on the ability of the discriminator to tell one from the other.

![generator](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/generator_loss.png)

## Child Face Generator - FamilyGAN
Used [TSKinFace Dataset](http://parnec.nuaa.edu.cn/_upload/tpl/02/db/731/template731/pages/xtan/TSKinFace.html), which includes 1500 pictures of triplets: father, mother, and child.

![latent](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/Latentspace.png)
Scatter plot of faces latent vectors. Blue dots are males, pink are females. Moving with the red arrow makes you more of a male, while moving in a negative direction makes you more of a female.

![familygan](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/FamilyGAN.png)

## Results
**Father**
![father](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/father.png)

**Mother**
![mother](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/mother.png)

**Daughter**
![daughter](https://github.com/Mainak21/Child-Face-Generator-using-GAN/blob/main/Images/daughter.png)

## Conclusion
- FaceApp, Oldify, Baldify, Photo Lab, Face Camera applications work in this similar approach of face manipulations.
- This idea can also be used in different social media applications.
- In this project, I have learnt about CNNs and GANs thoroughly.
- Introduced with DCGAN, StyleGAN and CycleGAN.

## References 
[1]  [Baby Face Generator with CycleGAN](http://cs230.stanford.edu/projects_fall_2019/reports/26256603.pdf), Shihao Li.

[2] [Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](https://arxiv.org/pdf/1511.06434.pdf), Alec Radford & Luke Metz, Soumith Chintala. 

[3] [A Style-Based Generator Architecture for Generative Adversarial Networks](https://arxiv.org/abs/1812.04948), Tero Karras, Samuli Laine, Timo Aila. 

[4] [Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://arxiv.org/pdf/1703.10593.pdf), Jun-Yan Zhu, Taesung Park, Phillip Isola, Alexei A. Efros.

[5] [Image2StyleGAN: How to Embed Images Into the StyleGAN Latent Space?](https://arxiv.org/pdf/1904.03189.pdf), Rameen Abdal, Yipeng Qin, Peter Wonka.

[6] https://github.com/munozalexander/Child-Face-Generation

[7] https://github.com/tg-bomze/BabyGAN





