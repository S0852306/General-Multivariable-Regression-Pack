# Function Approximation Neural Networks
**Neural networks for multiavariable function approximation & regression.**
# Introduction
* Neural networks possess the property of universal approximation, which means that given enough parameters, a neural net can approximate any multi-variable continuous function to any desired level of accuracy.
* Many built-in functions in MATLAB only provide functionality for curve fitting (1D) or surface fitting (2D). In contrast, neural networks can handle more general and higher-dimensional fitting problems. 
* Compared to the fitting errors of built-in functions, neural networks can provide astonishing accuracy when it comes to approximating highly complex functions.
* More Info : https://tinyurl.com/wre9r5uk 
(MATLAB File Exchange)
# Types of Neural Nets
 1. Ordinary MultiLayer Perceptron 
 2. Residual Neural Network
# Optimization Solvers
 1. Stochastic Gradient Descents (SGD)
 2. Stochastic Gradient Descents with Momentum (SGDM)
 3. Adaptive Momentum Estimation (ADAM)
 4. Root Mean Square Propagation (RMSprop)
 5. Broyden-Fletcher-Goldfarb-Shanno Method (BFGS)
# User Guide
"GeneralGuide.mlx" provide a a general workflow and detailed instructions on how to configure the solver.
If you are not familiar with numerical optimization/deep learning, you can also use the following command to automatically configure the solver.
```
% Network Structure Set Up
LayerStruct=[InputDimension,10,10,10,OutputDimension];
NN=Initialization(LayerStruct);
% Solver Set Up
option.MaxIteration=500;
NN=OptimizationSolver(data,label,NN,option);
```
![image](https://github.com/s0422038/Function-Approximation-Neural-Networks/assets/111946393/d9f411dc-158c-4dfb-bbca-08b46453df77)

# Reference
 1. Numerical Optimization, Nocedal & Wright.
 2. Practical Quasi-Newton Methods for Training Deep Neural Networks, Goldfarb, et al.
 3. Kronecker-factored Quasi-Newton Methods for Deep Learning, Yi Ren, et al.
