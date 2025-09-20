## GANs
Generative Adversarial Networks (GAN) were introduced by Ian Goodfellow in Generative Adversarial Networks, Goodfellow, 2014.<br>
<br>
The GAN consists of two networks namely:<br>
1. The generator G that produces fake samples.<br>
2. The discriminator D that that receives samples from both G and the dataset.<br>
During Training the two networks have competing goals. The generator tries to fool the discriminator by outputting values that resemble real data and the discriminator tries to become better at distinguishing between the real and fake data.
<br>
Mathematically, this means that the Generator's weights are optimized to maximize the probability that fake data is classified as belonging to the real data. The discriminators's weights are optimized to maximize the probability that the real input data is classified as real while minimizing the probability of fake input data being classified as real.
<br>
Optimality is reached when the generator produces an output that the disciminator cannot concretely label as real or fake and this, happens when either of the networks cannot improve anymore.
<br>
<br>

![Gan-Page-2](https://github.com/user-attachments/assets/7b5d012c-c214-422c-b18e-bf1872877229)
<br>

### Loss Function for GANs
<img width="739" height="49" alt="image" src="https://github.com/user-attachments/assets/9ad09c4b-eed9-49f3-9a02-5364642f5bbe" />
<br>
<br>
The first part of the above equation reflects the log probability of the discriminator predicting that the input sample is genuine and the second half reflects the probability of the Discriminator predicting that the Generator's output is not genuine.
