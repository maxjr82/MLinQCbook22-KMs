### Supplementary material for the book "Quantum Chemistry in the Age of Machine Learning"

# Kernel Methods (chapter 22)

This repository contains a practical illustration of the kernel matrix definition (see introduction 
of the book chapter) and a hands-on tutorial about kernel principal component analysis (KPCA), all
designed in a jupyter notebook environment using python3. 

- Introduction to kernel matrix (intro_kernel_similarity.ipynb):

In this introductory notebook, it is shown how to build a kernel matrix from scratch for a "toy" 
dataset of small molecules. Then, this kernel matrix is used to illustrate how to train a non-linear 
machine learning model (regression or classification) and make predictions for a new data point. 

- Case study for Fitting with kernel ridge regression (fitting_with_KRR.ipynb):

This notebook provides an implementation of KRR (Kernel Ridge Rergression) from scratch with numpy library and the corresponding formula. 
After the implementation, this notebook will use this KRR class to fit $H_2$ FCI data with Linear kernel and Guassian kernel, then plot it to show the result. You can also change the hyperparameter by yourself to see how the result changes with different hyperparameter.

- Case study for unsupervised learning using kernels (case_study_kpca.ipynb):

This notebook provides an implementation of the **kernel PCA (KPCA)** algorithm from scratch using the
popular **radial basis function (RBF)** kernel as an example. The KPCA algorithm is then applied to a 
real quantum chemical dataset of small molecules covering the compositional and configurational space
of fragmentation reactions involving interhalogen compounds. After training the KPCA model, the two
most important components of the non-linear projections are represented in a 2D scatter plot to 
illustrate how the KPCA method can be used to navigate in the "chemical space" and get new insights
on the relationship between the data distribution and specific molecular properties used as color code 
in the scatter plot.

## Requirements

To run the notebooks locally, the following python libraries will be required:

- Math and data processing libraries:

  - pandas
  - numpy
  - scipy
  - scikit-learn

- Graphical libraries:

  - matplotlib
  - plotly

- Specialized packages:

  - QML (to create molecular representations)
  - py3Dmol (for molecular visualization)

The tutorial can be also run in the cloud using the google colab environment.
