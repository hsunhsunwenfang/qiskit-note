

# Matrix Methamatics

## Latex Library

- $$V_{sphere} = \frac{4}{3}\pi r^3$$
- $$\langle a_{jj}|$$
- Matrix Multiplication Example
$$M1=\begin{pmatrix}1 & 1\\0 & 0\end{pmatrix}\hspace{0.5em},\hspace{0.5em}M2=\begin{pmatrix}0 & 1\\1 & 0\end{pmatrix}$$
$$M1M2=\begin{pmatrix}1 & 1\\0 & 0\end{pmatrix}\hspace{0.5em},\hspace{0.5em}M2M1=\begin{pmatrix}1 & 1\\0 & 0\end{pmatrix}$$


## Dirac Notation

- "bra" $\langle a|$ is a row vector : $1xN$
- "ket" $|b \rangle$ is a column vector : $Nx1$
- "bra" $\langle a|$  together with a "ket" $|b \rangle$  yields a "bracket" $\langle a|b \rangle$

# Single System

## Classical System

- Deterministic system

- Stochastic matrix
    - Probability of state transition for classical system
    - All entries are non-negative
    - Entries in each column sum to 1


## Quantum System

- The allowable operations on a quantum system are unitary operators

- Unitary matrix
    - Probability of state transition for quantum system
    - All entries are complex numbers
    - **absolute values squared** entries in each column sum to 1

- Born Rule
    - Measurement always collapse the state to one of the basis states
    - Measured probability is the absolute value squared of the amplitude of the state in the basis state


- Plus state
    - $|+\rangle = \frac{1}{\sqrt{2}}(|0\rangle + |1\rangle)$
    - $|+\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}1\\1\end{pmatrix}$
- Minus state
    - $|-\rangle = \frac{1}{\sqrt{2}}(|0\rangle - |1\rangle)$
    - $|-\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}1\\-1\end{pmatrix}$

## Unitary operators

- Operators not changing the Euclidean norm of the vector

- Identity
    - $U^{\dagger} = \bar{U^T} = U^{-1} = U^{*T}$
    - $U^{\dagger}U = I$

## Composition of Unitary operators

- $U_1U_2$ is also a unitary operator


# Multiple System

## Classical System

- Cartesian product of the subsystems
    - $|\pi \rangle = |\phi \rangle \otimes |\psi \rangle$
    - $\otimes$ (the *tensor product*) often omitted
- $\langle ab|\pi \rangle = \langle a|\phi \rangle \langle b|\psi \rangle$

## Tensor product



### Independent operations

- $P(A,B) = P(A)P(B)$
- Tensor product as the operator on the compound system
    - If $U_1, U_2$ are the probability operators on the subsystems $S1, S2$
    - Then $U_1 \otimes U_2$ is the probability operator on the compound system $(S1, S2)$

### Partial measurement

- Reduced Probability
    - $P(X=a) = \sum_{b}P((X,Y)=(a,b))$
- Conditional Probability
    - $P(Y=b|X=a) = \frac{P((X,Y)=(a,b))}{P(X=a)}$

- $P(A|B) = \frac{P(A,B)}{P(B)}$


## Quantum System

### Entangled state

- Not a product state
    - $|\pi \rangle \neq |\phi \rangle \otimes |\psi \rangle$
    
### Measurement

- Inner product
    - $\langle \phi | \psi \rangle = \sum_{i=1}^{n} \phi_i^* \psi_i$


# Quantum Circuit

## Inner product and Projection

### Projection metric


### Projective measurement

- Collection of projectors
    - $\sum_{k=1}^{m}M_k=\mathbb{1_n}\hspace{0.5em},\hspace{0.5em}m<=n$
    - $n$ is the number of classical states
- Probability
    - $P(|\phi \rangle) = ||M_k | \psi \rangle||^2$
- Post-measurement state
    - $|\psi \rangle = \frac{M_k | \psi \rangle}{||M_k | \psi \rangle||}$

- [TODO] Implementing projective measurements using standard basis measurements
    - Quantum circuithttps://learn.qiskit.org/course/basics/quantum-circuits#quantum-15-0:~:text=Implementing%20projective%20measurements%20using%20standard%20basis%20measurements

## Quantum state properties

- No-cloning theorem
    - It is impossible to copy an arbitrary quantum state
    - Does not exist a unitary operator $U$ such that
    - $U(|\phi \rangle \otimes |\pi \rangle) = |\phi \rangle \otimes |\phi \rangle , \hspace{0.5em} \forall |\phi \rangle \in X$