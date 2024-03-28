# label_noise_regularization
This repository is for our paper entitled "On the impact of several regularization techniques on label noise robustness of self-supervised speaker verification systems" currently under review.

Code of our experiments and trained models will be available upon acceptance of the paper.

# Study of several loss functions

# CAMSAT clustering algorithm
For clustering, we adopt the same CAMSAT clustering approach used in [19] to generate pseudo-labels. CAMSAT is based on augmentation mix and self-augmented training. The goal is to impose invariance to data augmentation on the output predictions of deep models in an end-to-end fashion while maximizing the information-theoretic dependency between samples and their predicted discrete representations (cluster assignments). It provided both state-of-the-art speaker clustering and SV performance. In this paper, we try to investigate several metric learning loss functions to enhance the generalization performance of self-supervised speaker embedding systems and to mitigate the negative effect of heavy noise in the generated pseudo-labels (PLs) used to train these systems. Please refer to [19] for details about CAMSAT architecture and training details.

# The clustering evaluation metrics
Following the commonly used evaluation metrics for clustering, we assess the quality of the generated pseudo-labels using the following three supervised clustering metrics:
