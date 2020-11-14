# Comsol manual 

In this note, the method, information and tools are introduced here.

## official blog

.[photonic crystal].(https://www.comsol.com/blogs/engineering-the-flow-of-light-using-photonic-crystals/) 

-  correctly identifying the fundamental and higher-order modes from the total calculated modes. Method 1: perform the integration in the core region.
> apply a filter to the power: $ewfd.neff*(intop1(ewfd.Poavz)>Pthreshold)$, where $P_threshold$ is the power that will eliminate the unnecessary modes.  
> observe the effective mode index number for the fundamental and higher-order modes and if it is getting repeated. 
-  frequent-dependent index: **eigenvalue solver** 
