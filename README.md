# Conditional Very Deep VAE

After reading Rewon Child's paper on very deep variational autoencoders (VDVAE), I felt inspired to see if I could make their model **conditional**. A conditional VAE is similar to a regular VAE but includes a label during the forward pass. This allows the model to pick up on the correlation between a label and its corresponding image features, which ultimately allows for more fine-grained control over the model's generated samples. For instance, once a conditional VAE has been trained on the CIFAR-10 dataset, you can specify that you want "horse" or "airplane" samples from the model's learned distribution.
