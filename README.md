# Turbulent/Laminar Mixing Simulator
A python code for fast real-time 2D simulations of scalar mixing in turbulent or laminar flows 

# Install
Install necessary python tools : 
>> pip3 install numpy time PyQt5 vispy scipy

# Run
>> python3 mixing_simulator_v1.0.py

# Change parameters :
Simulation Mode :
- Gradient : Simulate scalar mixing in a mean horizontal scalar gradient $c' = c- \overline{\nabla c} \dot x$
- Decay : Simulate decay of scalar fluctuations (periodic boundaries)
- Source : Simulate mixing of a scalar plume with point source and mean horizontal flow $\langle u \rangle = - 2 A/t_c$

Roughness : Flow velocity roughness, measure by the slope of the velocity lengthscale spectrum: $\langle v(k)^2 \rangle\sim k^{\xi}$. $\xi=-5/3$ in 3D turbulence, $\xi=-3$  in 2D turbulence, $\xi=-\infty$ in single lengthscale laminar flows.

Correlation time : Velocity correlation time $t_c$ of the largest length scale $L=1$. The correlation time of smaller scales $\ell$ is $t_c'(\ell) \ sim t_c \ell$

Amplitude : Amplitude $A$ of the velocity fluctuations. $\langle v^2 \rangle ^{1/2} = A / t_c$

Diffusion : Molecular diffusion of the scalar 
