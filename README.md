# 2D-time-dependent-heat-equation-using-PINNs-tf2-
A Physics-Informed Neural Network to solve 2D time-dependent heat equations.


Inspired by [this](https://github.com/314arhaam/heat-pinn), Which solved a steady-state 2D heat equation using a Physics-Informed Neural Network. In this project, time is introduced. 

The heat equation is a fundamental partial differential equation that describes how heat diffuses through a given region over time. It is widely used in various fields such as physics, engineering, and mathematics to model the distribution of temperature in a given region.

## Governing Equation

The heat equation in two dimension is given by:

$\[ \frac{\partial u}{\partial t} = \alpha \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} \right) \]$

where:
- \( u(x, t) \) is the temperature distribution function, dependent on position \( x \) and time \( t \),
- \( \alpha \) is the thermal diffusivity of the material, in this case, it is set \( \alpha \) = 1.
- \( \frac{\partial u}{\partial t} \) is the partial derivative of \( u \) with respect to time,
- \( \frac{\partial^2 u}{\partial x^2} \) is the second partial derivative of \( u \) with respect to x.
- \( \frac{\partial^2 u}{\partial y^2} \) is the second partial derivative of \( u \) with respect to y.

