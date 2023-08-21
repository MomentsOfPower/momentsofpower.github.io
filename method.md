The basic premise of "moments of power" is simple. 

Imagine an energy conversion system, such as an electric motor. 
The input variable is the mechanical power demand $P$, and the output variable is the electrical input power $Y$. 
$Y$ is a function of $P$: 

$$ Y=f(P) $$

This function can be approximated using a polynomial such as:

$$ Y = Y_0 + Y_1 P + Y_2 P^2 + Y_3 P^3 $$

The overall electrical energy demand can be found by integrating $Y$:

$$ E = \int Y dt $$

So far, so conventional. This value can be established using a simulation in one of many simulation tools. However, there is also an algebraic solution. 

Insert the polynomial into the integral leads to 

$$ E = \int Y_0 + Y_1 P + Y_2 P^2 + Y_3 Y^3 dt $$

which can be separate into 

$$ E = Y_0 \int dt + Y_1 \int P dt + Y_2 \int P^2 dt + Y_3 \int P^3 dt $$

Those integrals are related to the moments of the distributino of P, which are familiar statistical measures, leading to:

$$ E = T ( Y_0 + Y_1 \mu_1 + Y_2 \mu_2 + Y_3 \mu_3) $$

This way, the electrical energy consumption can be calculated using a simple set of multiplications, without the numerical complexity of a simulation. 
And more importantly, the algebraic solution gives greater insight into how to reduce the energy consumption. 
This is helpful for analysing any energy system under realistic usage conditions. 
