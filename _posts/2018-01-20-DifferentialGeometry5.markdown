---



layout: post



title : \[Differential Geometry] Global Differential Geometry



date : 2018-01-20 12:56:04 +0900



---

(Section 5) Global Differential Geometry

(subsection 5.2.) The Rigidity of the Sphere

(Thm 1) Let S be a compact , connected, regular surface with constant Gaussian curvature K. Then S is a sphere.

(Lem 1) Let S be a regular surface and p \in S a point of S satisfying the following conditions :

K(p) >0 ; that is, the Gaussian curvature in p is positive.

p is simultaneously a point of local maximum for the function k_{1} an a point of local minimum for the function k_{2} (k_{1} \ge k_{2}) . 

Then p is an umbilical point of S.

(Thm 1a.) Let S be a regular, compact, and connected surface with Gaussian curvature K > 0 and mean curvature H constant. Then S is a sphere.

(Thm 1b) Let S be a regular, compact, and connected surface of positive Gaussian curvature. If there exists a relation k_{2} = f(k_{1}) in S, where f is a decreasing function of k_{1}, k_{1} \ge k_{2}, then S is a sphere.

(Lem 2) A regular compact surface S \subset R^{3} has at least one elliptic point.

(subsection 5.3.) Complete Surfaces . Theorem of Hopf-Rinow

(Def 1) A regular (connected) surface S is said to be extendable if there exists a regular (connected) surface \bar{S} s.t. S \subset \bar{S} as a proper subset. If there exists no such \bar{S}, S said to be nonextendable.

(Def 2) A regular surface S is said to be complete when for every point p \in S, any parametrized geodesic \gamma : [0, \epsilon) \to S of S, starting from p = \gamma(0) , may be extended into a parametrized geodesic \bar{\gamma} : R \to S, defined on the entire line R. In other words, S is complete when for every p \in S the mapping exp_{p} : T_{p} (S) \to S is defined for every v \in T_{p}(S).

(Prop 1) A complete surface S is nonextendable.

(Prop 2) Given two points p, q \in S of a regular(connected) surface S, there exists a parametrized piecewise differentiable curve joining p to q.

(Def 3) The (intrinsic) distance d(p,q) from the point p \in S to the point q \in S is the number d(p,q) = \inf 1(\alpha_{p,q}) , where the inf is taken over all piecewise differentiable curves joining p to q.

(Prop 3) The distance d defined above has the following properties.

d(p,q) = d(q,p),

d(p,q) + d(q,r) \ge d(p,r) ,

d(p,q) \ge 0,

d(p,q) = 0 iff p = q.

(Cor) |d(p,r) – d(r,q)| \le d(p,q).

(prop 4) If we let p_{0} \in S be a point of S, then the function f : S \to R given by f(p) = d(p_{0}, p) , p \in S, is continuous on S.

(prop 5) A closed surface S \subset R^{3} is complete.

(Cor) A compact surface is complete.

(Def) A geodesic \gamma joining two points p, q \in S is minimal if its length l(\gamma) is smaller than or equal to the length of any piecewise regular curve joining p to q. 

(Hopf-Rinow) (Thm) Let S be a complete surface. Given two points p, q \in S, there exists a minimal geodesic joining p to q.

(Cor 1) Let S be complete. Then for every point p \in S the map exp_{p} : T_{p}(S) \to S is onto S.

(Cor 2) Let S be complete and bounded in the metric d (that is, there exists r >0 s.t. d(p,q) < r for every pair p,q \in S). Then S is compact.

(subsection 5.4.) First and Second Variations of Arc length ; Bonnet’s Theorem

(Def 1) Let \alpha : [0,l] \to S be a regular parametrized curve, where the parameter s \in [0,l] is the arc length. A variation of \alpha is a differentiable map h : [0,l] \times (-\epsilon, \epsilon) \subset R^{2} \to S s.t. h(s,0) = \alpha(s), s \in [0,l] . For each t \in (-\epsilon, \epsilon) , the curve h_{t} : [0,l] \to S, given by h_{t}(s) = h(s,t), is called a curve of the variation h. A variation h is said to be proper if h(0,t) = \alpha(0) , h(l,t) = \alpha(l), t \in (-\epsilon, \epsilon).

(Def) A variation h of \alpha determines a differentiable vector field V(s) along \alpha by V(s) = \frac{\partial h}{\partial s}(s,0) , s \in [0,l] . V is called the variational vector field of h; If h is proper, then V(0) = V(l) = 0.

(prop 1) If we let V(s) be a differentiable vector field along a parametrized regular curve \alpha : [0,l] \to S then there exists a variation h : [0,l] \times (-\epsilon , \epsilon) \to S of \alpha s.t. V(s) is the variational vector field of h. Furthermore, if V(0) = V(l) = 0, then h can be chosen to be proper.

(Def) Define a function L : (-\epsilon, \epsilon) \to R by L(t) = \int_{0}^{l} |\frac{\partial h}{\partial s}(s,t)|ds, t \in (-\epsilon, \epsilon) . 

(Lem 1) The function L defined above is differentiable in a neighborhood of t= 0 ; in such a neighborhood , the derivative of L may be obtained by differentiation under the integral sign.

(Lem 2) Let w(t) be a differentiable vector field along the parametrized curve \alpha : [a,b] \to S and let f : [a,b] \to R be a differentiable function. Then \frac{D}{dt}(f(t)w(t)) = f(t) \frac{Dw}{dt} + \frac{df}{dt}w(t).

(Lem 3) Let v(t) and w(t) be differentiable vector fields along the parametrized curve \alpha : [a,b] \to S. Then \frac{d}{dt} \langle v(t), w(t) \rangle = \langle \frac{Dv}{dt},w(t) \rangle + \langle v(t), \frac{Dw}{dt} \rangle.

(Lem 4) Let h : [0,l] \times (-\epsilon, \epsilon) \subset R^{2} \to S be a differentiable mapping. Then \frac{D}{\partial s} \frac{\partial h}{\partial t} (s,t) = \frac{D}{\partial t} \frac{\partial h}{\partial s} (s,t).

(prop 2) Let h : [0,l] \times (-\epsilon, \epsilon) be a proper variation of the curve \alpha : [0,l] \to S and let V(s) = (\partial h / \partial t)(s,0) , s \in [0,l] , be the variational vector field of h. Then L’(0) = -\int_{0}^{l} \langle A(s) , V(s) \rangle ds, where A(s) = (D/\partial s) (\partial h / \partial s) (s,0).

(prop 3) A regular parametrized curve \alpha : [0,l] \to S , where the parameter s \in [0,l] is the arc length of \alpha , is a geodesic iff , for every proper variation h : [0,l] \times (-\epsilon , \epsilon) \to S of \alpha , L’(0) = 0.

(Lemma 5) Let x : U \to S be a parametrization at a point p \in S of a regular surface S, with parameters u,v, and let K be a Gaussian curvature of S. Then \frac{D}{\partial v}\frac{D}{\partial u} x_{u} - \frac{D}{\partial u}\frac{D}{\partial v}x_{u} = K(x_{u} \wedge x_{v}) \wedge x_{u}.

(Lem 6) Let h : [0,l] \times (-\epsilon, \epsilon) \to S be a differentiable mapping and let V(s,t) , (s,t) \in [0,l] \times (-\epsilon , \epsilon) , be a differentiable vector field along h. Then \frac{D}{\partial t}\frac{D}{\partial s} V - \frac{D}{\partial s}\frac{D}{\partial t}V = K(s,t)(\frac{\partial h}{\partial s} \wedge \frac{\partial h}{\partial t}) \wedge V, where K(s,t) is the curvature of S at the point h(s,t).

(Prop 4) Let h : [0,l] \times (-\epsilon , \epsilon) \to S be a proper orthogonal variation of a geodesic \gamma :[0,l] \to S parametrized by the arc length s \in [0,l] . Let V(s) = (\partial h/\partial t) (s,0) be the variational vector field of h. Then L’’(0) = \int_{0}^{t} (|\frac{D}{\partial s}V(s)|^{2} -K(s)|V(s)|^{2})ds where K(s) = K(s,0) is the Gaussian curvature of S at \gamma(s) = h(s,0).

(Bonnet)(Thm) Let the Gaussian curvature K of a complete surface S satisfy the condition K \ge \delta > 0 . Then S is compact and the diameter \rho of S satisfies the inequality \rho \le \frac{\pi}{\sqrt{\delta}} .

(subsection 5.5.) Jacobi Fields and Conjugate Points

(Def 1) Let \gamma : [0,l] \to S be a parametrized geodesic on S and let h : [0,l] \times (-\epsilon , \epsilon) \to S be a variation of \gamma s.t. for every t \in (-\epsilon , \epsilon) the curve h_{t}(s) = h(s,t) , s \in [0,l] , is a parametrized geodesic (not necessarily parametrized by arc length) . The variational field (\partial h/\partial h)(s,0) = J(s) is called a Jacobi field along \gamma.

(Prop 1) Let J(s) be a Jacobi field along \gamma : [0,l] \to S, s \in [0,l] . Then J satisfies the so-called Jacobi equation \frac{D}{ds}\frac{D}{ds}J(s) + K(s)(\gamma’(s) \wedge J(s)) \wedge \gamma’(s) = 0, where K(s) is the Gaussian curvature of S at \gamma(s).

(Lem 1) Let p \in S and choose v,w \in T_{p}(S), with |v| = l. Let \gamma:[0,l] \to S be the geodesic on S given by \gamma(s) = exp_{p}(sv) , s \in [0,l]. Then, the vector field J(s) along \gamma given by J(s) = s(d exp_{p})_{sv}(w) , s \in [0,l] , is a Jacobi field. Furthermore, J(0) = 0, (DJ/ds) (0) = w.

(Prop 2) If we let J(s) be a differentiable vector field along \gamma : [0,l] \to S, s \in [0,l] , satisfying the Jacobi equation with J(0) = 0, then J(s) is a Jacobi field along \gamma.

(Def 2) Let \gamma : [0,l] \to S be a geodesic of S with \gamma(0) = p. We say that the point q = \gamma(s_{0}) , s_{0} \in [0,l] , is conjugate to p relative to the geodesic \gamma (if there exists a Jacobi field J(s) which is not identically zero along \gamma with J(0) = J(s_{0}) = J(s_{0}) = 0.

(Prop 3) Let J_{1}(s) and J_{2}(s) be the Jacobi fields along \gamma : [0,l] \to S, s \in [0,l] . Then \langle \frac{DJ_{1}}{ds}, J_{2}(s) \rangle - \langle J_{1}(s) , \frac{DJ_{2}}{ds} \rangle = const.

(Cor) Let J(s) be a Jacobi field along \gamma : [0,l] \to S, with J(0) = J(l) = 0. Then \langle J(s) , \gamma’(s) \rangle = 0, s \in [0,l].

(Prop 5) Let p , q \in S be two points of S and let \gamma : [0,l] \to S be a geodesic joining p = \gamma(0) to q = exp_{p}(l\gamma’(0)) . Then q is conjugate to p relative to \gamma iff v = l\gamma’(0) is a critical point of exp_{p} : T_{p}(S) \to S.

(Thm) Assume that the Gaussian curvature K of a surface S satisfies the condition K \le 0. Then, for every p \in S. the conjugate locus of p is empty. In short, a surface of curvature K \le 0 does not have conjugate points.

(Cor) Assume the Gaussian curvature K of S to be negative or zero. Then for every p \in S, the mapping exp_{p} : T_{p}(S) \to S is a local diffeomorphism.

(Gauss) (Lem 2) Let p \in S be a point of a (complete) surface S and let u \in T_{p}(S) and w \in (T_{p}(S))_{u} . Then \langle u, w \rangle = \langle (d exp_{p})_{u}(u) , (d exp_{p})_{u}(w) \rangle , where the identification T_{p}(S) \approx (T_{p}(S))_{u} is being used.

(subsection 5.6.) Covering Spaces ; The Theorem of Hadamard

(subsubsection A) Covering Spaces

(Def 1) Let \tilde{B} and B be subsets of R^{3} . We say that \pi : \tilde{B} \to B is a covering map if \pi is continuous and \pi(\tilde{B}) = B.

Each point p \in B has a neighborhood U in B (to be called a distinguished neighborhood of p) s.t. \pi^{-1}(U) = \bigcup_{\alpha}V_{\alpha}, where the V_{\alpha}’s are pairwise disjoint open sets s.t. the restriction of \pi to V_{\pi} is a homeomorphism of V_{\alpha} onto U. \tilde{B} is then called a covering space of B.

(Prop 1) Let \pi : \tilde{B} \to B be a local homeomorphism, \tilde{B} compact and B connected. Then \pi is a covering map.

(Prop 2) Let \pi : \tilde{B} \to B be a coveing map, \alpha : [0,l] \to B an arc in B and \tilde{p}_{0} \in \tilde{B} a point of \tilde{B} s.t. \pi(\tilde{p}_{0}) = \alpha(0) = p_{0} . Then there exists a unique lifting \tilde{\alpha} : [0,l] \to \tilde{B} with origin at \tilde{p}_{0} , that is, with \tilde{\alpha}(0) = \tilde{p}_{0}.

(Def 2) Let B \subset R^{3} and let \alpha_{0} : [0,l] \to B, \alpha_{1} : [0,l] \to B be two arcs of B, joining the points p = \alpha_{0}(0) = \alpha_{1}(0) , q = \alpha_{0}(l)= \alpha_{1}(l). We say that \alpha_{0} and \alpha_{1} are homotopic if there exists a continuous map H : [0,l] \times [0,l] \to B s.t. H(s,0) = \alpha_{0}(s), H(s,1) = \alpha_{1}(s), s \in [0,l] . H(0,t) = p, H(l,t) = q, t \in [0,1]. The map H is called a homotopy between \alpha_{0} and \alpha_{1}.

(Def) Let \pi : \tilde{B} \to B be a continuous map and let \alpha_{0} , \alpha_{1} \to B be two arcs of B joining the points p and q. Let H : [0,l] \times [0,1] \to B be a homotopy between \alpha_{0} and \alpha_{1}. If there exists a continuous map \tilde{H} : [0,l] \times [0,1] \to \tilde{B} s.t. \pi \bullet \tilde{H} = H, we say that \tilde{H} is a lifting of the homotopy H, with origin at \tilde{H}(0,0) = \tilde{p} \in \tilde{B}.

(prop 3) Let \pi : \tilde{B} \to B be a local homeomorphism with the property of lifting arcs. Let \alpha_{0} , \alpha_{1} : [0,l] \to B be two arcs of B joining the points p and q. Let H : [0,l] \times [0,1] \to B be a homotopy between \alpha_{0} and \alpha_{1} , and let \tilde{p} \in \tilde{B} be a point of \tilde{B} s.t. \pi(\tilde{p}) = p. Then there exists a unique lifting \tilde{H} of H with origin at \tilde{p}.

(Prop 4) Let \pi : \tilde{B} \to B be a local homeomorphism with the property of lifting arcs. Let \alpha_{0} , \alpha_{1} : [0,l] \to B be two arcs of B joining the points p and q and choose \tilde{p} \in \tilde{B} s.t. \pi(\tilde{p}) = p. If \alpha_{0} and \alpha_{1} are homotopic, then the liftings \tilde{\alpha_{0}} and \tilde{\alpha_{1}} , of \alpha_{0} and \alpha_{1}, respectively, with origin \tilde{p} , are homotopic.

(Def 3) An arcwise connected set B \subset R^{3} is simply connected if given two points p, q \in B and two arcs \alpha_{0} : [0,l] \to B, \alpha_{1} : [0,l] \to B joining p to q, there exists a homotopy in B between \alpha_{0} and \alpha_{1} . In particular, any closed arc of B, \alpha:[0,l] \to B (closed means that \alpha(0) = \alpha(l) = p) , is homotopic to the constant arc \alpha(s) = p, s \in [0,l]

(Prop 5) Let \pi : \tilde{B} \to B be a local homeomorphism with the property of lifting arcs. Let \tilde{B} be arcwise connected and B simply connected. Then \pi is a homeomorphism.

(Cor) Let \pi : \tilde{B} \to B be a covering map, \tilde{B} arcwise connected, and B simply connected. Then \pi is a homeomorphism.

(Def 4) B is locally simply connected if any neighborhood of each point contains a simply connected neighborhood.

(Prop 6) Let \pi : \tilde{B} \to B be a local homeomorphism with the property of lifting arcs. Assume that B is locally simply connected and that \tilde{B} is locally arcwise connected. Then \pi is a covering map.

(subsubsection B) The Hadamard Theorem

(Lem 1) Let S be a complete surface of curvature K \le 0. Then exp_{p} : T_{p} (S) \to S , p \in S, is length-increasing in the following sense : If u, w \in T_{p}(S), we have \langle(d exp_{p})_{u}(w), (d exp_{p})_{u}(w) \rangle \ge \langle w, w \rangle, where, as usual, w denotes a vector in (T_{p}(S))_{u} that is obtained from w by the translation u.

(Cor) Let K \equiv 0. Then exp_{p} : T_{p}(S) \to S, p \in S, is a local isometry.

(Prop 7) Let S be a complete surface with Gaussian curvature K \le 0. Then the map exp_{p} : T_{p}(S) \to S, p \in S, is a covering map.

(Hadamard)(Thm 1) Let S be a simply connected, complete surface, with Gaussian curvature K \le 0. Then exp_{p} : T_{p}(S) \to S, p \in S, is a diffeomorphism; that is , S is diffeomorphic to a plane.

(Hadamard) (Thm 2) Let S be an ovaloid(Connected, compact, regular surface with Gaussian curvature K > 0) . Then the Gauss map N : S \to S^{2} is a diffeomorphism. In particular, S is diffeomorphic to a sphere.

(subsection 5.7.) Global Theorems for curves; The Fary-Milnor Theorem

(Def) Let \phi : S^{1} \to S^{1} be a continuous map. \phi can be though as continuous map \phi : [0,l] \to S^{1}, with \phi(0) = \phi(l) = p \in S^{1}. Thus, \phi is a closed arc at p in S^{1} which, by (Prop 2) of (Sec 5-6) , can be lifted into a unique arc \tilde{\phi} : [0,l] \to R, starting at a point x \in R with \pi(x) = p. Since \pi(\tilde{\phi}(0)) = \pi(\tilde{\phi}), the difference \tilde{\phi}(l) - \tilde{\phi}(0) is an integral multiple of 2 \pi. The integer given by \tilde{\phi}(l) - \tilde{\phi}(0) = (deg \phi) 2\pi is called the degree of \phi.

(Differentiable Jordan Curve Theorem) (Thm 1) Let \alpha : [0,l] \to R^{2} be a plane, regular, closed, simple curve. Then R^{2} - \alpha([0,l]) has exactly two connected components, and \alpha([0,l]) is their common boundary.

(Def) A plane, regular, closed curve \alpha : [0,l] \to R^{2} is convex if, for each t \in [0,l] , the curve lies in one of the closed half-planes determined by the tangent line at t.

(Thm 2) Let \beta : [0,l] \to R^{2} be a plane, regular, simple, closed curve. Then the rotation index of \beta is \mp 1 (depending on the orientation of \beta)

(Prop 1) A plane, regular, closed curve is convex iff it is simple and its curvature k does not change sign.

(Fenchel’s Theorem) (Thm 3) The total curvature of a simple closed curve is \ge 2\pi, and equality holds iff the curve is a plane convex curve.

(Def) A simple closed continuous curve C \subset R^{3} is unknotted if there exists a homotopy H : S^{1} \times I \to R^{3} , I = [0,1], s.t. H(S^{1} \times {0}) = S^{1}, H(S^{1} \times {1}) = C; and H(S^{1} \times {t}) = C_{t} \subset R^{3} is homeomorphic to S^{1} for all t \in [0,1]. Such a homotopy is called an isotopy; an unknotted curve is then a curve isotopic to S^{1}. When this is not the case, C is said to be knotted.

(Fary-Milnor)(Thm 4) The total curvature of a knotted simple closed curve is greater than 4\pi.

(subsection 5.8.) Surfaces of Zero Gaussian Curvature

(Def) A cylinder is a regular surface S s.t. through each point p \in S there passes a unique line R(p) \subset S (the generator through p) which satisfies the condition that if q \neq p, then the lines R(p) and R(q) are parallel or equal.

(Thm) Let S \subset R^{3} be a complete surface with zero Gaussian curvature. Then S is a cylinder or a plane.

(Prop 1) The unique asymptotic line that passes through a parabolic point p \in U \subset S of a surface S of curvature K \equiv 0 is an (open) segment of a (straight) line in S.

(Massey)(Prop 2) Let r be a maximal asymptotic line passing through a parabolic point p \in U \subset S of a surface S of curvature K \equiv 0 and let P \subset S be the set of planar points of S. Then r \cap P = \empty.

(Lem 1) Let s be the arc length of the asymptotic curve passing through a parabolic point p of a surface S of zero curvature and let H = H(s) be the mean curvature of S along this curve. Then , in U, \frac{d^{2}}{ds^{2}}(\frac{1}{H}) = 0.

(Def) Let now Bd(U) be the boundary of U in S ; that is, Bd(U) is the set of points p \in S s.t. every neighborhood of p in S contains points of U and points of S – U = P. 

(Massey)(Prop 3) Let p \in Bd(U) \subset S be a point of the boundary of the set U of parabolic points of a surface S of curvature K \equiv 0. Then through p there passes a unique open segment of line C(p) \subset S . Furthermore, C(p) \subset Bd(U); that is, the boundary of U is formed by segments of lines.

(subsection 5.9.) Jacobi’s Theorems

(Lem 1) Let p \in S, u \in T_{p}(S), l = |u| \neq 0, and let \bar{\gamma} : [0,l] \to T_{p}(S) be the line of T_{p}(S) given by \bar{\gamma}(s) = sv, s \in [0,l] , v = \frac{u}{|u|}. Let \bar{\alpha} : [0,l] \to T_{p}(S) be a differentiable parametrized curve of T_{p}(S), with \bar{\alpha} (0) = 0, \bar{\alpha}(l) = u, and \bar{\alpha}(s) \neq 0 if s \neq 0. Furthermore, let \alpha(s) = exp_{p}(\bar{\alpha})(s) and \gamma(s) = exp_{p}(\bar{\gamma}(s)). We have

l(\alpha) \ge l(\gamma) , where l() denotes the arc length of the corresponding curve. 

In addition, if \bar{\alpha}(s) is not a critical point of exp_{p}, s \in [0,l)] , and if the traces of \alpha and \gamma are distinct, then l(\alpha) > l(\gamma).

(Jacobi) (Thm 1) Let \gamma : [0,l] \to S, \gamma(0) = p be a geodesic without conjugate points; that is, exp_{p}: T_{p}(S) \to S is regular at the points of the line \bar{\gamma}(s) = s\gamma’(0) of T_{p}(S), s \in [0,l] . Let h : [0,l] \times (-\epsilon, \epsilon) \to S be a proper variation of \gamma. Then

There exists a \delta >0 , \delta \le \epsilon, s.t. if t \in (-\delta, \delta), L(t) \ge L(0), where L(t) is the length of the curve h_{t} : [0,l] \to S that is given by h_{t}(s) = h(s,t).

If, in addition, the trace of h, is distinct from the trace of \gamma, L(t) > L(0).

(Def 1) Let \gamma : [0,l] \to S be a geodesic of S and let h : [0,l] \times (-\epsilon, \epsilon) \to S be a continuous map with h(s,0) = \gamma(s) , s \in [0,l] . h is said to be a broken variation of \gamma if there exists a partition 0 = s_{0} < s_{1} < s_{2} < \cdots < s_{n-1} < s_{n} = l of [0,l] s.t. h: [s_{i}, s_{i+1}] \times (-\epsilon, \epsilon) \to S, i = 0,1,…, n-1, is differentiable. The broken variation is said to be proper if h(0,t) = \gamma(0) , h(l,t) = \gamma(l) for every t \in (-\epsilon, \epsilon).

(Lem 2) Let V \in \mathcal{U} be a Jacobi Field along a geodesic \gamma : [0,l] \to S and W \to \mathcal{U}. Then I(V,W) = \langle \frac{DV}{ds}(l) , W(l) \rangle - \langle \frac{DV}{ds} (0), W(0) \rangle.

(Jacobi)(Thm 2) If we let \gamma : [0,l] \to S be a geodesic of S and we let \gamma(s_{0}) \in \gamma((0,l)) be a point conjugate to \gamma(0) = p relative to \gamma, then there exists a proper broken variation h : [0,l] \times (-\epsilon, \epsilon) \to S of \gamma and a real number \delta >0, \delta \le \epsilon, s.t. if t \in (-\delta, \delta) we have L(t) \le L(0).

(subsection 5.10.) Abstract Surfaces; Further Generalizations

(Def 1) An abstract surface(differentiable manifold of dimension 2) is a set S together with a family of one-to-one maps x_{\alpha} : U_{\alpha \to S of open sets U_{\alpha} \subset R^{2} into S s.t. 

\bigcup_{\alpha}(x_{\alpha})(U_{\alpha}) = S.

For each pair \alpha , \beta with x_{\alpha} (U_{\alpha}) \cap x_{\beta}(U_{\beta}) = W \neq \empty we have that x^{-1}_{\alpha}(W) , x_{\beta}^{-1} (W) are open sets in R^{2} , and x_{\beta}^{-1} \bullet x_{\alpha}, x_{\alpha}^{-1} \bullet x_{\beta} are differentiable maps. 

The pair (U_{\alpha}, x_{\alpha}) with p \in x_{\alpha}(U_{\alpha}) is called a parametrization (or coordinate system) of S around p. x_{\alpha}(U_{\alpha}) is called a coordinate neighborhood, and if q = x_{\alpha} (u_{\alpha}, v_{\alpha}) \in S, we say that (u_{\alpha}, v_{\alpha}) are coordinates of q in this coordinate system. The family {U_{\alpha} , x_{\alpha}} is called a differentiable structure for S. 

(Def 2) Let S_{1} and S_{2} be abstract surfaces. A map \phi : S_{1} \to S_{2} is differentiable at p \in S_{1} if given a parametrization y : V \subset R^{2} \to S_{2} around \phi(p) there exists a parametrization x : U \subset R^{2} \to S_{1} around p s.t. \phi(x(U)) \subset y(V) and the map y^{-1} \bullet \phi \bullet x : x^{-1}(U) \subset R^{2} \to R^{2} is differentiable at x^{-1}(p) . \phi is differentiable on S_{1} if it is differentiable at every p \in S_{1} .

(Def 3) A differentiable map \alpha : (-\epsilon, \epsilon) \to S is called a curve on S. Assume that \alpha(0) = p and let D be the set of functions on S which are differentiable at p. The tangent vector to the curve \alpha at t = 0 is the function \alpha’(0) : D \to R given by \alpha’(0) (f) = \frac{d(f \bullet \alpha)}{dt}|_{t = 0} , f \in D. A tangent vector at a point p \in S is the tangent vector at t = 0 of some curve \alpha : (-\epsilon , \epsilon) \to S with \alpha(0) = p.

(Def 4) Let S_{1} and S_{2} be abstract surfaces and let \phi : S_{1} \to S_{2} be a differentiable map. For each p \in S_{1} and each w \in T_{p}(S_{1}) , consider a differentiable curve \alpha : (-\epsilon, \epsilon) \to S_{1} , with \alpha(0) = p, \alpha’(0) = w. Set \beta = \phi \bullet \alpha. The map d\phi_{p} : T_{p} (S_{1}) \to T_{p}(S_{2}) given by d\phi_{p}(w) = \beta’(0) is a well-defined linear map, called the differential of \phi at p.

(Def 5) A geometric surface (Riemannian manifold of dimension 2) is an abstract surface S together with the choice of an inner product \langle , \rangle_{p} at each T_{p} (S), p \in S, which varies differentiably with p in the following sense. For some(and hence all) parametrization x : U \to S around p, the funcitons E(u,v) = \langle \frac{ \partial }{\partial u } , \frac{\partial }{\partial u } \rangle , F(u,v) = \langle \frac{\partial }{\partial u} , \frac{\partial }{\partial v} \rangle , G(u,v) = \langle \frac{\partial }{\partial v} , \frac{\partial }{\partial v} \rangle are differentiable functions in U. The inner product \langle , \rangle is often called a (Riemannian) metric on S.

(Def 6) A differentiable map \phi : S \to R^{3} of an abstract surface S into R^{3} is an immersion if the differential d \phi_{p} : T_{p} (S) \to T_{p}(R^{3}) is injective. If, in addition, S has a metric \langle, \rangle and \langle d \phi_{p}(v), d \phi_{p}(w) \rangle_{\phi(p)} = \langle v , w \rangle_{p} , v , w \in T_{p}(S), \phi is said to be an isometric immersion.

(Def 7) Let S be an abstract surface. A differentiable map \phi : S \to R^{n} is an embedding if \phi is an immersion and a homeomorphism onto its image.

(Def 1a) A differentiable manifold of dimension n is a set M together with a family of one-to-one maps x_{\alpha} : U_{\alpha} \to M of open sets U_{\alpha} \subset R^{n} into M s.t. 

\bigcup_{\alpha}(x_{\alpha})(U_{\alpha}) = M.

For each pair \alpha , \beta with x_{\alpha} (U_{\alpha}) \cap x_{\beta}(U_{\beta}) = W \neq \empty we have that x^{-1}_{\alpha}(W) , x_{\beta}^{-1} (W) are open sets in R^{n} , and x_{\beta}^{-1} \bullet x_{\alpha}, x_{\alpha}^{-1} \bullet x_{\beta} are differentiable maps.

The family {U_{\alpha}, x_{\alpha}} is maximal relative to first and second conditions.

The family {U_{\alpha}, x_{\alpha}} satisfying first and second conditions is called a differentiable structure on M.

(Def 5a) ) A Riemannian manifold is an n-dimensional differentiable manifold M together with a choice, for each p \in M, of an inner product \langle , \rangle_{p} at each T_{p} (M), p \in M, which varies differentiably with p in the following sense. For some parametrization x_{\alpha} : U_{\alpha} \to M with p \in x_{\alpha}(U_{\alpha}) , the functions g_{ij}(u_{1},…,u_{n}) = \langle \frac{\partial}{\partial u_{i}}, \frac{\partial}{\partial u_{j}} \rangle , i, j = 1, …, n , are differentiable at x_{\alpha}^{-1} (p) ; here (u_{1}, …, u_{n}) are the coordinates of U_{\alpha} \subset R^{n}.

(subsection 5.11) Hilbert’s Theorem

(Thm) A complete geometric surface S with constant negative curvature cannot be isometrically immersed in R^{3}.

(Def) assume the curvature K \equiv -1. Since exp_{p} : T_{p}(S) \to S is a local diffeomorphism , it induces an inner product in T_{p}(S). Denote by S’ the geometric surface T_{p}(S) with this inner product.

(Lem 1) The area of S’ is infinite.

(Def) Assume there exists an isometric immersion \phi : S’ \to R^{3} , where S’ is a geometric surface homeomorphic to a plane and with K \equiv -1.

(Lem 2) For each p \in S’ there is a parametrization x : U \subset R^{2} \to S’, p \in x(U) , s.t. the coordinate curves of x are the asymptotic curves of x(U) = V’ and form a Tchbyshef net. (we shall express this by saying that the asymptotic curves of V’ form a Tchebyshef net.)

(Lem 3) Let V’ \subset S’ be a coordinate neighborhood of S’ s.t. the coordinate curves are the asymptotic curves in V’. Then the area A of any quadrilateral formed by the coordinate curves is smaller than 2\pi.

(Lem 4) For a fixed t, the curve x(s,t) , -\infty < s < \infty , is an asymptotic curve with s as arc length.

(Lem 5) x is a local diffeomorphism.

(Lem 6) x is surjective.

(Lem 7) On S’ there are two differentiable linearly independent vector fields which are tangent to the asymptotic curves of S’.

(Lem 8) x is injective.

(Appendix) Point-Set Topology of Euclidean Spaces

(subsection A) Preliminaries

(Def 1) A sequence p_{1}, …, p_{i}, …, \in R^{n} converges to p_{0} \in R^{n} if given \epsilon >0, there exists an index i_{0} of the sequence s.t. p_{i} \in B_{e}(p_{0}) for all i > i_{0} . In this situation, p_{0} is the limit of the sequence {p_{i}} and this is denoted by {p_{i}} \to p_{0}.

(Prop 1) A map F : U \subset R^{n} \to R^{m} is continuous at p_{0} \in U iff for each converging sequence {p_{i}} \to p_{0} in U, the sequence {F(p_{i})} converges to F(p_{0}).

(Def 2) A point p \in R^{n} is a limit point of a set A \subset R^{n} if every neighborhood of p in R^{n} contains one point of A distinct from p.

(Def 3) A set F \subset R^{n} is closed if every limit point of F belongs to F. The closure of A \subset R^{n} denoted by \bar{A} is the union of A with its limit points.

(Prop 2) F \subset R^{n} is closed iff the complement R^{n} – F of F is open.

(Prop 3) A map F : U \subset R^{n} \to R^{m} is continuous iff for each open set V \subset R^{m} , F^{-1}(V) is an open set.

(Cor) F : U \subset R^{n} \to R^{m} is continuous iff for every closed set A \subset R^{m}, F^{-1} (A) is a closed set.

(Def 4) Let A \subset R^{n}. The boundary Bd A of A is the set of points p in R^{n} s.t. every neighborhood of p contains points in A and points in R^{n} – A.

(Def 5) Let A \subset R^{n} . We say that V \subset A is an open set in A if there exists an open set U in R^{n} s.t. V = U \cap A. A neighborhood of p \in A in A is an open set in A containing p.

(Def 6) A subset A \subset R of the real line R is bounded above if there exists M \in R s.t. M \ge a for all a \in A. The number M is called an upper bound for A. When A is bounded above, a supremum or a least upper bound of A, sup A(or l.u.b. A) is an upper bound M which satisfies the following condition : Given \epsilon >0, there exists a \in A s.t. M - \epsilon < a. By changing the sign of the above inequalities, we define similarly a lower bound for A and an infimum (or a greatest lower bound) of A, inf A (or g.l.b. A).

(Axiom of Completeness of Real numbers) Let A \subset R be nonempty and bounded above(below). Then there exists sup A (inf A).

(Lem 1) Call a sequence {x_{i}} of real numbers a Cauchy sequence if given \epsilon <0, there exists i_{0} s.t. |x_{i} – x_{j}| < \epsilon for all i,j > i_{0}. A sequence is convergent iff it is a Cauchy sequence.

(Def 7) A sequence {p_{i}} , p_{i} \in R^{n}, is a Cauchy sequence if given \epsilon >0, there exists an index i_{0} s.t. the distance |p_{i} – p_{j}| < \epsilon for all i,j > i_{0}.

(Prop 4) A sequence {p_{i}} , p_{i} \in R^{n}, converges iff it is a Cauchy sequence.

(subsection B) Connected sets

(Def 8) A continuous curve \alpha : [a,b] \to A \subset R^{n} is called an arc in A joining \alpha(a) to \alpha(b).

(Def 9) A \subset R^{n} is arcwise connected if , given two points p, q \in A, there exists an arc in A joining p to q.

(Def 10) A \subset R^{n} is connected when it is not possible to write A = U_{1} \cap U_{2} , where U_{1} and U_{2} are nonempty open sets in A and U_{1} \cap U_{2} = \empty.

(Prop 5) Let A \subset R^{n} be connected and let B \subset A be simultaneously open and closed in A. Then either B = \empty or B = A.

(Prop 6) Let F : A \subset R^{n} \to R^{m} be continuous and A be connected. Then F(A) is connected.

(Def 11) An interval of the real line R is any of the sets a < x < b, a \le x \le b, a < x \le b , a \le x < b , x \in R, The cases a = b , a = - \infty , b = + \infty are not excluded, so that an interval may be a point , a half-line, or R itself.

(Prop 7) A \subset R is connected iff A is an interval.

(Prop 8) Let f : A \subset R^{n} \to R be continuous and A be connected. Assume that f(q) \neq 0 for all q \in A. Then f does not change sign in A.

(Prop 9) Let A \subset R^{n} be arcwise connected. Then A is connected.

(Def 12) A set A \subset R^{n} is locally arcwise connected if for each p \in A and each neighborhood V of p in A there exists an arcwise connected neighborhood U \subset V of p in A.

(Prop 10) Let A \subset R^{n} be a locally arcwise connected set. Then A is connected iff it is arcwise connected.

(subsection C) Compact sets

(Def 13) A set A \subset R^{n} is bounded if it is contained in some ball of R^{n}. A set K \subset R^{n} is compact if it is closed and bounded.

(Def 14) An open cover of a set A \subset R^{n} is a family of open sets {U_{\alpha}} , \alpha \in \mathfrak{A} s.t. \bigcup_{\alpha} U_{\alpha} = A. When there are only finitely many U_{\alpha} in the family, we say that the cover is finite. If the subfamily {U_{\beta}} , \beta \in \mathfrak{B} \subset \mathfrak{A} , still covers A, that is, \bigcup_{\beta} U_{\beta{ = A, we say that {U_{\beta}} is a subcover of {U_{\alpha}} .

(Prop 11) For a set K \subset R^{n} the following assertions are equivalent.

K is compact.

(Heine-Borel) Every open cover of K has a finite subcover.

(Bolzano-Weierstrass) Every infinite subset of K has a limit point in K.

(Prop 12) Let F : K \subset R^{n} \to R^{m} be continuous and let K be compact. Then F(K) is compact.

(Prop 13) Let f : K \subset R^{n} \to R be a continuous function defined on a compact set K. Then there exists p_{1}, p_{2} \in K s.t. f(p_{2}) \le f(p) \le f(p_{1}) for all p \in K; that is, f reaches a maximum at p_{1} and a minimum at p_{2}.

(subsection D) Connected Components

(Prop 14) Let C_{\alpha} \subset R^{n} be a family of connected sets s.t. \bigcap_{\alpha} C_{\alpha} \neq \empty. Then \bigcup_{\alpha} C_{\alpha} = C is a connected set.

(Def 15) Let A \subset R^{n} and p \in A. The union of all connected subsets of A which contain p is called the connected component of A containing p.

(Prop 15) Let C \subset A \subset R^{n} be a connected set. Then the closure \bar{C} of C in A is connected.

(Cor) A connected component C \subset A \subset R^{n} of a set A is closed in A.

(prop 16) Let C \subset A \subset R^{n} be a connected component of a locally arcwise connected set A. Then C is open in A.

