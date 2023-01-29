# Metastability-Simulation
 Simulating the Metastability in Flip Flops for Visualization purposes

Metastability is a very cruical problem in Embedded Systems which is often considered as *solved* but it isn't. Infact the Developers have reduced it's chances to a very small probabilistic value such that it can be easily avoided by following best design practices. 
<br>
For visualization purposes, I have created this simulation under the supervision of my professor. It shows how Metastability occurs and what are it's aftereffects.


## Schematic 
<p align="center">
  <img src="https://github.com/aitesam961/Metastability-Simulation/blob/main/sch.png" width="950" title="Opening Image">
</p>

<br> 
In the simulation below, It can be seen that the input D of the flip flop changes right on the time when clock is transitioning from LOW to HIGH state.
Resultantly, such a waveform appears where both the outputs of Flip Flops are held to an undefined state for certain amount of time which RESETS to Either side once the clock pulls to LOW.
<br> In simulation environments, It's hard to reproduce such an even due to very high precision of calculation given the fact that most of the Environmental variables are running in Ideal States.

## Simulation
<p align="center">
  <img src="https://github.com/aitesam961/Metastability-Simulation/blob/main/Screenshot%202023-01-02%20212710.png" width="950" title="Opening Image">
</p>

<br> The downside of this work is that the states always set to one side upon every iteration which should'nt happen for a true metastability event.
If someone in the community comes up with a fix for this, Feel free to FORK the Repo and Merge your Solution.

## Simulation Environment

LTSpice is used to create this simulation as it happens to be a sensible choice where we can vary the MOSFET properties and Simulation Variables to a great Extent.
