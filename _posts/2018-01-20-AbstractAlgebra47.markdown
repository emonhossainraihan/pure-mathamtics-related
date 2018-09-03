---



layout: post



title : (Abstract Algebra) Gaussian integers and multiplicative Norms



date : 2018-01-20 14:52:54 +0900



---

(Section 47) Gaussian integers and multiplicative Norms

(subsection) Gaussian Integers

(Def 47.1) A Gaussian integer is a complex number a + bi, where a, b \in \mathbb{Z}. For a Gaussian integer \alpha = a + bi, the norm N(\alpha) of \alpha is a^{2} + b^{2}.

(Lem 47.2) In \mathbb{Z} [i], the following properties of the norm function N hold for all \alpha , \beta \in \mathbb{Z} [i].

N(\alpha ) \ge 0.

N(\alpha ) = 0 iff \alpha = 0.

N(\alpha \beta ) = N(\alpha ) N(\beta )

(Lem 47.3) \mathbb{Z} [i] is an integral domain.

(Lem 47.4) The function \nu is given by \nu (\alpha ) = N( \alpha ) for nonzero \alpha \in \mathbb{Z} [i] is a Euclidean norm on \mathbb{Z} [i] . Thus \mathbb{Z} [i] is a Euclidean domain.

(subsection) Multiplicative Norms

(Def 47.6) Let D be an integral domain. A multiplicative norm N on D is a function mapping D into the integers \mathbb{Z} s.t. the following conditions are satisfied.

N(\alpha ) = 0 iff \alpha = 0

N( \alpha \beta ) = N( \alpha ) N( \beta ) for all \alpha , \beta \in D.

(Thm 47.7) If D is an integral domain with a multiplicative norm N, then N(1) = 1 and | N(u) | = 1 for every unit u in D. If, furthermore, every \alpha s.t. | N(\alpha ) | = 1 is a unit in D, then an element \pi in D, with | N(\pi) | = p for a prime p \in \mathbb{Z} , is an irreducible of D.

(Fermat’s p = a^{2} + b^{2} Theorem) (Thm 47.10) Let p be an odd prime in \mathbb{Z}. Then p = a^{2} + b^{2} for integers a and b in \mathbb{Z} iff p \equiv 1 \pmod{4} .

