---



layout: post



title : Cauchy’s Theorem and Its Applications



date : 2018-01-20 09:52:04 +0900



---

(Section 2) Cauchy’s Theorem and Its Applications

(subsection 1) Goursat’s Thm

(prop) If f has a primitive in an open set \Omega, then \int_{\gamma} f(z) dz = 0 for any closed curve \gamma in \Omega. Conversely, if we can show that the above relation holds for some types of curves \gamma, then a primitive will exist.

(Thm 11.1.) If \Omega is an open set in \mathbb{C}, and T \subset \Omega a triangle whose interior is also contained in \Omega, then \int_{T} f(z) dz = 0 whenever f is holomorphic in \Omega.

(Cor 1.2.) If f is holomorphic in an open set \Omega that contains a rectangle R and its interior, then \int_{R} f(z) dz = 0.

(subsection 2) Local existence of primitives and Cauchy’s theorem in a disc

(Thm 2.1.) A holomorphic function in an open disc has a primitive in that disc.

(Cauchy’s theorem for a disc) (Thm 2.2.) If f is holomorphic in a disc, then \int_{\gamma} f(z) dz = 0 for any closed curve \gamma in that disc.

(Cor 2.3.) Suppose f is holomorphic in an open set containing the circle C and its interior, Then \int_{C} f(z) dz = 0.

(Def) We call a toy contour any closed curve where the notion of interior is obvious, and a construction similar to that in (Thm 2.1.) is possible in a neighborhood of the curve and its interior. Its positive orientation is that for which the interior is to the left as we travel along the toy contour.

(Def) Keyhole \Gamma . It consists of two almost complete circles one large and one small, connected by a narrow corridor. The interior of \Gamma, which we denote by \Gamma_{int}, is clearly that region enclosed by the curve.

(Prop) For a toy contour \gamma we have that \int_{\gamma} f(z)dz = 0, whenever f is holomorphic in an open set that contains the contour \gamma and its interior.

(subsection 4) Cauchy’s integral formulas

(Thm 4.1.) Suppose f is holomorphic in an open set that contains the closure of a disc D. If C denotes the boundary circle of this disc with the positive orientation, then f(z) = \frac{1}{2\pi i} \int_{C} \frac{f(\zeta)}{\zeta - z} d\zeta for any point z \in D.

(Prop) If f is holomorphic in an open set that contains a (positively oriented) rectangle R and its interior, then f(z) = \frac{1}{2\pi i} \int_{R} \frac{f(\zeta)}{\zeta - z} d\zeta whenever z belongs to the interior of R.

(Cor 4.2.) If f is holomorphic in an open set \Omega, then f has infinitely many complex derivatives in \Omega. Moreover, if C \subset \Omega is a circle whose interior is also contained in \Omega, then f^{(n)} (z) = \frac{n!}{2\pi i} \int_{C} \frac{f(\zeta)}{(\zeta – z)^{n+1}} d \zeta for all z in the interior of C.

(Cauchy inequalities) (Cor 4.3.) If f is holomorphic in an open set that contains the closure of a disc D centered at z_{0} and of radius R, then |f^{(n)} (z_{0})| \le \frac{n!\Vert f \Vert_{C}}{R^{n}} where \Vert f \Vert_{C} = \sup_{z \in C}|f(z)| denotes the supremum of |f| on the boundary circle C.

(Thm 4.4.) Suppose f is holomorphic in an open set \Omega. IF D is a disc centered at z_{0} and whose closure is contained in \Omega, then f has a power series expansion at z_{0} f(z) = \sum_{n = 0}^{\infty} a_{n} (z-z_{0})^{n} for all z \in D, and the coefficients are given by a_{n} = \frac{f^{(n)} (z_{0})}{n!} for all n \ge 0.

(Liouville’s theorem) (Cor 4.5.) If f is entire and bounded, then f is constant.

(Cor 4.6.) Every non-constant polynomial P(z) = a_{n}z^{n} + \cdot + a_{0} with complex coefficients has a root in \mathbb{C}.

(Cor 4.7.) Every polynomial P(z) = a_{n}z^{n} + \cdots + a_{0} of degree n \ge 1 has precisely n roots in \mathbb{C}. If these roots are denoted by w_{1}, …, w_{n}, then P can be factored as P(z) = a_{n}(z-w_{1})(z-w_{2})\cdot(z-w_{n}).

(Thm 4.8.) Suppose f is a holomorphic function in a region \Omega that vanishes on a sequence of distinct points with a limit point in \Omega. Then f is identically 0.

(Cor 4.9) Suppose f and g are holomorphic in a region \Omega and f(z) = g(z) for all z in some non-empty open subset of \Omega (or more generally for z in some sequence of distinct points with limit points in \Omega). Then f(z) = g(z) throughout \Omega.

(subsection 5) Further applications

(subsubsection 5.1.) Morera’s Theorem

(Thm 5.1.) Suppose f is a continuous function in the open disc D s.t. for any triangle T contained in D \int_{T} f(z)dz = 0, then f is holomorphic.

(subsubsection 5.2.) Sequences of holomorphic functions

(Thm 5.2.) If {f_{n}}_{n=1}^{\infty} is a sequence of holomorphic functions that converges uniformly to a function f| in every compact subset of \Omega, then f is holomorphic in \Omega.

(Thm 5.3.) Under the hypotheses of the previous theorem, the sequence of derivatives {f’_{n}}_{n=1}^{\infty} converges uniformly to f’ on every compact subset of \Omega.

(subsubsection 5.3.) Holomorphic functions defined in terms of integrals

(Thm 5.4.) Let F(z,s) be defined for (z,s) \in \Omega \times [0,1] where \Omega is an open set in \mathbb{C}. Suppose F satisfies the following properties :

F(z,s) is holomorphic in z for each s.

F is continuous on \Omega \times [0,1].

Then the function f defined on \Omega by f(z) = \int_{0}^{1} F(z,s) ds is holomorphic.

(subsubseciton 5.4.) Schwarz reflection principle

(Def) Let \Omega be an open subset of \mathbb{C} that is symmetric with respect to the real line, that is z \in \Omega iff \bar{z} \in \Omega. Let \Omega^{+} denote the part of \Omega that lies in the upper half-plane and \Omega^{-} that part lies in the lower half-plane.

Let I = \Omega \cap \mathbb{R} so that I denotes the interior of that part of the boundary of \Omega^{+} and \Omega^{-} that lies on the real axis. Then we have \Omega^{+} \cap I \cap \Omega^{-} = \Omega .

(Symmetry Principle) (Thm 5.5.) If f^{+} and f^{-} are holomorphic functions in \Omega^{+} and \Omega^{-} respectively that extend continuously to I and f^{+}(x) = f^{-}(x) for all x \in I, then the function f defined on \Omega by f(z) = \begin{cases} f^{+}(z) & if z \in \Omega^{+} \\ f^{+}(z) = f^{-}(z) & if z \in I \\ f^{-}(z) & if z \in \Omega^{-}\end{cases} is holomorphic on all of \Omega.

(Schwarz reflection principle) (Thm 5.6.) Suppose that f is a holomorphic function in \Omega^{+} that extends continuously to I and s.t. f is real-valued on I. Then there exists a function F holomorphic in all of \Omega s.t. F = f on \Omega^{+}.

(subsubsection 5.5.) Runge’s approximation theorem

(Thm 5.7.) Any function holomorphic in a neighborhood of a compact set K can be approximated uniformly on K by rational functions whose singularities are in K^{c}.

If K^{c} is connected, any function holomorphic in a neighborhood of K can be approximated uniformly on K by polynomials.

(Lem 5.8.) Suppose f is holomorphic in an open set \Omega, and K \subset \Omega is compact. Then, there exists finitely many segments \gamma_{1}, …, \gamma_{N} in \Omega – K s.t. f(z) = \sum_{n = 1}^{N} \frac{1}{2\pi i} \int_{\gamma_{n}} \frac{f(\zeta)}{\zeta - z} d \zeta for all z \in K.

(Lem 5.9.) For any line segment \gamma entirely contained in \Omega – K , there exists a sequence of rational functions with singularities on \gamma that approximate the integral \int_{\gamma}f(\zeta) /(\zeta – z) d\zeta uniformly on K.

(Lem 5.10.) If K^{c} is connected and z_{0} \notin K, then the function 1/(z-z_{0}) can be approximated uniformly on K by polynomials.

