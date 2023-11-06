#### Meta information
23-02-16, 09:09
Status: #idea
Tags: [[ClassicalMolecularDynamics]]





# PotentialFields

- There are different ways to obtain the gradient of the potential of a protein
	- Classical molecular dynamics (force fields)
	- Solving the schrodinger equation
	- Mixed
- Note that there are different force fields, and the difference between them is how we group/aggregate/calculate the energy from the individual interactions.
___
Since we are dealing with moleucles, Interactions can be grouped into two catagories, Bounded interactions and non-bounded interactions.

The goal is to calculate the energy that a molecule will experince in total so we simply sum the two catagories
$$
E_{total} = E_{\text{bounded}} + E_{\text{non-bound}}
$$
___
Furthermore, we can further break this down into individual interactions, for the bounded energy we have 3 different interactions that contribute to the energy:
- Bond energy: atoms that are directly bonded together no separation
$$
E_{\text{bond}} = F_{\text{bond}}(r-r_{eq})
$$
- Angle: atoms that are bonded with a distance of two bonds
$$
E_{\text{angle}} = F_{\text{angle}}(\gamma - \gamma_{eq})
$$
- Dihedral: atoms that lay on the same plance, separated with a distance of 3 bonds.
$$
E_{\text{DIH}} = \sum^n A(q+cos(n \theta + \psi))
$$

Thus we obtain a complete bounded energy term:
$$
E_{\text{bounded}} = E_{\text{bond}} + E_{\text{angle}} + E_{\text{DIH}}

$$
___
Additionally we also break down the non bounded energy contributions from two types of interactions, where the atoms are separated by more than 3 bonds:
- Lennar jones law/interaction, this includes the van der waals interaction (attractive) and the repulsive force:
$$
E_{\text{LJ}} = \frac{A}{r^{12}} - \frac{B}{r^6}
$$
- The coulomb electrostatic interaction:
$$
E_{\text{coulomb}} = \frac{1}{4\pi\epsilon}\frac{q_1q_2}{r^2}
$$
Thus we obtain a complete non bounded energy term:
$$
E_{\text{non-bounded}} = E_{\text{LJ}} + E_{\text{coulomb}}
$$
___
Finally we can obtain a total Energy term for each molecule written as: 

$$
E_{\text{total}} = 

E_{\text{bond}} + E_{\text{angle}} + E_{\text{DIH}} + 
E_{\text{LJ}} + E_{\text{coulomb}}
$$



# References
