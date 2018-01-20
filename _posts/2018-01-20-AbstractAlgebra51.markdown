---



layout: post



title : [Abstract Algebra] CSeparable Extensions



date : 2018-01-20 14:53:34 +0900



---

(Section 51) Separable Extensions

(subsection) Multiplicity of Zeros of a Polynomial

(Def 51.1) Let f(x) \in F[x]. An element \alpha of \bar{F} s.t. f( \alpha ) = 0 is a zero of f(x) of multiplicity \nu if \nu is the greatest integer s.t. (x- \alpha )^{\nu} is a factor of f(x) in \bar{F} [x].

(Thm 51.2) Let f(x) be irreducible in F[x]. Then all zeros of f(x) in \bar{F} have the same multiplicity.

(Cor 51.3) If f(x) is irreducible in F[x], then f(x) has a factorization in F[x] of the form a \prod_{i} (x- \alpha_{i} )^{\nu} , where the \alpha_{i} are the distinct zeros of f(x) in \bar{F} and a \in F.

(prop) {F(\alpha ) : F } is the number of distinct zeros of irr( \alpha , F).

(Thm 51.6) If E is a finite extension of F, then {E : F} divides [E : F].

(subsection) Separable Extensions

(Def 51.7) A finite Extension E of F is a separable extension of F if {E : F} = [E : F] . An element \alpha of \bar{F} is separable over F if F( \alpha ) is a separable extension of F. An irreducible polynomial f(x) \in F[x] is separable over F if every zero of f(x) in \bar{F} is separable over F.

(Thm 51.9) If K is a finite extension of E and E is a finite extension of F , that is F \le E \le K, then K is separable over F iff K is separable over E and E is separable over F.

(Cor 51.10) If E is a finite extension of F, then E is separable over F iff each \alpha in E is separable over F.

(subsection) Perfect Fields

(Lem 51.11) Let \bar{F} be an algebraic closure of F, and let f(x) = x^{n} + a_{n-1} x^{n-1} + \cdots + a_{1} x + a_{0} be any monic polynomial in \bar{F} [x] . If (f(x))^{m} \in F[x] and m \cdot 1 \neq 0 in F, then f(x) \in F[x] , that is, all a_{i} \in F.

(Def 51.12) A field is perfect if every finite extension is a separable extension.

(Thm 51.13) Every field of characteristic zero is perfect.

(Thm 51.14) Every finite field is perfect.

(subsection) Primitive element theorem

(Primitive element theorem) (Thm 51.15) Let E be a finite separable extension of a field F. Then there exists \alpha \in E s.t. F = F(\alpha) . (Such an element \alpha is a primitive element.)

 That is, a finite separable extension of a field is a simple extension.

(Cor 51.16) A finite extension of a field of characteristic zero is a simple extension.

