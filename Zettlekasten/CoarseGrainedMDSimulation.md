#### Meta information
23-02-16, 09:12
Status: #idea
Tags: [[ModellingResolutions]] [[ProblemsWithClassicalMD]] [[MathematicalFormalismOfPotentialFields]] [[GNNsForMD]]





# CoarseGrainingMDSimulation

Coarse grained molecular dynamics simulations attept to lower the resolution of our physical system, this is done to easy the computational cost and allow for longer simulation times.

In CG simulations, the local atoms are grouped together in a specific and consistent way across our system.

The potential field generated by the coarse grained model is inherintly different and much more simplified that that obtained by the real all-atom force field, this is an apporximation, and could be called a psudo forcefield.

- we expect the all-atom force fed to be highly spike-ful while the coarse grained energy field to be flattened.
- This enables efficent exploration of the enrgy landscape in search for a global minima.





# References
