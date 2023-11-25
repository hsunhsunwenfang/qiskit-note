
\documentclass{article}
\usepackage[hybrid]{markdown}
\begin{document}

\begin{markdown}

# 8.04

## Wave Equation

- $u_{tt} = c^2 u_{xx}$

## Superposition Principle

- $u(x,t) = f(x-ct) + g(x+ct)$

## Fourier Transform

- If f(x) is localized, $\tilde{f}(\omega)$ is spread out
- Mathematically
    - Any f(t) is the superposition of plane waves $e^{i\omega t}$
    - $f(x) = \int_{-\infty}^{\infty} \tilde{f}(\omega) e^{i\omega t} d\omega$
    - Inverse: $\tilde{f}(\omega) = \frac{1}{2\pi} \int_{-\infty}^{\infty} f(x) e^{-i\omega t} dt$
- Physically
    - Any f(t) is the superposition of plane waves $e^{i\omega t}$

## Fourier Transform of the Wave Equation

- Superposition of plane waves -> momentum
    - $u(x,t) = \int_{-\infty}^{\infty} \tilde{u}(\omega) e^{i\omega t} d\omega$
- Superposition of delta function -> position
    - $u(x,t) = \int_{-\infty}^{\infty} \tilde{u}(\omega) \delta(\omega - ck) e^{i\omega t} d\omega$


## Noether's Theorem

- Symmetry -> Conservation Law
    - x translation -> momentum conservation
    - t translation -> energy conservation
    - rotation -> angular momentum conservation
    - $x \rightarrow x + \epsilon$ -> $p \rightarrow p$
    - $t \rightarrow t + \epsilon$ -> $E \rightarrow E$
    - $x \rightarrow x + \epsilon$ -> $L \rightarrow L$




## Uncertainty and Expectation

- Definition
    - Expectation
        - $\langle \hat A \rangle = \int \psi^* \hat A \psi dx$
    - Uncertainty
        - $\Delta A = \sqrt{\langle \hat A^2 \rangle - \langle A \rangle^2}$

- Uncertainty Principle
    - $\Delta\omega\Delta t\gtrsim 1$
    - $\Delta E\Delta t\gtrsim \hbar$


## Operator

### Commutator


- $[\hat A, \hat B] = \hat A \hat B - \hat B \hat A$
- $[\hat X, \hat P] = i \hbar \mathbb{I}$


## Eigenvalue and Eigenfunction

- Definition
    - $\hat A \psi = a \psi$

- Measurement
    - $\hat A \psi = a \psi$
    - Measured value
        - $\langle \hat A \rangle = \int \psi^* \hat A \psi dx = a$
    - Collapse
        - $\psi \rightarrow \psi_a = \frac{\hat A \psi}{\sqrt{\langle \hat A \rangle}}$