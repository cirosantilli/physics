Plan of attack:

- do some 1D examples
- see the fully blasted formulation
- digest each term of the formulation
- understand how one could come up with the equation intuitively.

#prerequisites

- differential equations. Cannot do anything without them.
- basics of continuous probability distributions.
- basics of Newtonian physics. Momentum and Newton's law.

#sources

[gri04]: http://www.amazon.com/Introduction-Quantum-Mechanics-2nd-Edition/dp/0131118927

- [Griffiths - Introduction to Quantum Mechanics (2nd Edition)][gri04]

    *Very* clear. Good introduction.

#introduction

TODO

The wave function is the probability density of finding a particle on a region of space at a given time.

The [Shrodinger's equation](http://en.wikipedia.org/wiki/Schr%C3%B6dinger_equation) says how the probability evolves with time.
Like Newton's equation does for classical systems is a differential equation (it is however partial).

$$i \hbar \frac{\partial}{\partial t}\Psi = \hat H \Psi$$

with:

$$H = TODO$$

On this equation, the only thing that determines a property of an specific system
is the potential $\hat H$. It is analogous to the potential field $V$ in classical mechanics
from which the force can be derived as $\vec{F} = \nabla V$

If the potential is constant with time, we can break Shrodinger's equations 
by separation of variables.

##example: infinite well

Energy quantization example.

TODO

##example: harmonic oscilator

Energy quantization example.

TODO

#formulation

There have been several.

A good one is the [von Neumann formulation](http://en.wikipedia.org/wiki/Dirac%E2%80%93von_Neumann_axioms)
which we consider here.

##how do we describe a quantum system.

1) All the state of a quantum system is described by an **unit vector**
of a [Hilbert space](#hilbert-space) $H$.

2) Observables of a quantum system are defined to be the (possibly unbounded)
[self-adjoint operators](#self-adjoint-operator) $A$ on $H$.

3) Every measure of an observable gives as result an eigenvector of $A$

    Every measure affects the state of a system. After a measure has been made,
    the state of the system becomes exactly the one observed.

    The probability of getting each eigenvector $\Phi$ is given by $(\Phi,A\Phi)$.

    As a consequence, the expectation value of an observable $A$ for a system in a state
    $\phi$ is given by the inner product 

First we must digest the definition.

After, get down to some simple examples and it will be crystal clear.

It will also be necessary to solve the Shrodinger equation for some simple cases to see what it gives.

##hilbert space

A simple example of Hilbert space is $R^n$.

In quantum mechanics, we will most often consider Hilbert spaces made up of
functions with the following inner product:

TODO why the integral?

A [Hilbert space](http://en.wikipedia.org/wiki/Hilbert_space) is a:

- [vector space](http://en.wikipedia.org/wiki/Vector_space)
- with an [inner product]()
- such that the norm induced by the inner product makes the space complete.

###completeness

You should know that for every inner product $(u,v)$ we can create a norm
( a function that satisfies the properties of the definition of a norm)
$|u| = \sqrt{(u,u)}$

A space is complete if every Cauchy sequence converges on it to a point on the space.

Completeness in function spaces is a bit delicate.

To fully grasp it,
you must understand the $L^p$ spaces and why they are complete.
This in turn requires that you understand the Lebesgue integral:
the Reimann integral is simply not good enough to assure completeness
on spaces with $L^p$ products

In practice, thinking with the Reimann integral mostly works,
but to really understand things it is necessary to understand $L^p$.

##self-adjoint operator

The advantage of restricting ourselves to self-adjoint operators is that
the spectrum of any bounded symmetric operator is real.

This means that all the measures that we make give real values.

TODO what happens if not bounded?

A problem arises with self-adjoint operators, by the
[Hellinger-Toeplitz theorem](http://en.wikipedia.org/wiki/Hellinger-Toeplitz_theorem)
when those are not bounded they cannot be defined everywhere.

This is the case for the energy of an harmonic oscillator it is unbounded
(its eigenvalues are 1/2, 3/2, 5/2, ...), so the energy cannot be defined for *all*
possible states.
