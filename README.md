# 2D transient heat equation

## Introduction
This repository provides a solution to the transient 2D heat equation using Physics-Informed Neural Networks (PINNs). PINNs leverage the power of deep learning while respecting the underlying physical laws described by partial differential equations (PDEs). This approach allows for the solution of complex PDEs without the need for traditional discretization methods.


## Governing Equation
<p>$$\frac{\partial u}{\partial t} = \alpha \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} \right)$$</p>
where:


**u(x, y, t)  is the temperature distribution**

**$\alpha$ is the thermal diffusivity constant**

**x  and  y  are the coordinates**

**t  is the time variable**


## Domain
<p>$$ \Omega = \{ (x, y, t) \ | \ x \in [0, 1], \ y \in [0, 1], \ t \in [0, 4000] \} $$</p>

where:
- \( x \) and \( y \) are  both ranging from 0 to 1.
- \( t \) is the time variable, ranging from 0 to 4000.


## Boundary Conditions

bottom wall = T(x,0) = 273K

top wall = T(x,1) = 400k

left wall = T(0,y) = 300k

right wall = T(1,y) = 300k


 



**when normalized:**


bottom wall = T(x,0) = 273/400 = 0.6825

top wall = T(x,1) = 400/400 = 1

left wall = T(0,y) = 300/400 = 0.75

right wall = T(1,y) = 300/400 = 0.75

## Initial Condition:
T(x,y,0) = 273k


## Results
**Loss function:**
![Screenshot (642)](https://github.com/user-attachments/assets/ca1e0f4e-6974-480f-bc8a-c6235185b48c)

![temperature_distribution](https://github.com/user-attachments/assets/5e39ace8-c94c-4772-aac0-a9294ef502b5)






