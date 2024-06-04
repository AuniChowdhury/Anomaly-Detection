# Anomaly-Detection

This notebook is a rough implementation for anomaly detection using variational autoencoder.

# Dataset
https://www.mvtec.com/company/research/datasets/mvtec-ad
Carpet Images



#Implementation
The implementation uses alibi_detect library.It trains a variational autoencoder model to detect anomalies in carpet images of the mvtec dataset. The model is trained only on the good (without anomaly) samples. When an input image is reconstructed using the trained VAE model, the region where reconstruction loss is highest, meaning where the difference between the reconstructed image and the actual image is highest, that gets identified as an anomaly. The encoder-decoder architecture used in this implementation is very simple. Even this simple architecture yields good enough results. 


