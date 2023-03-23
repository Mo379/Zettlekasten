#### Meta information
23-02-16, 17:57
Status: #idea
Tags: 





# RevertingCoarseGrainedToAllAtom

The article discusses the challenges in using coarse-grained configurations to investigate molecular properties that require atomic resolution. The authors propose a two-stage process that involves sampling coarse-grained configurations in proportion to their Boltzmann probability and then using an invertible neural network to harvest a statistical sample of fine-grained configurations. The authors also discuss how to correct discrepancies in the coarse-grained potential and how to reweight the generated samples. The proposed approach can accelerate exploration of the free energy landscape while reconstructing fine-grained configurations.








In molecular simulations, scientists need to investigate properties of molecules at an atomic level, which can be challenging. To address this, the authors of the article propose a two-stage process that involves using a simpler, coarse-grained representation of the molecule to sample a variety of possible configurations. They do this by randomly generating a set of coarse-grained configurations that represent possible shapes and arrangements of the molecule.

Next, they use an advanced mathematical tool called an invertible neural network to generate more detailed, fine-grained configurations of the molecule. The neural network allows them to generate a statistical sample of fine-grained configurations in a way that takes into account the true probability of each configuration. This is important because some configurations are more likely to occur than others, and the neural network can ensure that the generated configurations accurately reflect these probabilities.

To make sure their approach is accurate, the scientists also correct for any discrepancies in the way they represent the molecule in the coarse-grained model. They do this by using a process called back-projection, which helps them refine their coarse-grained model and generate more accurate fine-grained configurations.

Overall, the scientists' approach allows them to explore the properties of molecules more efficiently, by generating a variety of possible configurations and then using an advanced mathematical tool to generate more detailed configurations that accurately reflect the probability of each configuration occurring.





# References
