---



layout: post



title : (Differential Geometry) The Intrinsic Geometry of Surfaces



date : 2018-01-20 12:55:04 +0900



---

(section 4) The Intrinsic Geometry of Surfaces

(subsection 4.2) Isometries ; Conformal maps

(Def 1) S and \bar{S} will always denote regular surfaces. A diffeomorphism \phi : S \to \bar{S} is an isometry if for all p \in S and all pairs w_{1} , w_{2} \in T_{p}(S) we have \langle w_{1}, w_{2} \rangle_{p} = \langle d\phi_{p} (w_{1}) , d\phi_{p}( w_{2}) \rangle_{\phi(p)} , the surfaces S and \bar{S} are then said to be isometric.

(Def 2) A map \phi : V \to \bar{S} of a neighborhood V of p \in S is a local isometry at p if there exists a neighborhood \bar{C} of \phi(p) \in \bar{S} s.t. \phi : V \to \bar{V} is an isometry. If there exists a local isometry into \bar{S} at every p \in S, the surface S is said to be locally isometric to \bar{S} . S and \bar{S} are locally isometric if S is locally isometric to \bar{S} and \bar{S} is locally isometric to S.

(Prop 1) Assume the existence of parametrizations x : U \to S and \bar{x} : U \to \bar{S} s.t. E = \bar{E}, F = \bar{F}, G = \bar{G} in U. Then the map \phi = \bar{x} \bullet x^{-1} ; x(U) \to \bar{S} is a local isometry.

(Def 3) A diffeomorphism \phi : S \to \bar{S} is called a conformal map if for all p \in S and all v_{1} , v_{2} \in T_{p}(S) we have \langel d\phi_{p}(v_{1}, d\phi_{p}(v_{2}) \rangle = \lambda^{2}(p) \langle v_{1}, v_{2} \rangle_{p} , where \lambda^{2} is a nowhere-zero differentiable function on S; the surfaces S and \bar{S} are then said to be conformal. A map \phi : V \to \bar{S} of a neighbhorhood V of p \in S into \bar{S} is a local conformal map at p if there exists a neighborhood \bar{V} of \phi(p) s.t. \phi : V \to \bar{V} is a conformal map. If for each p \in S, there exists a local conformal map at p, the surface S is said to be locally conformal to \bar{S}.

(Prop 2) Let x : U \to S and \bar{x} : U \to \bar{S} be parametrizations s.t. E = \lambda^{2} \bar{E}, F = \lambda^{2} \bar{F}, G = \lambda^{2} \bar{G} in U, where \lambda^{2} is a nowhere-zero differentiable function in U. Then the map \phi = \bar{x} \bullet x^{-1} : x (U) \to \bar{S} is a local conformal map.

(Thm) Any two regular surfaces are locally conformal.

(subsection 4.3.) The Gauss Theorem and the Equations of Compatibility

(Def) Given x : U \subset R^{2} \to S be a parametrization in the orientation of S. By expressing the derivatives of the vectors x_{u}, x_{v} and N in the basis [x_{u}, x_{v} , N] , we obtain 

x_{uu} = \Gamma_{1}^{1}_{1} x_{u} + \Gamma_{1}^{2}_{1} x_{v} + L_{1}N ,

x_{uv} = \Gamma_{1}^{1}_{2} x_{u} + \Gamma_{1}^{2}_{2} x_{v} + L_{2}N ,

x_{vu} = \Gamma_{2}^{1}_{1} x_{u} + \Gamma_{2}^{2}_{1} x_{v} + L_{3}N ,

x_{vv} = \Gamma_{2}^{1}_{2} x_{u} + \Gamma_{2}^{2}_{2} x_{v} + L_{4}N ,

N_{u} = a_{1 1} x_{u} + a_{21} x_{v} ,

N_{v} = a_{12} x_{u} + a_{22} x_{v}.

where the a_{ij} , i,j = 1,2, were obtained in Chap. 3 and the other coefficients are to be determined. The coefficients \Gamma_{ij}^{k} ,i,j,k = 1,2, are called the Christoffel symbols of S in the parametrization x. Since x_{uv} = x_{vu} , \Gamma_{12}^{1} = \Gamma_{21}^{1} and \Gamma_{12}^{2} = \Gamma_{21}^{2}.

We obtain L_{1} = e , L_{2} = \bar{L_{2}} = f, L_{3} = g, where e,f,g are coefficients of the second fundamental form of S.

All geometric concepts and properties expressed in terms of Christoffel symbols are invariant under isometries.

(Theorema Egregium) (Gauss) The Gaussian curvature K of a surface is invariant by local isometries.

(Def) Gauss formula : (\Gamma_{12}^{2})_{u} ??? (\Gamma_{11}^{2})_{v} + \Gamma_{12}^{1}\Gamma_{11}^{2} +\Gamma_{12}^{2}\Gamma_{12}^{2} - \Gamma_{11}^{2}\Gamma_{22}^{2} - \Gamma_{11}^{1}\Gamma_{12}^{2} = -E \frac{eg-f^{2}}{EG-F^{2}} = -EK.

(Def) Mainardi-Codazzi equations

e_{v} ??? f_{u} = e\Gamma_{12}^{1} + f(\Gamma_{12}^{2} - \Gamma_{11}^{1}) ??? g \Gamma_{11}^{2} 

f_{v} ??? g_{u} = e \Gamma_{22}^{1} + f(\Gamma_{22}^{2} - \Gamma_{12}^{1} ) -g \Gamma_{12}^{2}

(Bonnet) (Thm) Let E,F,G,e,f,g, be differentiable functions, defined in an open set V \subset R^{2} , with E >0, and G >0. Assume that the given functions satisfy formally the Gauss and Mainardi-Codazzi equations and that EG-F^{2} >0. Then, for every q \in V there exists a neighborhood U \subset V of q and a diffeomorphism x : U \to x(U) \subset R^{3} s.t. the regular surface x(U) \subset R^{3} has E,F,G, and e,f,g, as coefficients of the first and second fundamental forms, respectively. Furthermore, if U is connected and if \bar{x} : U \to \bar{x}(U) \subset R^{3} is another diffeomorphism satisfying the same conditions, then there exist a translation T and a proper linear orthogonal transformation \rho in R^{3} s.t. \bar{x} = T \bullet \rho \bullet x.

(subsection 4.4.) Parallel Transport . Geodesics.

(Def 1) Let w be a differentiable vector field in an open set U \subset S and p \in U. Let y \in T_{p}(S). Consider a parametrized curve \alpha : (-\epsilon , \epsilon) \to U, with \alpha(0) = p and \alpha???(0) = y, and let w(t) , t \in (- \epsilon, \epsilon) , be the restriction of the vector field w to the curve \alpha. The vector obtained by the normal projection of (dw/dt)(0) onto the plane T_{p}(S) is called the covariant derivative at p of the vector field w relative to the vector y. This covariant derivative is denoted by (Dw/dt)(0) or (D,w)(p) 

(Def 2) A parametrized curve \alpha : [0,l] \to S is the restriction to [0,l] of a differentiable mapping of (0 - \epsilon , l + \epsilon) , \epsilon >0, into S. If \alpha(0) = p and \alpha(l) = q, we say that \alpha joins p to q. \alpha is regular if \alpha???(t) \neq 0 for t \in [0, l].

(Def 3) Let \alpha : I \to S be a parametrized curve in S. A vector field w along \alpha is a correspondence that assigns to each t \in I a vector w(t) \in T_{\alpha(t)} (S). The vector field w is differentiable at t_{0} \in I if for some parametrization x(u,v) in \alpha(t_{0}) the components a(t), b(t) of w(t) = ax_{u} + bx_{v} are differentiable functions of t at t_{0}. w is differentiable in I if it is differentiable for every t \in I.

(Def 4) Let w be a differentiable vector field along \alpha : I \to S. The expression 

\frac{Dw}{dt} = (a??? + \Gamma_{11}^{1} au??? + \Gamma_{12}^{1} av??? + \Gamma_{12}^{1}bu??? + \Gamma_{22}^{1}bv???) x_{u} + (b??? + \Gamma_{11}^{2}au??? + \Gamma_{12}^{2} av??? + \Gamma_{12}^{2}bu??? + \Gamma_{22}^{2} bv???) x_{v}

of (Dw/dt)(t), t \in I , is well-defined and is called the covariant derivative of w at t.

(Def 5) A vector field w along a parametrized curve \alpha : i \to S is said to be parallel if Dw/dt = 0 for every t \in I.

(prop 1) Let w and v be parallel vector fields along \alpha : I \to S. Then \langle w(t), v(t) \rangle is constant. In particular, |w(t)| and |v(t)| are constant, and the angle between v(t) and w(t) is constant.

(prop 2) Let \alpha : I \to S be a parametrized curve in S and let w_{0} \in T_{\alpha(t_{0}) (S) , t_{0} \in I. Then there exists a unique parallel vector field w(t) along \alpha(t) , with w(t_{0}) = w_{0}.

(Def 6) Let \alpha : I \to S be a parametrized curve and w_{0} \in T_{\alpha(t_{0})} (S) , t_{0} \in I. Let w be the parallel vector field along \alpha, with w(t_{0}) = w_{0}. The vector w(t_{1}) , t_{1} \in I, is called the parallel transport of w_{0} along \alpha at the point t_{1}.

(Def 7) A map \alpha : [0,l] \to S is a parametrized piecewise regular curve if \alpha is continuous and there exists a subdivision 0 = t_{0} < t_{1} < \cdots < t_{k} < t_{k+1} = l of the interval [0,l] in such a way that the restriction \alpha | [t_{i}, t_{i+1}] , i = 0, ???, k is a parametrized regular curve. Each \alpha|[t_{i},t_{i+1}] is called a regular arc of \alpha .

(Def 8) A nonconstant, parametrized curve \gamma : I \to S is said to be geodesic at t \in I if the field of tangent vectors \gamma ???(t) is parallel along \gamma at t; that is , \frac{D\gamma???(t)}{dt} = 0 ; \gamma is a parametrized geodesic if it is geodesic for all t \in I.

(Def 8a) A regular connected curve C in S is said to be a geodesic if , for every p \in S, the parametrization \alpha(s) of a coordinate neighborhood of p by the arc length s is a parametrized geodesic; that is, \alpha???(s) is a parallel vector field along \alpha(s).

(Def 9) Let w be a differentiable field of unit vectors along a parametrized curve \alpha : I \to S on an oriented surface S. Since w(t), t \in I, is a unit vector field, (dw/dt)(t) is a normal to w(t), and therefore \frac{Dw}{dt} = \lambda(N \wedge w(t)) . The real number \lambda = \lambda(T) , denoted by [Dw/dt] , is called the algebraic value of the covariant derivative of w at t.

(Def 10) Let C be an oriented regular curve contained on an oriented surface S ,and let \alpha(s) be a parametrization of C, in a neighborhood of p \in S, by the arc length s. The algebraic value of the covariant derivative [D\alpha???(s)/ds] = k_{g} of \alpha???(s) at p is called the geodesic curvature of C at p.

(Lem 1) Let a and b be differentiable functions in I with a^{2} + b^{2} = 1 and \phi_{0} be s.t. a(t_{0}) = cos \phi_{0} , b(t_{0}) = sin \phi_{0} . Then the differentiable function \phi = \phi_{0} + \int_{t_{0}}^{t} (ab??? ??? ba???) dt is such that cos \phi(t) = a(t), sin \phi(t) = b(t) , t \in I, and \phi(t_{0}) = \phi_{0}.

(Lem 2) Let v and w be two differentiable vector fields along the curve \alpha : I \to S, with |w(t)| = |v(t)| = 1, t \in I, Then [\frac{Dw}{dt}] ??? [\frac{Dv}{dt}] = \frac{d\phi}{dt} where \phi is one of the differentiable determinations of the angle fron v to w, as given by (Lem 1).

(Prop 3) Let x(u,v) be an orthogonal parametrization (that is, F = 0) of a neighborhood of an oriented surface S, and w(t) be a differentiable field of unit vectors along the curve x(u(t), v(t)). Then [\frac{Dw}{dt}] = \frac{1}{2\sqrt{EG}} {G_{u}\frac{dv}{dt} ??? E_{v}\frac{du}{dt}} + \frac{d\phi}{dt} where \phi(t) is the angle from x_{u} to w(t) in the given orientation.

(Liouville)(prop 4) Let \alpha(s) be a parametrization by arc length of a neighborhood of a point p \in S of a regular oriented curve C on an oriented surface S. Let x(u,v) be an orthogonal parametrization of S in p and \phi(s) be the angle that x_{u} makes with \alpha???(s) in the given orientation. Then k_{g} = (k_{g})_{1} cos \phi + (k_{g})_{2} sin \phi + \frac{d\phi}{ds} where (k_{g})_{1} and (k_{g})_{2} are the geodesic curvatures of the coordinate curves v = const. and u = const. respectively.

(Prop 5) Given a point p \in S and a vector w \in T_{p}(S), w \neq 0 . There exists an \epsilon >0 and a unique parametrized geodesic \gamma : (-epsilon , \epsilon) \to S s.t. \gamma(0) = p , \gamma???(0) = w.

(subsection 4.5.) The Gauss-Bonnet Theorem and its Applications

(Def) Let \alpha : [0,l] \to S be a continuous map from the closed interval [0,l] into the regular surface S. We say that \alpha is a simple, closed, piecewise regular, parametrized curve if

\alpha(0) = \alpha(l).

t_{1} \neq t_{2}, t_{1}, t_{2} \in [0,l) implies that \alpha(t_{1}) \neq \alpha(t_{2}) .

There exists a subdivision 0 = t_{0} < t_{1} < \cdots < t_{k} < t_{k+1} = l of [0,l] s.t. \alpha is differentiable and regular in each [t_{i}, t_{i+1}] i = 0,???,k.

(Def) \alpha is a closed curve which fails to have a well-defined tangent line only at a finite number of points. The points \alpha(t_{i}) , i = 0,???,k are called the vertices of \alpha and the traces \alpha([t_{i}, t_{i+1}]) are called the regular arcs of \alpha. Assume now that S is oriented and let |\theta_{i}| , 0 < |\theta_{i}| \le \pi , be the smallest determination of the angle from \alpha???(t_{i} ??? 0) to \alpha???(t_{i} + 0) . we give \theta_{i} the sign of the determinant (\alpha???(t_{i} ??? 0) , \alpha???(t_{i} + 0), N). 

(Def) Let x : U \subset R^{2} \to S be a parametrization compatible with the orientation of S. Assume that U is homeomorphic to an open disk in the plane.

Let \alpha : [0,l] \to x(U) \subset S be a simple closed, piecewise regular, parametrized curve, with vertices \alpha(t_{i}) and external angles \theta_{i}, i = 0,???,k.

Let \phi_{i} : [t_{i}, t_{i+1}] \to R be differentiable functions which measure at each t \in [t_{i}, t_{i+1}] the positive angle from x_{u} to \alpha???(t) (section 4-4 Lem 1)

(Thm)(Of Turning Tangents) With the above notation \sum_{i = 0}^{k} (\phi_{i}(t_{i+1}) - \phi_{i}(t_{i})) + \sum_{i = 0}^{k} \theta_{i} = \mp 2\pi where the sign plus or minus depends on the orientation of \alpha.

(Def) Let x : U \subset R^{2} \to S be a parametrization of S compatible with its orientation and let R \subset x(U) be a bounded region of S. If f is a differentiable function on S, the integral \int \int_{x^{-1}(R)} f(u,v) \sqrt{EG ??? F^{2}} du dv does not depend on the parametrization x, chosen in the class of orientation of x. It is called the integral of f over the region R. Denote it by \int \int_{R} f d \sigma.

(Local)(Gauss Bonnet Theorem) Let x : U \to S be an orthogonal parametrization (that is , F = 0) , of an oriented surface S, where U \subset R^{2} is homeomorphic to an open disk and x is compatible with the orientation of S. Let R \subset x(U) be a simple region of S and let \alpha : I \to S be s.t. \partial R = \alpha(I). Assume that \alpha is positively oriented, parametrized by arc length s, and let \alpha(s_{0}), \alpha(s_{k}) and \theta_{0} , ???, \theta_{k} be, respectively, the vertices and the external angles of \alpha. Then \sum_{i = 0}^{k} \int_{s_{i}}^{s_{i+1}} k_{g}(s) ds + \int \int_{R}K d \sigma + \sum_{i = 0}^{k} \theta_{o} = 2 \pi where k_{g}(s) is the geodesic curvature of the regular arcs of \alpha and K is the Gaussian curvature of S.

(Def) Let S be a regular surface. A region R \subset S is said to be regular if R is compact and its boundary \partial R is the finite union of (simple) closed piecewise regular curves which do not intersect . We shall consider a compact surface as a regular region, the boundary of which is empty.

A simple region which has only three vertices with external angles \alpha_{i} \neq 0 , i = 1,2,3, is called a triangle.

A triangulation of a regular region R \subset S is a finite family \mathfrak{J} of triangles T_{i}, i = 1,???.,n, s.t.

\bigcup_{i=1}^{n} T_{i} = R.

If T_{i} \cap T_{j} \neq \empty, then T_{i} \cap T_{j} is either a common edge of T_{i} and T_{j} or a common vertex of T_{i} and T_{j}.

Given a triangulation \mathfrak{J} of a regular region R \subset S of a surface S, denote F the number of triangles(faces), by E the number of sides(edges), by V the number of vertices of the triangulation. The number F-E+V = \chi is called The Euler-Poincare characteristic of the triangulation.

(prop 1) Every regular region of a regular surface admits a triangulation.

(prop 2) Let S be an oriented surface and {x_{\alpha}}, \alpha \in A, a family of parametrizations compatible with the orientation of S. Let R \subset S be a regular region of S. Then there is a triangulation \mathfrak{J} of R s.t. every triangle T \in \mathfrak{J} is contained in some coordinate neighborhood of the family {x_{\alpha}} . Furthermore, If the boundary of every triangle of \mathfrak{J} is positively oriented , adjacent triangles determine opposite orientations in the common edge.

(Prop 3) If R \subset S is a regular region of a surface S, the Euler-Poincare characteristic does not depend on the triangulation of R. It is convenient, therefore, to denote it \chi(R).

(Prop 4) Let S \subset R^{3} be a compact connected surface; then one of the values 2,0,-2,???,-2n, ???, is assumed by the Euler-Poincare characteristic \chi(S). Furthermore, if S??? \subset R^{3} is another compact surface and \chi(S) = \chi(S???), then S is homeomorphic to S???.

(Prop 5) Let R \subset S be a regular region of an oriented surface S and let \mathfrak{J} be a triangulation of R s.t. every triangle T_{j} \in \mathfrak{J} , j = 1,???,k, is contained in a coordinate neighborhood x_{j}(U_{j}) of a family of parametrizations {x_{\alpha}} , \alpha \in A, compatible with the orientation of S. Let f be a differentiable function on S. the sum \sum_{j = 1}^{k} \int \int_{x_{j}^{-1}(T_{j}) f(u_{j}, v_{j}) \sqrt{E_{j}G_{j} ??? F_{j}^{2}} du_{j} dv_{j} does not depend on the triangulation \mathfrak{J} or on the family {x_{j}} of parametrizations of S.

(Global Gauss-Bonnet Thm) Let R \subset S be a regular region of an oriented surface and let C_{1}, ???, C_{n} be the closed, simple, piecewise regular curves which form the boundary \partial R of R. Suppose that each C_{i} is positively oriented and let \theta_{1}, ???, \theta_{p} be the set of all external angles of the curves C_{1}, ???, C_{n} . Then \sum_{i = 1}^{n} \int_{C_{i}} k_{g}(s) ds + \int \int_{R} K d \sigma + \sum_{i = 1}^{p} \theta_{i} = 2 \pi \chi(R), where s denotes the arc length of C_{i}, and the integral over C_{i} means the sum of integrals in every regular arc of C_{i}.

(Cor 1) If R is a simple region of S, then \sum_{i = 0}^{k} \int_{s_{i}}^{s_{i+1}} k_{g}(s) ds + \int \int_{R} k d \sigma + \sum_{i = 0}^{k} \theta_{i} = 2\pi.

(Cor 2) Let S be an orientable compact surface ; then \int \int_{S} K d \sigma = 2 \pi \chi(S).

(Prop) Assume Every piecewise regular curve in the plane(thus without self-intersections) is the boundary of a simple region.

A compact surface of positive curvature is homeomorphic to a sphere.

Let S be an orientable surface of negative or zero curvature. Then two geodesics \gamma_{1} and \gamma_{2} which start from a point p \in S cannot mmet again at a point q \in S in such a way that the traces of \gamma_{1} and \gamma_{2} constitute the boundary of a simple region R of S.

Let S be a surface homeomorphic to a cylinder with Gaussian curvature K < 0. Then S has at most one simple closed geodesic.

If there exist two simple closed geodesics \Gamma_{1} and \Gamma_{2} on a compact surface S of a positive curvature, then \Gamma_{1} and \Gamma_{2} intetsect.

Let \alpha : I \to R^{3} be a closed, regular, parametrized curve with nonzero curvature. Assume that the curve described by normal vector n(s) in the unit sphere S^{2} (the normal indicatrix) is simple. Then n(I) divides S^{2} in two regions with equal areas.

Let T be a geodesic triangle(that is, the sides of T are geodesics) in an oriented surface S. Let \theta_{1}, \theta_{2}, \theta_{3} be the external angles of T and let \phi_{1} = \pi - \theta_{1}, \phi_{2} = \pi -\theta_{2}, \phi_{3} = \pi - \theta_{3} be its interior angles. \int \int_{T} K d \sigma = - \pi + \sum_{i = 1}^{3} \phi_{i}. The sum of the interior angles , \sum_{i = 1}^{3} \phi_{i} of a geodesic triangle is Equal to \phi if K = 0, Greater than \pi if K > 0 , Smaller that \pi if K < 0.

Furthermore, the difference - \pi + \sum_{i = 1}^{3} \phi_{i} (the excess of T) is given precisely by \int \int_{T} K d \sigma. If K \neq 0 on T, this is the area of the image N(T) of T by the Gauss map N : S \to S^{2}. In other words, The excess of a geodesic triangle T is equal to the area of its spherical image N(T).

Vector fields on surfaces. Let v be a differentiable vector field on an oriented surface S. We say that p \in S is a singular point of v if v(p) = 0. The singular point p is isolated if there exists a neighborhood V of p in S such that v has no singular points in V other than p. let x : U \to S be an orthogonal parametrization at p = x(0,0) compatible with the orientation of S, and let \alpha : [0,l] \to S be a simple, closed, piecewise regular parametrized curve s.t. \alpha([0,l]) \subset x(U) is the boundary of a simple region R containing p as its only singular point. Let v = v(t), t \in [0,l] , be the restriction of v along \alpha, and let \phi = \phi(t) be some differentiable determination of the angle from x_{u} to v(t), given by (Lem 1 of Sec 4.4) Since \alpha is closed, there is an integer I defined by 2\pi I = \phi(l) - \phi(0) = \int_{0}^{t} \frac{d\phi}{dt} dt . I is called the index of v at p. (Poincare???s Theorem) The sum of the indices of a differentiable vector field v with isolated singular points on a compact surface S is equal to the Euler-Poincare characteristic of S.

(subsection 4.6.) The exponential map. Geodesic Polar Coordinates

(Lem 1) If the geodesic \gamma(t,v) is defined for t \in (-\epsilon , \epsilon) , then the geodesic \gamma (t, \lambda v) , \lambda \in R, \lambda \neq 0, is defined for t \in (-\epsilon / \lambda , \epsilon / \lambda) , and \gamma(t, \lambda v) = \gamma(\lambda t , v) .

(Def) If v = T_{p}(S), v \neq 0, is s.t. \gamma(|v| , v/|v|) = \gamma(1,v) is defined, we set exp_{p}(v) = \gamma(1,v) and exp_{p}(0) = p.

(prop 1) Given p \in S there exists an \epsilon >0 s.t. exp_{p} is defined and differentiable in the interior B_{e} of a disk of radius \epsilon of T_{p}(S), with center in the origin.

(prop 2) exp_{p} : B_{e} \subset T_{p}(S) \to S is a diffeomorphism in a neighborhood U \subset B , of the origin 0 of T_{p}(S).

(Def) V \subset S a normal neighborhood of p \in S if V is the image V = exp_{p}(U) of a neighborhood U of the origin of T_{p}(S) restricted to which exp_{p} is a diffeomorphism.

Since the exponential map at p \in S is a diffeomorphism on U, it may be used to introduce coordinates in V. The normal coordinates which correspond to a system of rectangular coordinates in the tangent plane T_{p}(S) . The geodesic polar coordinates which correspond to polar coordinates in the tangent plane T_{p}(S). 

polar coordinates in the plane are not defined in the closed half-line l which corresponds to \theta = 0. Set exp_{p}(l) = L . Since exp_{p} : U-l \to V-L is still a diffeomorphism, we may parametrize the points of V -L by the coordinates (\rho , \theta), which are called geodesic polar coordinates.

The images by exp_{p} : U \to V of circles in U centered in 0 will be called geodesic circles of V, and the imagnes of exp_{p} of the lines through 0 will be called radial geodesics of V. 

(prop 3) Let x : U -l \to V-L be a system of geodesic polar coordinates (\rho , \theta). Then the coefficients E = E(\rho, \theta) , F = F(\rho, \theta) , and G = G(\rho, \theta) of the first fundamental form satisfy the conditions E = 1, F = 0, \lim_{\rho \to 0} G = 0, \lim_{\rho \to 0} (\sqrt(G))_{\rho} = 1.

(Minding)(Thm) Any two regular surfaces with the same constant Gaussian curvature are locally isometric. More precisely, Let S_{1}, S_{2} be two regular surfaces with the same constant curvature K. Choose points p_{1} \in S_{1} , p_{2} \in S_{2} , and orthonormal basis {e_{1}, e_{2}} \in T_{p_{1}} (S_{1}) , [f_{1}, f_{2}] \in T_{p_{2}} (S_{2}) . Then there exists neighborhoods V_{1} of p_{1} , V_{2} of p_{2} and an isometry \psi : V_{1} \to V_{2} s.t. d\psi(e_{1}) = f_{1}, d\psi(e_{2}) = f_{2}.

(prop 4) Let p be a point on a surface S. Then, there exists a neighborhood W \subset S of p s.t. if \gamma : I \to W is a parametrized geodesic with \gamma(0)= p, \gamma(t_{1}) = q, t_{1} \in I, and \alpha : [0,t_{1}] \to S is a parametrized regular curve joining p to q, we have l_{\gamma} \le l_{\alpha} , where I_{\alpha} denotes the length of the curve \alpha. Moreofer, if I_{\gamma} = I_{\alpha} , then the trace of \alpha coincides with the trace of \alpha between p and q.

(Prop 5) Let \alpha : I \to S be a regular parametrized curve with a parameter proportional to arc length. Suppose that the arc length of \alpha between any two points t, \tau \in I, is smaller than or equal to the arc length of any regular parametrized curve joining \alpha(t) to \alpha(\tau) . Then \alpha is a geodesic.

(Thm 1) Let S a regular surface. Given p \in S there exist numbers \epsilon_{1} >0 , \epsilon_{2} >0 and a differentiable map \gamma : (-\epsilon_{2}, \epsilon_{2}) \times B_{\epsilon_{1}} \to S, B_{\epsilon_{1}} \subset T_{p}(S) s.t. for v \in B_{\epsilon_{1}} , v \neq 0 , t \in (-\epsilon_{2}, \epsilon_{2}) the curve t \in \gamma(t,v) is the geodesic of S with \gamma(0,v) = p , \gamma???(0,v) = v and for v = 0 \gamma(t,0) = p.

(Thm 1a.) Given p \in S, there exists positive numbers \epsilon, \epsilon_{1}, \epsilon_{2} and a differentiable map \gamma : (-\epsilon_{2}, \epsilon_{2}) \times \mathcal{U} \to S where \mathcal{U} = {(q,v) ; q \in B_{\epsilon}(p), v \in B_{\epsilon_{1}}(0) \subset T_{q}(S)}, s.t. \gamm(t,q,0) =q, and for v \neq 0 the curve t \to \gamma(t,q,v), t \in (-\epsilon_{2}, \epsilon_{2}) is the geodesic of S with \gamma(0,q,v) = q, \gamma???(0,q,v) = v.

(prop 1) Given p \in S there exist a neighborhood W of p in S and a number \delta >0 s.t. for every q \in W, exp_{q} is a diffeomorphism on B_{\delta}(0) \subset T_{q}(S) and exp_{q}(B_{\delta}(0)) \supset W ; that is, W is a normal neighborhood of all its points.

(prop 2) Let \alpha : I \to S be a parametrized, piecewise regular curve s.t. in each regular arc the parameter is proportional to the arc length. Suppose that the arc length between any two of this points is smaller than or equal to the arc length of any parametrized regular curve joining these points. Then \alpha is a geodesic ; in particular, \alpha is regular everywhere.

(prop 3) For each point p \in S there exists a positive number \epsilon with the following property ; If a geodesic \gamma(t) is tangent to the geodesic circle S_{r}(p), r < \epsilon , at \gamma(0) , then for t \neq 0 small, \gamma(t) is outside B_{t}(p) .

(Existence of Convex neighborhoods) (prop 4) For each point p \in S there exists a number c > 0 s.t. B_{c}(p) is convex ; that is, any two points of B_{c}(p) can be joined by a unique minimal geodesic in B_{c}(p) .

