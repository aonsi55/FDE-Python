# FDE-Python
Solving Heat equation PDE, using Finite Difference equation.

This repository serves to solve, partial differential equation using finite difference's equation, the equation in discuss is given by, 

$$\frac{\patial T}{\partial t} = \alpha \frac{\partial^2 T}{\partial x^2}$$

This is using finite difference equation, where we will use the fact that, 
$$\frac{dy}{dx} =  \lim_{h\to 0} \frac{ f(x+h) - f(x)}{h},$$
and, 
$$\frac{d^2y}{dx^2} =  \lim_{h\to 0} \frac{ f(x+h) - 2 f(x) + f(x-h)}{h^2},$$

which can be converted into an algebraic expression as follows, 
$$T^{n+1}_{i} = F \( T^{n}_{i+1} + T^{n}_{i-1} \) + (1 - 2 F) T^{n}_{i},$$
such that, 
$$F= \frac{\alpha \Delta t}{(\Delta x)^2},$$
where, $\alpha$ is the conductivity coefficient, $\Delta t$ is the time step for which we want to observe the flow of heat equation, and $\Delta x$ is the spatial step. 

In the given python code, we have implemented the solution to the above problem. 


