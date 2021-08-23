---
layout: default
title: projects
permalink: /projects/
---

### Research projects

#### Electron-phonon coupled effective Hamiltonians derived using correlated many-body wave function methods

In some low dimensional meterials, interaction with the collective motion of the atoms leads to a type of ground state called charge density wave, where certain distortions of the lattice are allowed upon lowering temperature.
Bulk 1T-TiSe<sub>2</sub> shows a 2X2 CDW transition at around 232 K, and a 2X2X2 transition at around 205 K. 
Several scenarios have been proposed to explain the origin of the CDW formation: the band Jahn-Teller effect, strong electron-phonon coupling, exciton insulator formed by exciton condensate, and a collaboration between exciton condensation and electron-phonon coupling.
To our knowledge, no first-principles study that is focused on the effect of electron-phonon coupling in 1T-TiSe<sub>2</sub> has ever been reported.
Besides, the cooperation of exciton formation and electron-phonon coupling has not been covered on the level of highly accurate first-principles studies. 
How the energy drop is contributed by electron-phonon coupling and exciton condensation remains quantitatively undetermined.

With density-matrix downfolding method based on quantum Monte Carlo calculations, we can derive a model Hamiltonian for 1T-TiSe<sub>2</sub>, both normal and CDW phases.
This enables us to disentangle the multiple mechanisms underlying the formation of CDW, by attributing the energy drop to the corresponding terms in the Hamiltonian.
 


#### Derive effective Hamiltonians for the dimerization of Hydrogen chains using correlated many-body wave function methods

To perform the density-matrix downfolding method (DMD-QMC) for a more complicated realistic material, it is important to make sure we understand the details of the sampling of the Hilbert space, justify that the compression of the Hamiltonian is reasonable. 
This motivates the benchmark project of performing DMD-QMC for Hydrogen chains. 

The DMD-QMC workflow goes as follows:
- Sample the low-$$E$$ subspace: choose the sub-Hilbert space that we want to model and generate sampled wave functions on this linear space.
- Compress the full Hamiltonian to a model Hamiltonian. Use the QMC data on these sampled wave functions to derive the parameters in the model.  

We would like to derive simplified model Hamiltonians with the following Hubbard form, where $$\tau$$ denotes the atomic displacement from the equally-spaced configuration,

$$ \begin{aligned}
&H_{\text {eff }}=E_{\text {lattice }}(\tau)+\sum_{\text {intra }(i, j\rangle} t_{\text {intra, } i j}(\tau)\left\langle c_{i}^{\dagger}(\tau) c_{j}(\tau)+c_{j}^{\dagger}(\tau) c_{i}(\tau)\right\rangle \\
&+\sum_{\text {inter }\langle i, j\rangle} t_{\text {inter }, i j}(\tau)\left\langle c_{i}^{\dagger}(\tau) c_{j}(\tau)+c_{j}^{\dagger}(\tau) c_{i}(\tau)\right\rangle+\sum_{i} U(\tau)\left(n_{i \uparrow}(\tau) n_{i \downarrow}(\tau)\right\rangle.
\end{aligned} $$

This is a simple Hubbard model with alternating hoppings. 
For smaller bond lengths, including the next-nearest neighbor hoppings can greatly improve the model. 

The DMD framework can be easily combined with other highly accurate first-principles methods. 
Within this framework, we can treat the non-interacting and interacting terms in the model Hamiltonian, as well as the spin-orbit interaction (see [Phys. Rev. Research 2, 013195 (2020)](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.2.013195)) all on the same footing.




