Plan of attack:

- the formulation
- digest each term of the formulation
- do tons of examples
- understand how one could come up with the equation intuitively.

#formulation

There have been several.

A good one is the [von Neumann formulation](http://en.wikipedia.org/wiki/Dirac%E2%80%93von_Neumann_axioms)
which we consider here.

The two questions are:

- how do we describe a quantum system.

    Answer:

    1) All the state of a quantum system is described by an **unit vector**
    of a [Hilbert space](#hilbert-space) $H$.

    2) Observables of a quantum system are defined to be the (possibly unbounded)
    [self-adjoint operators](#self-adjoint-operator) $A$ on $H$.

    3) The expectation value of an observable $A$ for a system in a state
    $\phi$ is given by the inner product $(\phi,A\phi)$

- how does the system evolve with time.

    This is given tby the [Shrodinger's equation](http://en.wikipedia.org/wiki/Schr%C3%B6dinger_equation)
    which like Newton's equation does for classical systems is a differential equation (it is however partial).

        $i \hbar \frac{\partial}{\partial t}\Psi = \hat H \Psi$

    On this equation, the only thing that determines a property of an specific system
    is the potential $\hat H$.

First we must digest that. After, get down to some simple examples and it will be crystal clear.

##hilbert space

A [Hilbert space](http://en.wikipedia.org/wiki/Hilbert_space) is a:

- [vector space](http://en.wikipedia.org/wiki/Vector_space)

- with an [inner product]()

- such that the norm induced by the inner product makes the space complete

    You should know that for every inner product $<u,v>$ we can create a norm
    (a function that satisfies the properties of the definition of a norm)
    $|u| = \sqrt{<u,u>}$

    A space is complete if every Cauchy sequence converges on it to a point on the space.

    A simple example of Hilbert space is $R^n$.

But in quantum mechanics, we will most often consider Hilbert spaces made up of
functions with the following inner product:

##self adjoint operator

##countable

You should know that 
