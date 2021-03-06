---



layout: post



title : (Differential Geometry) The Geometry of the Gauss Map



date : 2018-01-20 12:54:04 +0900



---

(section 3) The Geometry of the Gauss Map

(subsection 3.2.) The Definition of the Gauss Map and its Fundamental properties

(Def) If V \subset S is an open set in S and N : V \to R^{3} is a differentiable map which associates to each q \in V a unit normal vector at q , we say that N is a differentiable field of unit normal vectors on V.

A regular surface is orientable if it admits a differentiable field of unit normal vectors defined on the whole surface; the choice of such a field N is called an orientation of S.

(Def 1) Let S \subset R^{3} be a surface with an orientation N. The map N : S \to R^{3} takes its values in the unit sphere S^{2} = {(x,y,z) \in R^{3} ; | x^{2} + y^{2} + z^{2} = 1} The map N : S \to S^{2} , thus defined, is called the Gauss map of S.

(Prop 1) The differential dN_{p} : T_{p}(S) \to T_{p} (S) of the Gauss map is a self-adjoint linear map.

(Def 2) The quadratic form II_{p}, defined in T_{p}(S) by II_{p}(v) = - \langle dN_{p}(v), v \rangle  is called the second fundamental form of S at p.

(Def 3) Let C be a regular curve in S passing through p \in S, k the curvature of C at p, and cos \theat = \langle n, N \rangle, where n is the normal vector to C and N is the normal vector to S at p. The number k_{n} = k cos \theta is then called the normal curvature of C \subset S at p.

(Meusnier) (prop 2) All curves lying on a surface S and having at a given point p \in S the same tangent line have at this point the same normal curvatures.

(Def 4) The maximum normal curvature k_{1} and the minimum normal curvature k_{2} are called the principal curvatures at p; the corresponding directions, that is, the directions given by the eigenvectors e_{1}, e_{2} are called principal directions at p.

(Def 5) If a regular connected curve C on S is such that for all p \in C the tangent line of C is a principal direction at p, then C is said to be a line of curvature of S.

(Olinde Rodrigues) (Prop 3) A necessary and sufficient condition for a connected regular curve C on S to be a line of curvature of S is that N???(t) = \lambda(t) \alpha???(t) for any parametrization \alpha(t) of C, where N(t) = N \bullet \alpha(t) and \lambda (t) is a differentiable function on t. In this case, \lambda(t) is the (principal) curvature along \alpha???(t).

(Def 6) Let p \in S and let dN_{p} : T_{p}(S) \to T_{p}(S) be the differential of the Gauss map. The determinant of dN_{p} is the Gaussian curvature K of S at p. The negative of half of the trace of dN_{p} is called the mean curvature H of S at p.

(Def 7) A point of a surface S is called

Elliptic if det(dN_{p}) >0.

Hyperbolic if det(dN_{p}) < 0.

Parabolic if det(dN_{p}) = 0 , with dN_{p} \neq 0.

Planar if dN_{p} = 0.

(Def 8) If at p \in S, k_{1} = k_{2}, then p is called an umbilical point of S; in particular, the planar points (k_{1} = k_{2} = 0) are umbilical points.

(Prop 4) If all points of a connected surface S are umbilical points, then S is either contained in a sphere or in a plane.

(Def 9) Let p be a point in S. An asymptotic direction of S at p is a direction of T_{p}(S) for which the normal curvature is zero. An asymptotic curve of S is a regular connected curve C \subset S such that for each p \in C the tangent line of C at p is an asymptotic direction.

(Def) Let p be a point in S. the Dupin indicatrix at p is the set of vectors w of T_{p}(S) such that II_{p}(w) = \mp 1.

(Def 10) Let p be a point on a surface S. Two nonzero vectors w_{1}, w_{2} \in T_{p}(S) are conjugate if \langle dN_{p}(w_{1}) , w_{2} \rangle = \langle w_{1}, dN_{p} (w_{2}) \rangle = 0. Two directions r_{1}, r_{2} at p are conjugate if a pair of nonzero vectors w_{1}, w_{2} parallel to r_{1} and r_{2} , respectively, are conjugate.

(subsection 3.3.) The Gauss map in Local Coordinates

(Prop 1) Let p \in S be an elliptic point of a surface S. then there exists a neighborhood V of p in S s.t. all points in V belong to the same side of the tangent line T_{p}(S). Let p \in S be a hyperbolic point. Then in each neighborhood of p there exists points of S in both sides of T_{p}(S).

(Prop 2) Let p be a point of a surface S s.t. the Gaussian curvature K(p) \neq 0 , and let V be a connected neighborhood of p where K does not change sign. Then K(p) = \lim_{A \to 0} \frac{A???}{A} where A is the area of a region B \subset V containing p , A??? is the area of the image of B by the Gauss map N : S \to S^{2}, and the limit is taken through a sequence of regions B_{n} that converges to p, in the sense that any sphere around p contains all B_{n} for n sufficiently large.

(subsection 3.4.)Vector fields

(Def) A vector field in an open set U \subset R^{2} is a map which assigns to each q \in U a vector w(q) \in R^{2} . The vector field w is said to be differentiable if writing q = (x,y) and w(q) = (a(x,y) , b(x,y)) , the functions a and b are differentiable functions in U.

(Thm 1) Let w be a vector field in an open set U \subset R^{2}. Given p \in U, there exists a trajectory \alpha : I \to U of w (\alpha???(t) = w(\alpha(t)), t \in I) with \alpha(0) = p. This trajectory is unique in the following sense : Any other trajectory \beta : J \to U with \beta(0) = p agrees with \alpha in I \cap J.

(Thm 2) Let w be a vector field in an open set U \subset R^{2}. For each p \in U there exists a neighborhood V \subset U of p, an interval I, and a mapping \alpha : V \times I \to U s.t.

for a fixed q \in V, the curve \alpha(q,t) , t \in I, is the trajectory of w passing through q; that is, \alpha(q,0) = q, \frac{\partial \alpha}{\partial t} (q,t) = w(\alpha(q,t)).

\alpha is differentiable.

(Lem) Let w be a vector field in an open set U \subset R^{2} and let p \in U be such that w(p) \neq 0. Then there exists a neighborhood W \subset U of p and a differentiable function f: W \to R s.t. f is constant along each trajectory of w and df_{n} \new 0 for all q \in W.

(Def) A field of directions r in an open set U \subset R^{2} is a correspondence which assigns to each p \in U a line r(p) in R^{2} passing through p. r is said to be differentiable at p \in U if there exists a nonzero differentiable vector field w, defined in a neighborhood V \subset U of p, such that for each q \in V, w(q) \neq 0 is a basis of r(q); r is differentiable in U if it is differentiabl for every p \in U.

To each nonzero differentiable vector field w in U \subset R^{2}, there corresponds a differentiable field of directions given by r(p) = line generated by w(p), p \in U.

(Def 1) A vector field w in an open set U \subset S of a regular surface S is a correspondence which assigns to each p \in U a vector w(p) \in T_{p}(S). The vector field w is differentiable at p \in U if, for some parametrization x(u,v) at p, the functions a(u,v) and b(u,v) given by w(p) = a(u,v)x_{u} + b(u,v)x_{v} are differentiable functions at p; it is clear that this definition does not depend on the choice of x.

(Thm) Let w_{1} and w_{2} be two vector fields in an open set U \subset S, which are linearly independent at some point p \in U. Then it is possible to parametrize a neighborhood V \subset U of p in such a way that for each q \in V the coordinate lines of this parametrization passing through q are tangent to the lines determined by w_{1}(q) and w_{2}(q).

(Cor 1) Given two fields of directions r and r??? in an open set U \subset S s.t. at p \in U, r(p) \neq r???(p), there exists a parametrization x in a neighborhood of p s.t. the coordinate curves of x are the integral curves of r and r???.

(Cor 2) For all p \in S there exists a parametrization x(u,v) in a neighborhood V of p s.t. the coordinate curves u = const., v = const. intersect orthogonally for each q \in V (such an x is called an orthogonal parametrization).

(Cor 3) Let p \in S be a hyperbolic point of S. Then it is possible to parametrize a neighborhood of p in such a way that the coordinate curves of this parametrization are the asymptotic curves of S.

(Cor 4) Let p \in S be a nonumbilical points of S. Then it is possible to parametrize a neighborhood of p in such a way that the coordinate curves of this parametrization are the lines of curvature of S.

(subsection 3.5.) Ruled Surfaces and Minimal Surfaces

(Subsubsection A) Ruled Surfaces

(Def) A (differentiable) one-parameter family of (straight) lines [\alpha(t), w(t)] is a correspondence that assigns to each t \in I a point \alpha(t) \in R^{3} and a vector w(t) \in R^{3} , w(t) \neq 0 , so that both \alpha(t) and w(t) depend differentiably on t. For each t \in I, the line L, which passes through \alpha(t) and is parallel to w(t) is called the line of the family at t.

Given a one-parameter family of lines [\alpha(t), w(t)] , the parametrized surface x(t,v) = \alpha(t) + vw(t) , t \in I, v \in R, is called the ruled surface generated by the family [\alpha(t), w(t)]. The lines are called the rullings, and the curve \alpha(t) is called a directrix of the surface x. Sometimes we use the expression ruled surface to mean the trace of x.

(subsubsection B)Minimal Surfaces

(Def) A regular parametrized surface is called minimal if its mean curvature vanishes everywhere. A regular surface S \subset R^{3} is minimal if each of its parametrization is minimal.

Let x : U \subset R^{2} \to R^{3} be a regular parametrized surface. Choose a bounded domain D \subset U and a differentiable function h : \bar{D} \to R, where \bar{D} is the union of the domain D with its boundary \partial D. The normal variation of x(\bar{D}) , determined by h, is the map given by, \phi : \bar{D} \times (\epsilon, \epsilon) \to R^{3} : \phi (u,v,t) = x(u,v) + th(u,v)N(u,v) , (u,v) \in \bar{D} , t \in (-\epsilon, \epsilon). 

The mean curvature H is H = \frac{1}{2} \frac{Eg ??? 2fF + Ge}{EG-F^{2}} where \langle x_{u}, N_{u} \rangle = -e , \lange x_{u} , N_{v} \rangle + \langle x_{v} , N_{u} \rangle = -2f , \langle x_{v} , N_{v} \rangle = -g.

The derivative of the area A(t) of x???(\bar{D}) at t = 0 is A???(0) = -\int_{\bar{D}}2hH \sqrt{EG-F^{2}} du dv. the area A(t) of x^{t}(\bar{D}) is A(t) = \int_{\bar{D}} \sqrt{E^{t}G^{t} ??? (F^{t})^{2}} du dv

(Prop 1) Let x : U \to R^{3} be a regular parametrized surface and let D \subset U be a bounded domain in U. Then x is minimal iff A???(0) = 0 for all such D and all normal variations of x(\bar{D}).

(Def) For an arbitrary parametrized regular surface, the mean curvature vector defined by \mathbf{H} = HN.  A regular parametrized surface x = x(u,v) is said to be isothermal if \langle x_{u}, x_{u} \rangle = \langle x_{v} , x_{v} \rangle and \langle x_{u} , x_{v} \rangle = 0.

(Prop 2) Let x = x (u,v) be a regular parametrized surface and assume that x is isothermal. Then x_{uu} + x_{vv} = 2 \lambda^{2}\mathbf{H}, where \lambda^{2} = \langle x_{u}, x_{u} \rangle = \langle x_{v}, x_{v} \rangle.

(Def) The Laplacial \Delta f of a differentiable function f : U \subset R^{2} \to R is defined by \Delta f = (\partial^{2}f / \partial u^{2}) + (\partial^{2}f / \partial v^{2}) , (u,v) \in U. We say that f is harmonic in U if \Delta f = 0 .

(Cor) Let \mathbf{x}(u,v) = (x(u,v) , y(u,v), z(u,v)) be a parametrized surface and assume that x is isothermal. Then x is minimal iff its coordinate functions x,y,z are harmonic.

(Def) A function f : U \subset \mathbb{C} \to \mathbb{C} is analytic when, f(\zeta) = f_{1}(u,v) + i f_{2}(u,v), the real functions f_{1} and f_{2} have continuous partial derivatives of first order which satisfy the Cauchy-Riemann equations : \frac{\partial f_{1}}{\partial u} = \frac{\partial f_{2}}{\partial v}, \frac{\partial f_{1}}{\partial v} = -\frac{\partial f_{2}}{\partial u}.

Let x : U \subset R^{2} \to R^{3} be a regular parametrized surface and define complex functions \phi_{1}, \phi_{2}, \phi_{3} by \phi_{1}(\zeta) = \frac{x}{u} ??? i \frac{x}{v} , \phi_{2}(\zeta) = \frac{y}{u} ??? i \frac{y}{v} , \phi_{3}(\zeta) = \frac{z}{u} ??? i \frac{z}{v} , where x,y, z are the component functions of x.

(Lem) x is isothermal iff \phi_{1}^{2} + \phi_{2}^{2} + \phi_{3}^{2} \equiv 0. If this last condition is satisfied, x is minimal iff \phi_{1}, \phi_{2} and \phi_{3} are analytic functions.

(Osserman) (Thm) Let S \subset R^{3} be a regular, closed (as a subset of R^{3}) minimal surface in R^{3} which is not a plane. Then the image of the Gauss map N : S \to S^{2} is dense in the sphere S^{2} (that is, arbitrarily close to any point of S^{2} there is a point of N(S) \subset S^{2}) .

(Appendix) Self-adjoint Linear maps and Quadratic forms

(Def) V is a vector space of dimension 2, with an inner product \langle , \rangle. A linear map A : V \to V is self-adjoint if \langle Av , w \rangle = \langle v, Aw \rangle for all v , w \in V.

To each self-adjoint linear map we associate a map B : V \times V \to R defined B(v,w) = \langle Av , w \rangle. It is bilinear, and B(v,w) = B(w,v) so B is a bilinear symmetric form in V. 

To each Symmetric bilinear form B in V, there corresponds a quadratic form Q in V given by Q(v) = B(v,v) , v \in V . 

(Lem) If the function Q(x,y) = ax^{2} + 2bxy + cy^{2} , restricted to the unit circle x^{2} + y^{2} , has a maximum at the point (1,0), then b = 0.

(Prop) Given a quadratic form Q in V , there exists an orthonormal basis [e_{1}, e_{2}] of V s.t. if v \in V is given by v = xe_{1} + ye_{2}, then Q(v) = \lambda_{1} x^{2} + \lambda_{2} y^{2}, where \lambda_{1} and \lambda_{2} are the maximum and minimum, respectively, of Q on the unit circle |v| = 1.

(Thm) Let A : V \to V be a self-adjoint linear map. Then there exists an orthonormal basis [e_{1}, e_{2}] of V s.t. A(e_{1}) = \lambda_{1} e_{1} , A(e_{2}) = \lambda_{2} e_{2}. (that is, e_{1} and e_{2} are eigenvectors , and \lambda_{1}, \lambda_{2} are eigenvalues of A). In the basis [e_{1}, e_{2}] , the matrix of A is clearly diagonal and the elements \lambda_{1} , \lambda_{2} , \lambda_{1} \ge \lambda_{2}, on the diagonal are the maximum and the minimum, respectively, of the quadratic form Q(v) = \langle Av, v \rangle on the unit circle of V.

