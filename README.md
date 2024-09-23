# Midterm Exam #1: Phase Transitions

In class, we motivated why a spring-mass system, or a harmonic oscillator, is so often the focus of study in physics. To name a few, it helps use to understand:

1. oscillatory motion;
2. stable orbits;
3. wave phenomena;
4. and, the behavior of systems near equilibrium.

In this midterm exam, you will explore a (nonlinear) oscillator model, in, very likely, a different way that you have in the past; when the spring-constant becomes negative. When this happens we will need to include higher order terms in opur description of the energy, otherwise the mass will accelerate off to infinity.

Let's start by defining the model.

## The basic model

We can use the following minimal model to describe our system.

$$ U = \frac{1}{2} K Q^2 + \frac{1}{4} D Q^4 $$

where $D>0$ and $K$ can be either positive, zero, or negative.

The model has broad implications in the study of physical phenomena which can be connected to the symmetry table we derived in class. As a reminder, here is that table:

|               |        | Identity  | Vertical Mirror/Inversion | Horizontal Mirror | 180-degree Rotation |                         |
| Object        | Symbol | $E$       | $m_z$                    | $m_y$             | $C_{2y}$             | Example                 |
|---------------|--------|-----------|--------------------------|-------------------|----------------------|-------------------------|
| Scalar        | $Q_1$  | 1         | 1                        | 1                 | 1                    | $\vec{c} \cdot \vec{c}$  |
| Polar Vector  | $Q_2$  | 1         | -1                       | 1                 | -1                   | $\vec{c}$               |
| Axial Vector  | $Q_3$  | 1         | 1                        | -1                | -1                   | $\vec{a} \times \vec{b}$ |
| Pseudoscalar  | $Q_4$  | 1         | -1                       | -1                | 1                    | $(\vec{a} \times \vec{b}) \cdot \vec{c}$ |




A short list of examples from various areas of physics are listed below:

1. If two balloons are connected to a valve and inflated together in stages, they will initially inflate together while the rubber in the balloon has linear elastic properties (provided the balloons are similar enough). If we inflate the balloons so they are stretched beyond their linear elastic regime, one of the balloons will empty into the other. This is an example of ***spontaneous symmetry breaking***. The system starts symmetric, with the left and right balloons inflating approximately in unison. Once we reach a threshold in pressure in the balloons, one of the balloons will take up all of the slack and the other will be empty. Since $P\times V$ (pressure times volume) has units of energy, we can anticipate that in our equation for the energy, $Q$ would represent the difference in pressure of the two balloons (i.e. $Q=P_{right}-P_{left}$), and $K$ is proportional to elasticity times some reference volume, $\epsilon V_0$. (This is typical when dealing with elasticity.) The difference between the two pressures can be represented by a polar vector, connecting to our discussion of symmetry in one dimension.
2. If we take a thin cylindrical beam oriented vertically between the floor and a piston we can see that it has rotational symmetry. If we engage the piston, the beam will be under pressure and eventually, after some threshold is reached, the beam will bow to the left, or right, or front, or back... Again, this problem can be mapped onto our spring-mass model, by taking $Q$ to be the deviation of the beam from midline, and $K$ as some description of the beam's elasticity. If we look at our initial configuration, we have all of the symmetries present (vertical mirror, horizontal mirror, 180-degree rotation) in our symmetry table. Once the beam bows, we lose the horizontal mirror and the 180-degree rotation symmetries. That means that this situation can be described by an axial vector.
