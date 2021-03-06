# Monte Carlo Simulation of Colloidal Dispersion
The project implements Monte Carlo (MC) method for simulating and studying the system of an electrostatically charged colloid with a salt. 
## Feature of Project: Ewald Summation Method
In this project, we design and implement the Ewald Summation Method to calculate the electrostatic interactions among species.

**The advantage of this method is the rapid convergence of the sum compared with that of a direct summation.** 
This means that the method has high accuracy and reasonable speed when computing long-range interactions, and it is thus the de facto standard method for calculating long-range interactions in periodic systems.


Ewald summation method is a special case of the **Poisson summation formula**, replacing the summation in *real space* with an equivalent summation in *Fourier space*. 
In this method, the long-range interaction between two species is divided into two parts: a short-range contribution, and a long-range contribution which does not have a singularity. 
The short-range contribution is calculated in **real space**, whereas the long-range contribution is calculated using a **Fourier transform**. 




The full project report can be found at [mc_colloid.pdf](https://github.com/rohitnikam1/Monte-Carlo-simulation-colloidal-dispersion/blob/master/mc_colloid.pdf) in this repository. 


Premitive model of 1:1 electrolyte solution has been used to characterize electrostatic interactions among the particles (colloidal particles and ions). 
The total potential energy of the system is tracked as a function of the MC move of a randomly chosen particle. 
It is seen that the energy decreases exponentially during initial MC moves. 
The energy decreases and eventually reaches a plateau as the number of MC moves increases. 
Three systems have been studied -- (1) 2000 ions with 20 colloidal particles, (2) 1000 ions with 10 colloidal particles and (3) 100 ions with 1 colloidal particle.

**Radial density distributions** of oppositely charged ions around each colloidal particle are then calculated. 
For future work, these distributions can in principle be mapped to the Poisson-Boltzmann model for electrolyte distribution around oppositely charged colloidal particle. 
In addition, the **Widom insertion method**, which is a **statistical thermodynamic approach** to the calculation of material and mixture properties, is used to calculate the excess chemical potential of species.

![System of colloidal particle with oppositely charged ions](https://d3jlfsfsyc6yvi.cloudfront.net/image/mw:1024/q:85/https%3A%2F%2Fhaygot.s3.amazonaws.com%3A443%2Fcheatsheet%2F16520.png)
