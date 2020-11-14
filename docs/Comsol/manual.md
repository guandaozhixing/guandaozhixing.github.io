# Comsol manual 

In this note, the method, information and tools are introduced here.

## official blog

[photonic crystal](https://www.comsol.com/blogs/engineering-the-flow-of-light-using-photonic-crystals/) 

-  correctly identifying the fundamental and higher-order modes from the total calculated modes. Method 1: perform the integration in the core region.
> apply a filter to the power: ***ewfd.neff*(intop1(ewfd.Poavz)>Pthreshold)***, where **P_threshold** is the power that will eliminate the unnecessary modes.  
> observe the effective mode index number for the fundamental and higher-order modes and if it is getting repeated. 
-  frequent-dependent index: **eigenvalue solver** [comsol blog](https://www.comsol.de/model/band-gap-analysis-of-a-photonic-crystal-798)
>  extended to the non-single components of electric field. [^extension]  











-----
[^extension]: The normalization integral, which must be defined over the volume and considering all components of the electric field: $V=intop1(1)$, 
$nE=intop1(realdot(ewfd2.Ex, ewfd2.Ex)+realdot(ewfd2.Ey, ewfd2.Ey)+realdot(ewfd2.Ez, ewfd2.Ez))/V$, [reference1](https://www.researchgate.net/post/Simulation-of-photonic-crystal-waveguides-to-find-band-structure-by-COMSOL)  
