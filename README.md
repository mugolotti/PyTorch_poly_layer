# PyTorch Polynomial Layer
Polynomial layer module for PyTorch (** GitHub page under construction **)

## DESCRIPTION 
This is a PyTorch module that builds a polynomial layer with any number of inputs and outputs.\
This particular layer introduces an "intermediate" layer (called *polynomial*) in between inputs and outputs, which consists of a set of polynomial basis of the inputs as shown in the figure. Then, the intermediate layer is linearly connected to the output layer.

<img src="/images/poly_layer_diagram.png" width="500">

The number of neurons in the intermediate polynomial layer is based on the user-defined order of the independent and interaction terms.

This polynomial layer can be used either as a standalone model or used in more complex models, thus connecting it with other types of layers.

## HOW TO USE IT
To use it, copy the file into the main working directory of your machine learning script and import it as

>> from polynomial import Polynomial

To create the layer

>> poly = Polynomial(i_inputs, j_outputs, uni_degree, int_degree)

where:
* i_inputs   -> number of inputs of the layer
* j_outputs  -> number of outputs of the layer
* uni_degree -> max order of independent basis terms (i.e. <img src="https://render.githubusercontent.com/render/math?math=x_{1}^{2}"> or <img src="https://render.githubusercontent.com/render/math?math=x_{2}^{4}">)
* int_degree -> max order of interaction basis terms (i.e.  <img src="https://render.githubusercontent.com/render/math?math=x_1 \cdot x_2"> or <img src="https://render.githubusercontent.com/render/math?math=x_1^2 \cdot x_2^3">)
