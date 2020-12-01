# PyTorch_poly_layer
Polynomial layer module for PyTorch

####### DESCRIPTION ########
This is a PyTorch module that builds a polynomial layer with any number of inputs and outputs.

The layer outputs are a polynomial expansion of the inputs, which are the polynomial basis of given order n.



####### HOW TO USE IT #####
To use it, copy the file into the main working directory of your machine learning script and import it as

>> from polynomial import Polynomial

To create the layer

>> poly = Polynomial(i_inputs, j_outputs, uni_degree, int_degree)

where

i_inputs   -> number of inputs of the layer
j_outputs  -> number of outputs of the layer
uni_degree -> max order of independent basis terms (i.e. x_1^2 or x_1^4)
int_degree -> max order of interaction basis terms (i.e. x_1*x_2 or x_1^2*x_2^3)
