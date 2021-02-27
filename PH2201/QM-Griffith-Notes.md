## Wavefunction

In classical mechanics, we solve for $x(t)$, in Newton's laws. In Quantum, we solve for $\psi(x,t)$,in the Schrodinger equation, given by,
$$
i\hbar\frac{\partial \psi}{\partial t}=-\frac{\hbar^2}{2m}\cdot\frac{\partial^2\psi}{\partial x^2}+V\psi
$$

### Interpretation

$|\psi|^2$ gives the proability density. _i,e_,
$$
\int_a^b|\psi|^2dx
$$
All that quantum mechanics can offer is statistical information; not certainty. What is the position of the particle before the measurement? Simply, undefined. 

Measurement radically alters the wave function, in such a way that the wavefunction peaks in the area it is found, resulting in successive measurements yielding the same position of the particle.

So we see that there are two kinds of processes, those in which the wavefunction evolves according to the schrodinger equation, and one where the wavefunction collapses abruptly, following a measurement.

### Probability

#### Most probable value

The most frequent one. That is, the outcome that you are most likely to get if you picked one at random. 

#### Median

That point at which the distribution is divided into two. Getting an outcome on either side of the median outcome is equally probable. 

#### Average

Given by,
$$
\lang j\rang=\sum_{j=0}^\infty jP(j)
$$
In general, the average value of some function of $j$ is given by,
$$
\left< f(j)\right>=\sum_{j=0}^\infty f(j)P(j)
$$

#### Standard deviation

We first calculate the deviation from the average for each outcome.
$$
\Delta j = j-\left<j\right>
$$
We could take the average of this deviation, but that would be zero. Instead, we take the average of the square of this quantity. _i,e_
$$
\sigma^2=\left<(j-\left<j\right>)^2\right>
$$
The above quantity is the _variance_ whose square root gives the standard deviation. 

Another relation is,
$$
\sigma^2=\left<j^2\right>-\left<j\right>^2
$$

### Continuous distributions

The probability that $x$ lies between $a$ and $b$ is given by,
$$
P_{ab}=\int_a^b\rho(x)dx
$$
The same rules for discrete distributions apply for continuous distributions.

#### Normalisation

We require that, 
$$
\int_{-\infty}^{+\infty}|\psi(x,t)|^2dx=1
$$
This called the normalisation condition. The schrodinger equation has the remarkable property that a normalised solution will stay normalised at any time. 

#### Expectation values

The expectation value of $x$ is,
$$
\lang x\rang =\int_{-\infty}^{\infty}x|\psi|^2dx
$$
Physically, this expectation value is the average of repeated measurements of an ensemble of particles all in the state $\psi$.

Now, we can calculate $\frac{d\lang x\rang}{dt}$ which comes out to be,
$$
\frac{d\lang x\rang}{dt}=-\frac{i\hbar}{m}\int\psi^*\frac{\partial\psi}{\partial x}dx
$$
We call this the _velocity of expectation value of $x$_. This is not equivalent to velocity of the particle. 

One result we used in calculating this was, 
$$
\frac{\partial |\psi|^2}{\partial t}=\psi^*\frac{\partial \psi}{\partial x}-\psi\frac{\partial \psi^*}{\partial x}
$$
It is however, easier to work with momentum, and hence we write,
$$
\lang p\rang=m\frac{d\lang x\rang}{dt}=-i\hbar\int\psi^*\frac{\partial\psi}{\partial x}dx
$$

#### Operators

From the previous discussion, we can define position and momentum operators:
$$
\lang x\rang=\int\psi^*(x)\psi dx\\
\lang p\rang = \int\psi^*\left(\frac{h}{i}\frac{\partial}{\partial x}\right)\psi dx
$$
The position operator asks us to _multiply the function with $x$_.

The momentum operator asks us to differentiate with respect to $x$ and multiply by $\hbar/i$.

We say that the operator $x$ represents position, and the operator $\left(\frac{h}{i}\frac{\partial}{\partial x}\right):=\hat p$ represents momentum.

In general,

![image-20210226192536672](/home/sharon/Desktop/Celeste/academic-notes-sem4/PH2201/.markdown-assets/QM-Griffith-Notes.assets/image-20210226192536672.png)

The expectation of a dynamical quantity $Q$ is given by the above equation, for a particle in state $\Psi$.

#### Uncertainty

Fourier analysis shows us that when for a wave, the more precisely its wavelength is determined, the less precisely its position is determined; and vice versa. Given by,
$$
\sigma_x\sigma_p\ge\frac{\hbar}{2}
$$


#### Debroglie 

$$
p=\frac{h}{\lambda}
$$



## Solving the Schrodinger equation

If $V$ is independent of $t$, it can be solved using the method of separation of variables. 

We write:
$$
\Psi(x,t)=\psi(x)\cdot\phi(t)
$$
Substituting in the schrodinger equation, and simplifying,

![image-20210226190136091](/home/sharon/Desktop/Celeste/academic-notes-sem4/PH2201/.markdown-assets/QM-Griffith-Notes.assets/image-20210226190136091.png)

Since LHS if a function of only $t$ and RHS a function of only $x$, these must be identically equal to a constant. We call it $E$. 

Using the usual process, we get,
$$
\psi(t)=e^{-\frac{iEt}{\hbar}}
$$
The other equation, involving $\psi$ is called the time independent schrodinger equation, which can only be solved by specifying $V$. 

Note that, the probability density, is independent of $t$.
$$
|\Psi(x,t)|^2=\Psi^*\Psi=\psi^*\psi e^{-\frac{iEt}{\hbar}}e^{\frac{iEt}{\hbar}}=|\psi(x)|^2
$$
The same for the calculation of any expectation value. 

Thus, solutions of the form $\psi\phi$ are called __Stationary states__. The expectation values do not change with time. Nothing happens in a stationary state.

#### Hamiltonian

We can write the space part of the wave equation as, 
$$
-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2}+V\psi=E\psi
$$
Classicaly, the total energy is the hamiltonian. Stationary states have a definite hamiltonian. 
$$
H(x,p)=\frac{p^2}{2m}+V(x)
$$
In its operator form, the hamiltonian operator is given by,
$$
\hat H = -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}+V(x)
$$
Hence, we can write the space part of the wave equation as,
$$
\hat H\psi=E\psi
$$
Then, the expectation value of the total energy is,
$$
\lang  H\rang = \int\psi^*\hat H\psi dx=\int\psi^* E\psi=E\int\psi^*\psi dx=E\int\Psi^*\Psi dx=E
$$
Similarly, 
$$
\lang H^2\rang=E^2
$$
Then,
$$
\lang H\rang^2 -\lang H^2\rang=E^2-E^2=0
$$
Thus, there is no error in the measurement of energy, for systems in the stationary state. 

Why are we interested in the stationary states? Because, a linear combination of the separable solutions, will give us a solution of the time dependent schrodinger equation, and is of the form,

![image-20210226195817560](/home/sharon/Desktop/Celeste/academic-notes-sem4/PH2201/.markdown-assets/QM-Griffith-Notes.assets/image-20210226195817560.png)

#### Infinite square well

We are given that the potential is $0$ for $x\in(0,a)$ but infinite everywhere else. Now, $\psi$ must be zero outside the well as well. That is,
$$
\psi(x)=0\quad \forall \;x\notin(0,a)
$$
Using the previous analyses, inside the well, the time independent schrodinger equation is given by,
$$
-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2}=E\psi
$$
or,
$$
\frac{d^2\psi}{dx^2}=-k^2\psi
$$
where, 
$$
k=\frac{\sqrt {2mE}}{h}
$$
The general solution for the above equation is 
$$
\psi = A\sin kx+B\cos kx
$$
But $\psi(0)=0$. Then,
$$
\psi(0)=B=0\tag{b1}
$$
Thus, $\psi=A\sin kx$. Now, $\psi(a)=0$. That is,
$$
\psi(a)=A\sin ka=0\\\implies\\k_n=\frac{n\pi}{a}\tag{b2}
$$
This gives, 
$$
E_n=\frac{\hbar^2}{2m}\cdot\frac{n^2\pi^2}{a^2}
$$
We now find $A$ using the fact that $\int \psi=1$
$$
\int A^2\sin^2 (kx) dx=1\\\implies \\A^2=\frac{2}{a}\tag{b3}
$$
Thus, 
$$
\psi_n(x) = \sqrt{\frac{2}{a}}\sin\left(\frac{n\pi}{a}x\right)
$$
Thus, we have arrived at a collection of time independent schrodinger equation solutions. Note the following properties.

1. They are alternately even and odd.

2. Each successive state has one node more than the previous, with the first one having no nodes at all.

3. They are orthogonal. That is,
   $$
   \int \psi_m\psi_n=0
   $$
   Infact, we can combine normalisation and orthogonality into 
   $$
   \int \psi_m\psi_n=\delta_{mn}
   $$

From the previous analyses, we get that 
$$
\Psi_n(x,t)=\sqrt{\frac{2}{a}}\sin\left(\frac{n\pi x}{a}\right)e^{-in^2\pi^2\hbar^2t/2ma^2}
$$
The most general wavefunction is now,
$$
\Psi(x,t)=\sum c_n\sqrt{\frac{2}{a}}\sin\left(\frac{n\pi x}{a}\right)e^{-in^2\pi^2\hbar^2t/2ma^2}
$$
and,
$$
\Psi(x,0)=\sum c_n\sqrt{\frac{2}{a}}\sin\left(\frac{n\pi x}{a}\right)\tag{b4}
$$
So, if we are given $\Psi(x,0)$, the coefficients $c_n$ can be found using fourier analysis and we are done.
$$
c_n= \int \Psi(x,0)\sqrt{\frac{2}{a}}\sin\left(\frac{n\pi x}{a}\right)
$$

> $c_n^2$ gives us the probability of getting a particular $E_n$ for a measurement.

In fact, 
$$
\sum |c_n|^2=1
$$
This follows directly from the normalisation condition of $\Psi$.

In addition, 
$$
\lang H\rang=\sum|c_n|^2E_n
$$

Note that the probability of getting any energy is independent of time and is an expression of the conservation of energy in quantum mechanics.

## Harmonic oscillator

Classically,
$$
F=m\frac{d^2x}{dt^2}=-kx
$$
with solutions,
$$
x=A\cos \omega t+B\sin\omega t
$$
with $\omega=\sqrt\frac{k}{m}$. 

The potential energy is given by,
$$
V(x) =\frac{1}{2}kx^2
$$
_Any_ potential is approximately parabolic in the neighborhood of a local minima. 
$$
V(x)=V(x_0)+V'(x_0)(x-x_0)+\frac{1}{2}V''(x)(x-x_0)^2
$$
At a minima, $V'(x_0)=0$. So,
$$
V(x) = V(x_0)+\frac{1}{2}V''(x)(x-x_0)^2
$$
We can shift the origin appropriately so that,
$$
V(x) = \frac{1}{2}V''(x_0)\cdot(x-x_0)^2
$$
Comparing, we see that the effective spring constant, 
$$
k=V''(x_0)
$$
Thus, our problem is to solve the schrodinger equation for the potential 
$$
V(x)=\frac{1}{2}kx^2=\frac{1}{2}m\omega^2x^2
$$
Our goal is to solve, 
$$
{-h^2\over 2m}\frac{d^2\psi}{dx^2}+\frac{1}{2}m\omega^2x^2\psi = E\psi
$$
Two methods for solving this.

### Algebraic method

We can write the previous equat	ion as,
$$
\frac{1}{2m}\left[\hat p^2+(m\omega x)^2\right]\psi=E\psi
$$
Where the LHS is just an alternate notation for $\hat H$. 

We aim to factor the LHS. However, they are operators and it is not neccessary that $\hat a \hat b=\hat b\hat a$. We defined,
$$
a_\pm=\frac{1}{\sqrt{2\hbar m\omega}}(\mp ip+m\omega x)
$$
We see that,
$$
a_-a_+=\frac{1}{2\hbar \omega m}(p^2+(m\omega x)^2-im\omega(xp-px))
$$
Thus, we see an extra term $(xp-px)$, which we define as the commutator, and is a measure of how badly they fail to commute. 
$$
[x,p]=xp-px
$$
Then, 
$$
a_-a_+=\frac{1}{2m\omega \hbar}(p^2+(m\omega x)^2)-\frac{i}{2h}\left[x,p\right]
$$
We now evaluate $[x,p]$ using a test function $f(x)$ and find that,
$$
[x,p]=i\hbar
$$
Thus, our equation simplifies to,
$$
a_-a_+=\frac{1}{\hbar \omega}H+\frac{1}{2} 
$$
Rearranging gives,
$$
H=\hbar\omega (a_-a_+-\frac{1}{2})
$$
Thus, $H$ does not factor perfectly. Similarly,
$$
a_+a_-=\frac{1}{\hbar \omega}H-\frac{1}{2}\tag{10}
$$
Also note that 
$$
[a_-,a_+]=1	
$$
The crucial step: we claim, _(proved in page 56 of Griffith)_
$$
\hat H\psi=E\psi\implies\hat H(a_+\psi)=(E+\hbar \omega)a_+\psi
$$
Similarly, 
$$
\hat H(a_-\psi)=(E-\hbar\omega)a_-\psi
$$
Here we have an algorithm to find higher and lower energy wavefunctions, if we have just one solution.

#### Lowest energy

We cannot lower indefinitely. A wavefunction cannot have negative energy. We thus find this lowest energy wavefunction.
$$
a_-\psi_0=0
$$
Applying the definition of $a_-$, and integrating, we obtain,
$$
\psi_0(x)=Ae^{-\frac{m\omega}{2\hbar}x^2}
$$
Normalising, we obtain, 
$$
\psi_0(x)=\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}e^{-\frac{m\omega}{2\hbar}x^2}
$$
We find the energy of this state by plugging it into $(10)$. 
$$
E_0=\frac{1}{2}\hbar\omega
$$
Thus, to generate a wavefuntion of higher and higher energy, we apply,
$$
\psi_n(x)=A_n(a_+)^n\psi_0(x)\\
\text{with energies}\\
E_n=\left(n+\frac{1}{2}\right)\hbar\omega
$$
We can do some analysis (page 59 of griffith) to show that,
$$
A_n = \frac{1}{n!}
$$
Here too, we see that the stationary states are orthonormal, and hence we can use the fourier method to determine the full wavefunction.