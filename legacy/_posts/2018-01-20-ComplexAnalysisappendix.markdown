---



layout: post



title :  (Complex Analysis) Appendix



date : 2018-01-20 09:52:04 +0900



---

(Appendix A) Asymptotics

(subsection 1) Bessel functions

(Def) For all order \nu > -1/2, J_{\nu}(s) = \frac{(s/2)^{\nu}}{\Gamma(\nu + 1/2) \Gamma(1/2)} \int_{-1}^{1} e^{isx} (1-x^{2})^{\nu – 1/2} dx.

If we also write J_{-1/2}(s) for \lim_{v\to-1/2} J_{\nu}(s) , it equals \sqrt{\frac{2}{\pi s}} cos s; . J_{1/2}(s) = \sqrt{\frac{2}{\pi s}} sin s.

(Thm 1.1.) J_{\nu}(s) = \sqrt{2}{\pi s} cos (s- \frac{\pi \nu}{2} - \frac{\pi}{4}) + O(s^{-3/2}) as s \to \infty.

(Prop 1.2.) Suppose a and m are fixed, with a >0 and m > -1. Then as s \to \infty \int_{0}^{a} e^{-sx} x^{m} dx = s^{-m-1} \Gamma(m+1) + O(e^{-cs}), for some positive c.

(Prop 1.3.) Suppose a and m are fixed, with a >0 and -1<m<0. Then as |s| \to \infty with Re(s) \ge 0, \int_{0}^{a} e^{-sx} x^{m} dx = s^{-m-1} \Gamma(m+1) + O(1/|s|). (Here s^{-m-1} is the branch of that function that is positive for s >0.)

(subsection 2) Laplace’s method ; Stirling’s formula

(Def) Consider \int_{a}^{b} e^{-s\Phi(x)} \psi(x) dx where the phase \Phi is real-valued, and both it and the amplitude \psi are assumed for simplicity to be indefinitely differentiable. Our hypothesis regarding the minimum of \Phi is that there is an x_{0} \in (a,b) so that \Phi’(x_{0}) = 0, but \Phi”(x_{0}) >0 throughout [a,b].

(Prop 2.1.) Under the above assumptions, with s >0 and s \to \infty, \int_{a}^{b} e^{-s\Phi(x)}\psi(x) dx = e^{-s\Phi(x_{0})} [\frac{A}{s^{1/2}} + O(\frac{1}{s})], where A = \sqrt(2\pi) \frac{\psi(x_{0})}{(\Phi”(x_{0})^{1/2}}.

(Prop 2.2.) With the same assumptions on \Phi and \psi, the relation of (prop 2.1.) continues to hold if |s| \to \infty with Re(s) \ge 0.

(Def) The special case of (Prop 2.2.) When s is purely imaginary, s = it, t \to \mp \infty , is often treated separately; the argument in this situation is usually referred to as the method of stationary phase. The points x_{0} for which \Phi’(x_{0}) = 0 are called the critical points.

(Thm 2.3.) If |s| \to \infty with s \in S_{\delta} , then \Gamma(s) = e^{s log s} e^{-s} \frac{\sqrt{2\pi}}{s^{1/2}} (1+ O(\frac{1}{|s|^{1/2}}) ).

(subsection 3) The Airy function

(Def) The Airy function Ai is defined by Ai(s) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{i(x^{3}/3+sx)}dx , with s \in \mathbb{R}.

Ai”(s) = s Ai(s).

(Thm 3.1.) Suppose u >0. Then as u \to \infty, 

Ai(-u) = \pi^{-1/2} u^{-1/4} cos(\frac{2}{3} u^{3/2} - \frac{\pi}{4})(1+O(1/u^{3/4})).

Ai(u) = \frac{1}{2\pi^{1/2}} u^{-1/4} e^{-\frac{2}{3} u^{3/2}} (1+ O(1/u^{3/4})).

(De) Assume F(z) is holomorphic. We seek a contour \Gamma so that 

Im(F) = 0 on \Gamma.

Re(F) has a minimum on \Gamma at some point z_{0}, and this function is non-degenerate in the sense that the second derivative of Re(F) along \Gamma is strictly positive at z_{0}.

If as above, F”(z_{0}) \neq 0, then there are two curves \Gamma_{1} and \Gamma_{2} passing through z_{0} which are orthogonal, so that F|_{\Gamma}, is real for i = 1,2, with Re(F) restricted to \Gamma_{1} having a minimum at z_{0}; and Re(F) restricted to \Gamma_{2} having a maximum at z_{0} . We try to deform out original contour of integration to \Gamma = \Gamma_{1}. This approach is usually referred to as the method of steepest descent.

(subsection 4) The partition function

(Thm 4.1.) If p denotes the partition function, then 

p(n)~ \frac{1}{4\sqrt{3} n} e^{Kn^{1/2}} as n \to \infty, where K = \pi \sqrt{\frac{2}{3}}.

A much more precise assertion is that p(n) = \frac{1}{2\pi \sqrt{2}} \frac{d}{dn} (\frac{e^{K(n-\frac{1}{24})^{1/2}}}{(n-\frac{1}{24})^{1/2}}) + O(e^{\frac{K}{2} n^{1/2}}).

(Appendix B) Simple Connectivity and Jordan Curve Theorem

(subsection 1) Equivalent formulations of simple connectivity

(Thm 1.1.) A region \Omega is holomorphically simply connected iff \Omega is simply connected.

(Thm 1.2.) If \Omega is a bounded region in \mathbb{C}, then \Omega is simply connected iff the complement of \Omega is connected.

(Def) The winding number of a closed curve \gamma around a point z \notin \gamma is W_{\gamm}(z) = \frac{1}{2\pi i} \int_{\gamma} \frac{d\zeta}{\zeta - z}. Sometimes, W_{\gamma}(z) is also called the index of z with respect to \gamma.

(Lem 1.3.) Let \gamma be a closed curve in \mathbb{C}.

If z \notin \gamma, then W_{\gamma}(z) \in \mathbb{Z}.

If z and w belong to the same open connected component in the complement of \gamma, then W_{\gamma}(z) = W_{\gamma}(w).

If z belongs to the unbounded connected component in the complement of \gamma, then W_{\gamma}(z) = 0.

(Thm 1.4.) A bounded region \Omega is simply connected iff W_{\gamma}(z) = 0 for any closed curve \gamma in \Omega and any point z not in \Omega.

(Lem 1.5.) Let w be any point in F_{1}. Under the above assumptions. there exists a finite collection of closed squares \mathcal{Q} = {Q_{1},…,Q_{n}} that belong to a uniform grid \mathcal{G} of the plane, and are such that:

w belongs to the interior of Q_{1}.

The interiors of Q_{j} and Q_{k} are disjoint when j \neq k.

F_{1} is contained in the interior of \cup_{j=1}^{n} Q_{j}.

\cup_{j=1}^{n} Q_{j} is disjoint from F_{2}.

The boundary of \cup_{j=1}^{n} Q_{j} lies entirely in \Omega, and consists of a finite union of disjoint simple closed polygonal curves.

(subsection 2) The Jordan curve theorem

(Thm 2.1.) Let \Gamma be curve in the plane that is simple and piecewise smooth. Then, the complement of \Gamma is an open connected set whose boundary is precisely \Gamma.

(Thm 2.2.) Let \Gamma be a curve in the plane which is simple, closed, and piecewise-smooth. Then, the complement of \Gamma consists of two disjoint connected open sets. Precisely one of these regions is bounded and simply connected; it is called the interior of \Gamma and denoted by \Omega. The other component is unbounded, called the exterior of \Gamma, and denoted by \mathcal{U}. Moreover, with the appropriate orientation for \Gamma, we have W_{\Gamma}(z) = \begin{cases} 1 & if z \in \Omega \\ 0 & if z \in \mathcal{U}\end{cases}.

(Thm 2.3.) Suppose f is a function that is holomotphic in the interior \Omega of a simple closed curve \Gamma. Then \int_{\eta} f(\zeta) d \zeta = 0 whenever \eta is any closed curve contained in \Omega.

(prop) recall that an arc-length parametrization \gamma for a smooth curve \Gamma_{0} satisfies |\gamma’(t)| = 1 for all t. Every smooth curve has an arc-length parametrization.

(Lem 2.4.) Let \Gamma_{0} be a simple smooth curve with an arc-length parametrization given by \gamma : [0,L] \to \mathbb{C}. For each real number \epsilon, Let \Gamma_{\epsilon} be the continuous curve defined by the parametrization \gamma_{\epsilon} (t) = \gamma(t) + i\epsilon \gamma’(t) , for 0 \le t \le L. Then, there exists \kappa_{1}>0 so that \Gamma_{0} \cap \Gamma_{\epsilon} = \empty whenever 0 < |\epsilon| < \kappa_{1}.

(Lem 2.5.) Suppose z is a point which does not belong to the smooth curve \Gamma_{0}, but that is closer to an interior point of the curve than to either of its end-points. Then z belongs to \Gamma_{\epsilon} for some \epsilon \neq 0. More precisely, if z_{0} \in \Gamma_{0} is closest to z and z_{0} = \gamma(t_{0}) for some t_{0} in the open interval (0,L) , then z = \gamma(t_{0}) + i\epsilon \gamma’(t_{0}) for some \epsilon \neq 0.

(prop 2.6.) Let A and B denote the two end-points of a simple smooth curve \Gamma_{0}, and suppose that K is a compact set that satisfies either \Gamma_{0} \cap K = \empty or \Gamma_{0} \cap K = A \cup B. If z \notin \Gamma_{0} and w \notin \Gamma_{0} lie on the same side of \Gamma_{0}, and are closer to interor points of \Gamma_{0} than they are to K or to the end-points of \Gamma_{0}, then z and w can be joined by a continuous curve that lies entirely in the complement of K \cup \Gamma_{0}.

(Lem 2.7.) Let \Gamma_{0} be a simple smooth curve. There exists \kappa_{2} >0 so that the set N, which consists of points of the form z = \gamma(L) + \epsilon e^{i\theta} \gamma’(L) with -\pi/2 \ge \theta \ge \pi/2 and 0 < \epsilon < \kappa_{2} , is disjoint from \Gamma_{0}.

(Prop 2.8.) Let A denote an end-point of the simple smooth curve \Gamma_{0}, and suppose that K is a compact set that satisfies either \Gamma_{0} \cap K = \empty or \Gamma_{0} \cap K = A. If z \notin \Gamma_{0} and w \notin \Gamma_{0} are closer to inerior points of \Gamma_{0} than they are to K or to the end-points of \Gamma_{0}, then z and w can be joined by a continuous curve that lies entirely in the complement of \Gamma_{0} \cap K.

(Thm 2.9.) If a function f is holomorphic in an open set that contains a simple closed piecewise-smooth curve \Gamma and its interior, then \int_{\Gamma} f = 0. 

(Lem 2.10) Let \gamma : [0,1] \to \mathbb{C} be a simple smooth curve. Then, for all sufficiently small \delta >0 the circle C_{\delta} centered at \gamma(0) and of radius \delta intersects \gamma in precisely one point.







