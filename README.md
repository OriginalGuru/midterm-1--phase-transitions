# Midterm Exam #1: Phase Transitions

In class, we motivated why a spring-mass system, or a harmonic oscillator, is so often the focus of study in physics. To name a few, it helps use to understand:

1. oscillatory motion;
2. stable orbits;
3. wave phenomena;
4. and, the behavior of systems near equilibrium.

In this midterm exam, you will explore a (nonlinear) oscillator model, in, very likely, a different way than you have in the past: when the spring constant becomes negative. When this happens we will need to include higher-order terms in our description of the energy, otherwise the mass will accelerate off to infinity.

This model is a model for a broad class of phase transitions, and is used in the [***Landau theory of phase transitions***](https://en.wikipedia.org/wiki/Landau_theory).

Let's start by defining the model.

## The basic model

We can use the following minimal model to describe our system.

$$ U = \frac{1}{2} K Q^2 + \frac{1}{4} D Q^4 $$

where $D>0$ and $K$ can be either positive, zero, or negative.

## Connection to symmetry

The model has broad implications in the study of physical phenomena which can be connected to the symmetry table we derived in class. As a reminder, here is that table:

|               |        | Identity  | Vertical Mirror/Inversion | Horizontal Mirror | 180-degree Rotation |                         |
|---------------|--------|-----------|--------------------------|-------------------|----------------------|-------------------------|
| Object        | Symbol | $E$       | $m_z$                    | $m_y$             | $C_{2y}$             | Example                 |
| Scalar        | $N$  | 1         | 1                        | 1                 | 1                    | $\vec{c} \cdot \vec{c}$  |
| Polar Vector  | $P$  | 1         | -1                       | 1                 | -1                   | $\vec{c}$               |
| Axial Vector  | $G$  | 1         | 1                        | -1                | -1                   | $\vec{a} \times \vec{b}$ |
| Pseudoscalar  | $C$  | 1         | -1                       | -1                | 1                    | $(\vec{a} \times \vec{b}) \cdot \vec{c}$ |

The symbols above follow [Hlinka](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.165502). 

## Broad reaching implications

With some minor adjustments, our model can describe many physical phenomena. A short list of examples from various areas are listed below:

1. **Thermodynamics and Fluid Dynamics.** If two balloons are connected to a valve and inflated together in stages, but are able to exchange air through a patent connection, they will initially inflate together (provided the balloons are similar enough). If we inflate the balloons so they are stretched beyond their linear elastic regime, one of the balloons will empty into the other. This is an example of ***spontaneous symmetry breaking***. The system starts symmetric, with the left and right balloons inflating approximately in unison. Once we reach a threshold in pressure in the balloons, one of the balloons will take up all of the slack and the other will be empty. Since it is easy for us to track or measure, we could use the difference in the volume of the two balloons (i.e. $\epsilon = \left(V_{right}-V_{left}\right)/V_{total}$ as a way to track this behavior. Looking at our energy equation, this means that $Q=\epsilon$. With this choice, $K$ represents the stiffness or elasticity of the rubber in the balloon. The difference between the two volumes, $\epsilon$ can be represented by a polar vector, connecting to our discussion of symmetry in one dimension. This is because the inversion operation and the 180-degree rotation switch the two balloons, but the other mirror leaves them unchanged.
2. **Mechanics.** If we take a thin cylindrical beam oriented vertically between the floor and a piston we can see that it has rotational symmetry. If we engage the piston, the beam will be under pressure and eventually, after some threshold is reached, the beam will bow to the left, or right, or front, or back... Again, this problem can be mapped onto our spring-mass model, by taking $Q$ to be the deviation of the beam from midline, and $K$ as some description of the beam's elasticity. If we look at our initial configuration, we have all of the symmetries present (vertical mirror, horizontal mirror, 180-degree rotation) in our symmetry table. Once the beam bows, we lose the horizontal mirror and the 180-degree rotation symmetries. That means that this situation can be described by an axial vector.
3. **Ferromagnetism.** Many materials, when cooled below a critical temperature become magnetic (called the *Curie temperature*). For example, iron (Fe), where we get the *ferro* prefix from, has a Curie temperature of between 1000 K and 1600 K. This behavior is due to the collective orientation of the electron spins in iron. In our simple model, $Q$ would represent the magnetization. When the temperature goes below the Curie temperature, the parameter $K$ becomes negative.
4. **Superconductivity** Here $Q$ would need to be complex to represent the density and global quantum mechanical phase of the superconductor.
5. **Higgs mechanism.** Here $Q$ describes the breaking of the electroweak symmetries.
6. **Quantum Chromodynamics.** Chiral symmetry breaking in quarks.
7. **Galaxy Formation.** In the early universe, matter is thought to have been uniformly distributed. Small deviations are thought to have led to galaxy formation where matter started to clump together. In this case, $Q$ would be the deviation of the density of matter from the average value.
8. **Crystallization.** The transition from a liquid to a crystalline solid is very similar to galaxy formation.
9. **Biology/Biophysics.** Many biological systems exhibit chirality/handedness at various scales. This preference for one handedness over another can be described by our model.

## Complete the following questions in the attached `Jupyter Notebook`. Use code cells to complete the plotting and any other computational work. Use the `Markdown` cells to answer the conceptual questions. Use `Latex` for equations.

### Problem 1 (20 points)

1. Create an interactive plot with `matplotlib` and `ipywidgets` to show what happens when $K$ becomes negative. Label your axes and make your plot clear and aesthetically pleasing. Your finished plot should compare $K>0$ and $K<0$ to illustrate your findings.

2. With the insights drawn from your plot, find an expression for the amplitude of $Q$ as a function of $K$ and $D$. 

3. Assume that the effective mass of the coordinate $Q$ is $m$. Find an expression for the frequency of the oscillator for $K>0$ and $K<0$.

### Problem 2 (20 points)

Let's expand the model to include two degrees of freedom.

$$ U = \frac{1}{2} K_1 Q_1^2 + \frac{1}{2} K_2 Q_2^2 + C Q_1^2 Q_2 + \frac{1}{4} D_1 Q_1^4 + \frac{1}{4} D_2 Q_2^4 + \frac{1}{2} D_{12} Q_1^2 Q_2^2 $$

Take all coefficients to be positive to start.

1. Create an interactive contour plot of the energy. Label your axes and make your plot clear and aesthetically pleasing. Explore what happens when ***either*** $K_1$ or $K_2$ becomes negative.

2. When $K_1$ becomes negative what happens to $Q_1$, and what happens to $Q_2$. Explain.

3. When $K_2$ becomes negative what happens to $Q_1$, and what happens to $Q_2$. Explain.

4. What changes above if $C$ is negative?

### Problem 3 (10 points)

1. Use the symmetry table to explain which degrees of freedom ($N$, $P$, $G$, and $C$) can be described by **Problem 1**.
2. Use the symmetry table to explain which degrees of freedom ($N$, $P$, $G$, and $C$) can be coupled to each other as described in the model of **Problem 2**.
3. Is there a way to have a third-order term $Q_1 Q_2 Q_3$? If so, which degrees of freedom allow for this and why? It not, why not?

