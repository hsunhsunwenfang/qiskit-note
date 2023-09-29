

# Matrix Methamatics

## Latex Library

- $$V_{sphere} = \frac{4}{3}\pi r^3$$
- $$<a_{jj}|$$

## Dirac Notation

- "bra" $<a|$ is a row vector : $1xN$
- "ket" $|b>$ is a column vector : $Nx1$
- "bra" $<a|$  together with a "ket" $|b>$  yields a "bracket" $<a|b>$
- $P(|0\rangle) = |\langle 0|\psi\rangle|^2$

## Matrix About

- Matrix Multiplication Example
$$M1=\begin{pmatrix}1 & 1\\0 & 0\end{pmatrix}\hspace{0.5em},\hspace{0.5em}M2=\begin{pmatrix}0 & 1\\1 & 0\end{pmatrix}$$
$$M1M2=\begin{pmatrix}1 & 1\\0 & 0\end{pmatrix}\hspace{0.5em},\hspace{0.5em}M2M1=\begin{pmatrix}1 & 1\\0 & 0\end{pmatrix}$$

# Single System

## Classical System

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

- Identity
    - $U^{\dagger} = \bar{U^T}$
    - $U^{\dagger}U = I$
    - $U^{\dagger} = U^{-1}$
    - $U^{\dagger} = U^{*T}$

- Pauli operations
    - $\alpha_X = \begin{pmatrix}0 & 1\\1 & 0\end{pmatrix}$
        - flip bit | NOT
    - $\alpha_Y = \begin{pmatrix}0 & -i\\i & 0\end{pmatrix}$
        - flip bit and phase | Y gate
    - $\alpha_Z = \begin{pmatrix}1 & 0\\0 & -1\end{pmatrix}$
        - phase flip | Z gate

- Hadamard
    - $H = \frac{1}{\sqrt{2}}\begin{pmatrix}1 & 1\\1 & -1\end{pmatrix}$
    - $H|0\rangle = |+\rangle$
    - $H|1\rangle = |-\rangle$
    - $H|+\rangle = |0\rangle$
    - $H|-\rangle = |1\rangle$

- Phase
    - $P_{\theta} = \begin{pmatrix}1 & 0\\0 & e^{i\theta}\end{pmatrix}$
    - $S = P_{\frac{\pi}{2}} = \begin{pmatrix}1 & 0\\0 & i\end{pmatrix}$
    - $S|0\rangle = |0\rangle$
    - $S|1\rangle = i|1\rangle$
    - $S|+\rangle = |+\rangle$
    - $S|-\rangle = -|-\rangle$

# Multiple System

## Classical System