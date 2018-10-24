

Hyper-parameter settings
=========================

* HeMLGOP: either weight decay (0.0001) or max-norm constraint (3.0) is used. Input dropout (0.2) and dropout (0.2) after hidden layers. Intermediate BP 300 epochs with learning rate (0.01, 0.001, 0.0001) for every 100 epochs. Block size 40 neurons. Saturation threshold epsilon (1e-4)

* Random Forest: #trees from set {500, 1000, 2000, 4000}, with #features = sqrt(#total features)

* SVM: regularization coefficients selected from set {1e-2, 1e-1, 1, 1e1, 1e2}

* BLS: regularization coefficients in pseudo-inverse (lambda) and ADMM (muy) selected from set {1e-2, 1e-1, 1, 1e1, 1e2}, 500 iterations for ADMM. Incremental step size is 50 neurons and max neuron is 1000 for both feature and enhancement layer. 

* PLN: regularization coefficients in least-square (lambda), output layer optimization (alpha, muy) selected from set {1e-2, 1e-1, 1, 1e1, 1e2}, 500 iterations for ADMM. Incremental step size is 50 neurons and max neuron is 300.

* S-ELM: regularization coefficients selected from set {1e-2, 1e-1, 1, 1e1, 1e2}. Every hidden dimension size is 500 and PCA dimension is maximum 500 

