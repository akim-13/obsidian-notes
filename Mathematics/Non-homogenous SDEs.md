# Non-homogenous SDEs

* A **non-homogenous SDE** is an [[./Second-order Differential Equations (SDEs).md|SDE]] of the form:
$$ f(y'', y', y) = g(x) $$

* A **linear non-homogenous SDE** has the following form:
$$
a\frac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}} +
b\frac{\mathrm{d}y}{\mathrm{d}x} + cy = f(x),\ \text{where constants } a, b, c \in
\mathbb{R} \tag{1}
$$ 

* **Complementary function (C.F.)** of a non-homogenous SDE is its corresponding [[./Homogenous SDEs.md|homogenous SDE]]. For example, the C.F. of (1) is:
$$
a\frac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}} + b\frac{\mathrm{d}y}{\mathrm{d}x} + cy = 0 \tag{2}
$$
The general solution of the C.F. is called the **complementary solution (C.S.)**.

* **Particular integral (P.I.)** is a function that satisfies the original differential equation. For (1), the form of a P.I. will depend on $f(x)$, and is supposed to be "guessed". In the A-Level course, most of the time P.I will have one of the following forms:
    1) $\lambda$
    2) $\lambda + \mu x$
    3) $\lambda + \mu x + \nu x^{2}$
    4) $\lambda e^{kx}$
    5) $\lambda \cos{kx} +\mu \sin{kx}$,

    where $\lambda, \mu,$ and $\nu$ are the coefficients to be found by equating them to the corresponding coefficients of $f(x)$.

* **To find the general solution** of a linear non-homogenous SDE (1):
    1) Solve $a\frac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}} + b\frac{\mathrm{d}y}{\mathrm{d}x} + cy=0$ to find the C.S.
    2) Find a P.I. by guessing its form, and equating the coefficients to the coefficient of $f(x)$
    3) $y = \text{C.S.} + \text{P.I.}$

To prove that this method works, let $\hat y$ be the C.S. of (1), and $\tilde y$ the P.I. Then:

$$
\begin{align}
    &ay'' + by' + cy = f(x) \tag{1} \\
    &a\hat y'' + b\hat y' + c\hat y = 0 \tag{3} \\
    &a\tilde y'' + b\tilde y' + c\tilde y = f(x) \tag{4} \\
\end{align}
$$

If general solution $= \text{C.S} + \text{P.I.}$, then by substituting $y = \hat y + \tilde y\,$ in (1) we get:

$$
\begin{align}
    &a(\hat y + \tilde y)'' + b(\hat y + \tilde y)' + c(\hat y + \tilde y) \\
    = &(a\hat y'' + b\hat y' + c\hat y) + (a\tilde y'' + b\tilde y' + c\tilde y) \tag*{Expanded and rearranged} \\
    = &\textbf{(3)} + \textbf{(4)} \\
    = &0 + f(x) \\ 
    = &f(x) \implies y = \hat y + \tilde y\ \text{ satisfies (1)} \\
    & \tag*{QED}
\end{align}
$$

* It is possible to **solve non-linear** non-homogenous SDEs by a **substitution**^[Which is always given in the A-Level course.] (see **Q2**). **_It is extremely important to properly use the [[Chain Rule|chain rule]] for this kind of substitution!_**

---

**Q1:** Find the general solution of $\frac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}} - 8\frac{\mathrm{d}y}{\mathrm{d}x} + 12y= 36x$
**A:** 
1) Find the comlementary solution ([[./Homogenous SDEs.md#^solve-homogenous-sde|solving a homogenous SDE]]):
    $$ \frac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}} - 8\frac{\mathrm{d}y}{\mathrm{d}x} + 12y = 0 $$ 
    Auxiliary equation: $m^{2} - 8m +12 = 0 \implies m = \frac{8 \pm \sqrt{(-8)^{2}-4\times 12}}{2} 
    \implies m_1 = 2, m_2 = 6$
    C.S. $= y_c = Ae^{6x} + Be^{2x}$
2) Find a particular integral:
    RHS $= 36x \implies$ P.I. is of the form $\lambda + \mu x$, therefore let $y = \lambda + \mu x
    \implies y' = \mu \implies y'' = 0$. Substituting the values in the original equation:
    $$
    \begin{align}
        0 - 8 \mu + 12(\lambda + \mu x) = 36x \\
        (3 \lambda - 2 \mu) + 3 \mu x = 0 + 9x
    \end{align}
    $$
    Equating the coefficients:
    $$
    \begin{cases}
        3 \lambda - 2 \mu = 0 \\
        3 \mu = 9
    \end{cases}
    \iff
    \begin{cases}
        \lambda = 2 \\
        \mu = 3
    \end{cases}
    $$
    P.I. $= y_p = 2 + 3x$
3) $y = y_c + y_p = Ae^{6x} + Be^{2x} + 3x + 2$

*Answer:* $y = Ae^{6x} + Be^{2x} + 3x + 2$

---

**Q2:** 
**A:** 

*Answer:*
