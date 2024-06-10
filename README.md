# 2D-time-dependent-heat-equation-using-PINNs-tf2-
A Physics-Informed Neural Network to solve 2D time-dependent heat equations.


Inspired by [this](https://github.com/314arhaam/heat-pinn), Which solved a steady-state 2D heat equation using a Physics-Informed Neural Network. In this project, time is introduced. 

The heat equation is a fundamental partial differential equation that describes how heat diffuses through a given region over time. It is widely used in various fields such as physics, engineering, and mathematics to model the distribution of temperature in a given region.

## Governing Equation

The heat equation in two dimensions is given by:

$\displaystyle \frac{\partial u}{\partial t} = \alpha \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} \right) $

where:
- u(x, t) is the temperature distribution function, dependent on position x  and time t,
- $ \alpha $
   is the thermal diffusivity of the material, in this case, it is set
    $ \alpha = 1$
- $\displaystyle \frac{\partial u}{\partial t} $
  is the partial derivative of $ u $ with respect to time,
- $\displaystyle \frac{\partial^2 u}{\partial x^2} $
   is the second partial derivative of $ u $ with respect to x.
- $\displaystyle \frac{\partial^2 u}{\partial y^2} $
   is the second partial derivative of $ u $ with respect to y.

To solve the heat equation, we also need to specify initial and boundary conditions.

### Domain

The domain for the problem is specified as:
$D = {(x,y)| -1 < x < 1 and -1 < y < 1 }$

### Boundary Conditions

The temperature at the boundaries of the square domain are specified as follows:
- Left edge: $ T = 100 $
- Bottom edge: $ T = 100/3 $
- Top edge: $ T = 0 $
- Right edge: $ T = 0 $

It was then normalized. These temperatures remain constant over time.

### Initial Condition

The initial temperature distribution inside the square domain is set to 0:

$\[ u(x, y, 0) = 0 \]$

# Results 
![alt text](https://github.com/RRejuan/2D-time-dependent-heat-equation-using-PINNs-tf2-/blob/main/heat2dpinn.png).
![alt text](https://github.com/RRejuan/2D-time-dependent-heat-equation-using-PINNs-tf2-/blob/main/temperature_evolution.gif)
