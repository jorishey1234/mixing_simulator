# mixing_simulator
A python script to simulate scalar mixing by turbulent or laminar flows in real time 

# Install
Install necessary python tools : 
>> pip3 install numpy time PyQt5 vispy scipy

# Run
>> python3 mixing_simulator_v1.0.py

# Change parameters :
Roughness : Flow velocity roughness, measure by the slope of the velocity lengthscale spectrum: <v(k)²>^{1/2}\sim k^{\xi}. $\xi=5/6$ in 3D turbulence, $\xi=-2$  in 2D turbulence, $\xi=-\infty$ in single lengthscale laminar flows.
Correlation time : Velocity correlation time $t_c$ of the largest length scale $L$. The correlation time of smaller scales is $t_c' \ sim t_c L/\ell$
Amplitude : Amplitude $A$ of the velocity fluctuations. $<v²>^{1/2} \sim A / t_c$
Diffusion : Molecular diffusion of the scalar 
