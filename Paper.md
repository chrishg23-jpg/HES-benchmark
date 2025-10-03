Introduction

The nature of spacetime remains one of the deepest puzzles in theoretical physics. While General Relativity describes gravity as curvature in a geometric manifold, and Quantum Mechanics governs the probabilistic behavior of particles, a unified framework that explains how spacetime itself emerges from quantum principles remains elusive.

Recent advances in quantum information theory suggest that entanglement may play a foundational role in the emergence of spacetime geometry. The idea that “geometry is entanglement” has gained traction—but concrete, reproducible models remain rare.

This paper introduces a toy model based on the Holographic Entropic Spacetime (HES) framework, where curvature arises from entropy gradients in a discrete lattice of microstates. The model simulates how local entropic interactions and global feedback dynamics can generate stable geometric structure without invoking mass or classical fields.

We present a reproducible benchmark notebook that visualizes this process, offering a hands-on demonstration of how information structure alone can give rise to curvature. The results support the hypothesis that spacetime may be a macroscopic manifestation of underlying entropic dynamics—and open new avenues for exploring emergent gravity from first principles.

---

Theoretical Framework

The Holographic Entropic Spacetime (HES) framework proposes that spacetime curvature emerges from gradients in entanglement entropy across a discrete lattice of quantum microstates. Rather than treating geometry as a fundamental entity, HES models it as a macroscopic manifestation of underlying informational structure.

Each site in the lattice represents a quantum microstate. The system evolves by minimizing a fundamental Informational Action `\( \mathcal{A} \)`.

---

Local Entropic Dynamics: The Entanglement Analogue

Entropy quantifies the local informational tension. In this simplified classical toy model, we use the Shannon entropy as an analogue for the quantum Von Neumann entropy.

The local entropy at site `\( (x, y) \)` is defined as:

S(x, y) = - \sum_i p_i(x, y) \log p_i(x, y)


where `\( p_i(x, y) \)` is the probability distribution over microstates in the local neighborhood of `\( (x, y) \)`.

---

Global Feedback Stabilization: The Informational Action

The system’s evolution minimizes the total Informational Action `\( \mathcal{A} \)`, which combines the summed entropic density `\( S \)` and a stabilizing global feedback term `\( E_{\text{global}} \)`:

\mathcal{A}(t) = \sum_{x,y} S(x, y, t) + E_{\text{global}}(t)


The global feedback term suppresses vacuum energy fluctuations, acting as a damping mechanism:

E_{\text{global}}(t) = \gamma \left( \sum_{x,y} S(x, y, t) \right)^2


where `\( \gamma \)` is a tunable damping coefficient.

---

Curvature from Entropy: The Ricci Analogue

To extract curvature, we apply a discrete Laplacian operator `\( \nabla^2 \)` to the entropy field `\( S(x, y) \)`, yielding a curvature map `\( C(x, y) \)`:

C(x, y) = \nabla^2 S(x, y)


In this two-dimensional discrete lattice, `\( C(x, y) \)` serves as a direct analogue for the Ricci scalar `\( R \)`, demonstrating that geometry bends due to entropic structure.

---

Dynamical Update Rule (Key for Reproducibility)

The system evolves iteratively toward minimizing the total Informational Action `\( \mathcal{A} \)` using a stochastic dynamics approach (e.g., Metropolis-Hastings). At each time step, a random site’s microstate is proposed to flip `\( \mu \to \mu' \)`, and the change in action `\( \Delta \mathcal{A} \)` is computed.

The probability `\( P \)` of accepting the flip is:

P(\mu \to \mu') = \min \left( 1, \exp \left( -\frac{\Delta \mathcal{A}}{T} \right) \right)


where `\( T \)` is the effective informational temperature, held constant to simulate low-energy equilibrium.



Results and Interpretation

The HES benchmark simulation produces four key outputs: the evolving microstate lattice, the entropy map, the curvature map, and a time-series analysis of global entropy and energy. Together, these results illustrate how entropic structure alone can generate stable curvature in a discrete spacetime model.

1. Microstate Lattice Evolution

The initial lattice consists of randomly assigned microstates, representing a high-entropy, disordered configuration. As the simulation progresses, local entropic interactions and global feedback dynamics smooth the lattice, driving it toward equilibrium.


![Figure 1: Microstate Lattice Evolution](Figures/Figure_1.PNG)
Figure 1: Microstate Lattice Evolution

The system transitions from a high-entropy, disordered state to a smooth, stable configuration through local entropic interactions and global feedback.

Interpretation:
This evolution demonstrates that local entropy gradients can self-organize into coherent structure. The system stabilizes without external constraints, suggesting that informational dynamics alone can produce order.

---

2. Entropy Map


The entropy map visualizes the distribution of local entanglement across the lattice. High-entropy regions appear as smooth gradients, while low-entropy zones reflect equilibrium or alignment.

![Figure 2: Entropy Map](Figures/Figure_2.PNG)
Figure 2: Entropy Map

Entropy gradients reveal hidden structure in the lattice. High entropy regions indicate strong local entanglement; low entropy regions reflect equilibrium.

Interpretation:
Entropy acts as a proxy for informational connectivity. The emergence of smooth gradients indicates that entanglement structure can encode geometric features, supporting the hypothesis that spacetime may be woven from entropic relationships.

---

3. Curvature Map

Applying a discrete Laplacian to the entropy field yields a curvature map. This map reveals how entropy gradients bend the lattice geometry, producing warps and folds without invoking mass or classical fields.

![Figure 3: Curvature Map](Figures/Figure_3.PNG)
Figure 3: Curvature Map

Applying a Laplacian operator to the entropy map yields emergent curvature. Geometry bends in response to information structure, not mass.

Interpretation:
Curvature emerges directly from entropy. This result aligns with the idea that spacetime geometry is not fundamental, but emergent from deeper informational principles. The model provides a concrete, reproducible demonstration of this concept.

---

4. Time-Series Analysis

The simulation tracks global entropy and energy over time. Entropy stabilizes early, indicating equilibrium, while global energy exhibits damped oscillations due to feedback dynamics.

![Figure 4: Time-Series Analysis](Figures/Figure_4.PNG)
Figure 4: Time-Series Analysis

Entropy stabilizes early, indicating equilibrium. Global energy oscillates due to feedback dynamics, revealing the system’s self-regulating behavior.

Interpretation:
The system self-regulates through entropic feedback. The early stabilization of entropy suggests that equilibrium geometry can emerge quickly, while energy oscillations reflect the interplay between local structure and global constraints.

---

Summary of Findings

• Entropic gradients can self-organize into stable geometric structure
• Curvature arises from information, not mass
• The system stabilizes through global feedback without external tuning
• The model offers a reproducible testbed for emergent spacetime hypotheses


Relation to Existing Frameworks

• Einstein-Hilbert Action Analogue: The Informational Action `\( \mathcal{A} \)` acts as a minimal analogue to the Einstein-Hilbert action of General Relativity, where the entropy sum `\( \sum S \)` promotes stability.
• Van Raamsdonk’s Conjecture: Geometry stems from entanglement.
• Jacobson’s Derivation: Spacetime dynamics emerge from entropy balance.


Conceptual Comparison

• General Relativity: Curvature emerges from mass-energy; in HES, it emerges from entropy gradients.
• Quantum Gravity: Many models rely on discrete spacetime or spin networks; HES uses entropic feedback on a lattice.
• Entropic Gravity (Verlinde): Shares the idea of gravity as emergent from entropy, but HES adds dynamic feedback and curvature maps.

## Comparison to Other Models

| Model                  | Curvature Source        | Time Evolution | Visual Output            |
|------------------------|-------------------------|----------------|--------------------------|
| General Relativity     | Stress-energy tensor    | Continuous     | Metric tensor            |
| Entropic Gravity       | Information gradients   | Static         | Conceptual diagrams.     |
| **HES (Your Model)**   | Entropy + feedback loop | Dynamic        | Lattice + curvature maps |

Conceptual Comparison

• General Relativity:
  • Curvature Emerges From: Mass-Energy
  • Core Mechanism: Curvature of a geometric manifold
  
• Quantum Gravity Models (e.g., Causal Sets, Spin Networks):
  • Curvature Emerges From: Discrete/Quantum Principles
  • Core Mechanism: Spin networks, causal sets, or tensor graphs
  
• Entropic Gravity (Verlinde):
  • Curvature Emerges From: Entropy/Information Gradients
  • Core Mechanism: Thermodynamic response to information difference
  
• HES (Your Model):
  • Curvature Emerges From: Entropy and Global Feedback
  • Core Mechanism: Minimization of Informational Action (\bm{\mathcal{A}}) on a lattice

Comparison to Other Models (Focus on Dynamics and Output)

• General Relativity:
  • Curvature Source: Stress-energy tensor (\bm{T_{\mu \nu}})
  • Time Evolution: Continuous
  • Visual Output: Metric tensor
  
• Entropic Gravity:
  • Curvature Source: Information gradients
  • Time Evolution: Static
  • Visual Output: Conceptual diagrams
  
• HES (Your Model):
  • Curvature Source: Entropy + feedback loop (\bm{\mathcal{A}})
  • Time Evolution: Dynamic
  • Visual Output: Lattice + curvature maps

Final Conclusion and Outlook Summary
The HES framework successfully bridges entropy, geometry, and emergence by demonstrating that spacetime curvature is a consequence of self-regulating informational dynamics. The next steps focus on formally linking the Informational Action (\bm{\mathcal{A}}) to the Einstein-Hilbert Action and expanding the model into a full quantum information context using Tensor Networks and Von Neumann Entropy.

Conclusion and Outlook

This work introduces the HES framework, where curvature emerges from the structure and evolution of entropy and a global informational action. By defining a rigorous dynamical update rule, we demonstrate that spacetime-like curvature can arise from purely informational dynamics.

The results suggest that entropic gradients and self-regulating feedback mechanisms may be foundational to emergent geometry.

Future Directions

• Quantum Information Analogue: Replace Shannon entropy with Von Neumann entropy and implement the lattice as a tensor network (e.g., MERA).
• Formal Gravitational Isomorphism: Establish a mathematical link between the HES Informational Action `\( \mathcal{A} \)` and the Einstein-Hilbert action `\( \mathcal{S}_{\text{EH}} \)`.
• Dimensional and Dynamical Expansion: Extend to 3D lattices and incorporate causal structure or matter-like degrees of freedom.
• Comparative Benchmarking: Compare emergent geometry (e.g., spectral dimension) with causal dynamical triangulations and causal sets.


By bridging entropy, geometry, and emergence, HES offers a new lens on the deep structure of reality. It invites us to ask: what if spacetime is not the canvas, but the consequence?
