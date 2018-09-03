---



layout: post



title : (Abstract Algebra) Automorphisms and Galois Theory



date : 2018-01-20 14:53:04 +0900



---

(Section X) Automorphisms and Galois Theory

(Section 48) Automorphisms of Fields.

(subsection) The conjugation isomorphisms of Algebraic Field Theory

(Def) all algebraic extensions and all elements algebraic over a field F under consideration are contained in one fixed algebraic closure \bar{F} of F.

(Def 48.1) Let E be an algebraic extension of a field F. Two elements \alpha , \beta \in E are conjugate over F if irr( \alpha , F ) = irr ( \beta , F ) , that is, if \alpha and \beta are zeros of the same irreducible polynomial over F.

(The Conjugation Isomorphisms) (Thm 48.3) Let F be a field, and let \alpha and \beta be algebraic over F with deg ( \alpha , ) = n. The map \psi_{\alpha , \beta } : F( \alpha ) \to F( \beta ) defined by \psi_{\alpha , \beta } (c_{0} + c_{i} \alpha + \cdots + c_{n-1} \alpha^{n-1} ) = c_{0} + c_{1} \beta + \cdots + c_{n-1} \beta^{n-1} for c_{i} \in F is an isomorphism of F( \alpha ) onto F( \beta ) iff \alpha and \beta are conjugate over F.

(Cor 48.5) Let \alpha be algebraic over a field F. Every isomorphism \psi mapping F( \alpha ) onto a subfield of \bar{F} s.t. \psi (a) = a for a \in F maps \alpha onto a conjugate \beta of \alpha over F. Conversely, for each conjugate \beta of \alpha over F, there exists exactly one isomorphism \psi_{\alpha , \beta } of F( \alpha ) onto a subfield of \bar{F} mapping \alpha onto \beta and mapping each a \in F onto itself.

(Cor 48.6) Let f(x) \in \mathbb{R} [x] . If f(a + bi) = 0 for (a + bi) \in \mathbb{C}, where a, b \in \mathbb{R}, then f(a – bi) = 0 also. Loosely, complex zeros of polynomials with real coefficient occur in conjugate pairs.

(subsection) Automorphisms and Fixed Fields

(Def 48.8) An isomorphism of a field into itself is an automorphism of the field.

(Def 48.9) If \sigma is an isomorphism of a field E onto some field, then an element a of E is left fixed by \sigma if \sigma (a) = a. A collection S of isomorphisms of E leaves a subfield F of E fixed if each a \in F is left fixed by every \sigma \in S. If { \sigma } leaves F fixed, then \sigma leaves F fixed.

(Thm 48.11) Let \\( \lbrace \sigma_{i}  \vert i \in I \rbrace  \\) be a collection of automorphisms of a field E. Then the set \\(E_{\lbrace \sigma_{i} \rbrace }\\) of all a \in E left fixed by every \sigma_{i} for i \in I forms a subfield of E.

(Def 48.12) The field \\(E_{\lbrace \sigma_{i} \rbrace }\\)  of (Thm 48.11) is the fixed field of \\( \lbrace \sigma_{i}  \vert i \in I \rbrace  \\) . For a single automorphism \sigma, we shall refer to E_{ {\sigma } } as the fixed field of \sigma.

(Thm 48.14) The set of all automorphisms of a field E is a group under function composition.

(Thm 48.15) Let E be a field, and let F be a subfield of E, Then the set G( E/F) of all automorphisms of E leaving F fixed forms a subgroup of the group of all automorphisms of E. Furthermore, F \le E_{ G(E/F) } .

(Def 48.16) The group G(E/F) of the preceding theorem is the group of automorphisms of E leaving F fixed, or more briefly, the group of E over F.

(subsection) The Frobenius Automorphism

(Thm 48.19) Let F be a finite field of characteristic p. Then the map \sigma_{p} : F \to F defined by \sigma_{p} (a) = a^{p} for a \in F is an automorphism, the Frobenius automorphism, of F. Also, F_{ \sigma_{p} } \simeq \mathbb{Z}_{p} .

