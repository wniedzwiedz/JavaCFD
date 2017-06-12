
<h1>JavaCFD</h1><br>
Computational fluid dynamics software written in Java using the Lattice-Boltzmann method. Allows custom-defined, arbitrary geometries in 2D incompressible flow field.<br>

<hr><br>
TO RUN: Execute JavaCFD.pde in the NonOOP folder of the main branch. The object-oriented version optimizes the Lattice-Boltzmann code for Java but is still a work in progress. Check the demo folder for newest updates on the OOP version.<br>
1) set sliders for velocity and viscosity<br>
2) set display to velocity<br>
3) click start, and draw geometry on the fluid field by clicking and dragging<br>
- set the scaling slider to optimize display<br>
- clicking start again resets the simulation<br><br>

If the screen has a uniform color, adjust the scale slider until you have good contrast. It is good to start on velocity mode as that gives the normal, intuitive picture of fluid flow.<br>

If the fluid looks like it is being infested with a red virus erasing all the elements, you have saturated the algorithm and caused it to diverge. Simply click start again to reset.<br>

<br>
Note that the simulation is highly CPU intensive and only small fluid fields should be attempted on most machines. <br>

<hr><br>

Computational fluid dynamics is used extensively in engineering to accurately model fluid flow and its associated phenomena. Turbulent flow/hypersonic flow/vortex shredding etc can be simulated using the Navier-Stokes equations, which describe fluid flow using the conservation of momenta and mass flow. However, as they are nonlinear partial differential equations, a solver is very difficult to code.<br> 

The Lattice-Boltzmann method works in a way comparable to cellular automata. By discretizing thermal velocities for each element and then reassigning it based on the Boltzmann distribution, it is able to very accurately reconstruct the behavior of the Navier-Stokes equations in subsonic velocities (higher velocities require thermal coupling). In fact it is even more accurate in modeling turbulent flow and is optimized for massively parallel architectures. We have created our own implementation of the Lattice-Boltzmann algorithm with the D2Q9 model (two dimensions, 9 discretized velocities).<br><br>

Written for Mr. Konstantinovich's AP Computer Science Class, Stuyvesant High School.<br>
<hr><br>
References:
The bulk of the math comes from Alex Wagner's paper, A Practical Introduction to the Lattice-Boltzmann Method. https://www.ndsu.edu/fileadmin/physics.ndsu.edu/Wagner/LBbook.pdf <br>
Lindsay Crowl's GSAC Talk, http://www.math.utah.edu/~crowl/pres.pdf <br>
Weber State University's project on Lattice-Boltzmann, http://physics.weber.edu/schroeder/javacourse/LatticeBoltzmann.pdf
<hr><br>
*WORK IN PROGRESS*
