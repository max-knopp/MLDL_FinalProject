# Surface Defect Detection on KolektorSDD2
## A Comparative Study: PCA vs. Convolutional Autoencoder vs. Supervised CNNs

**Group Members:** Anton Gasenzer (185924), Martin Dieselhorst (185897), Max Knopp (185893)

**Research Question:** How does label scarcity influence the choice between supervised and unsupervised learning for surface defect detection?

**Dataset Source:** https://go.vicos.si/kolektorsdd2
Please download the original dataset from this link and change the working directory accordingly.

**Methods:**
1. PCA reconstruction error (unsupervised baseline)
2. Convolutional Autoencoder with hyperparameter sweep (unsupervised)
3. Supervised CNN iterations (v1, v2, v2_tuned) + ResNet50 transfer learning
4. Crossover experiment varying labeled defect count

**Note:** PCA and the CAE are fully unsupervised, so both representation learning and threshold calibration use only normal validation images. The supervised CNNs use labeled validation data for threshold selection (F1-max).
