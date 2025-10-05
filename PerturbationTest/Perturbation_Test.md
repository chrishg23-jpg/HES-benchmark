Perturbation Test: Reversibility in Windy Weather

To probe the resilience of the HES framework, we introduced localized perturbations—random velocity kicks—midway through a reversible simulation. This “windy weather” scenario allowed us to test whether time symmetry holds when the system is exposed to chaotic fluctuations.


![Figure 1: Perturbation Test](Figures/Pert001.png)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/chrishg23-jpg/HES-benchmark/blob/main/PerturbationHES001.ipynb)

The forward trajectory absorbed the perturbation and continued evolving with partial coherence. However, the reverse trajectory, initiated from the perturbed final state, failed to reconstruct the original configuration. This breakdown illustrates the edge of reconstructability: once memory is diffused into the environment, the reverse path becomes inaccessible.

Although quantum mechanics preserves information in principle, decoherence renders it unreachable in practice. The memory becomes a ghost in the wavefunction—present in the global state, but lost to any local observer. These results support the view that irreversibility emerges not from fundamental asymmetry, but from the dispersion of memory and the limits of reconstruction.


