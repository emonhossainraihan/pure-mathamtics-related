---



layout: post



title : (Differential Geometry) Regular Surfaces



date : 2018-01-20 12:53:04 +0900



---

Section 2) Regular Surfaces

(subsection 2.2) Regular Surfaces : Inverse Images of Regular Values

(Def 1) A subset S \subset R^{3} is a regular surface if, for each p \in S, there exists a neighborhood V in R^{3} and a map \mathbf{x} : U \to V \cap S of an open set U \subset R^{3} s.t.

\mathbf{x} is differentiable. This means that if we write \mathbf{x} (u,v) = (x(u,v), y(u,v), z(u,v)) , (u, v) \in U, the functions x(u,v) , y(u,v), z(u,v) have continuous partial derivatives of all orders in U.

\mathbf(x) is homeomorphism ; \mathbf{x} has an inverse \mathbf{x}^{-1} : V \cap S \to U which is continuous ; that is , \mathbf{x}^{-1} is the restriction of a continuous map F : W \subset R^{3} \to R^{2} defined on an open set W containing V \cap S.

(The regularity condition) For each q \in U, the differential d\mathbf{x}_{q} : R^{2} \to R^{3} is one-to-one; d\mathbf{x}_{q} = \begin{pmatrix} \frac{\partial x}{\partial u} &\frac{\partial x}{\partial v} \\ \frac{\partial y}{\partial u} & \frac{\partial y}{\partial v} \\ \frac{\partial z}{\partial u}& \frac{\partial z}{\partial v} \end{pmatrix} \right|_{q = (u_{0}, v_{0}) each column is linearly independent.

This mapping \mathbf{x} is called a parametrization or a system of (local) coordinates in (a neighborhood of) p. The neighborhood V \cap S of p in S is called a coordinate neighborhood.

(Prop 1) If f : U \to R is a differentiable function in an open set U of R^{2}. then the graph of f, that is , the subset of R^{3} given by (x,y,f(x,y)) for (x,y) \in U, is a regular surface.

(Def 2) Given a differential map F : U \subset R^{n} \to R^{m} defined in an open set U of R^{n} we say that p \in U is a critical point of F if the differential dF_{p} : R^{n} \to R^{m} is not a surjective mapping. The image F(p) \in R^{m} of a critical point is called a critical value of F. A point of R^{m} which is not a critical value is called a regular value of F. 

(prop 2) If f : U \subset R^{3} \to R is a differentiable function and a \in f(U) is a regular value of f, then f^{-1}(a) is a regular surface in R^{3}.

(prop 3) Let S \subset R^{3} be a regular surface and p \in S. Then there exists a neighborhood V of p in S s.t. V is the graph of a differentiable function which has one of the following three forms : z = f(x,y) , y = g(x,z), x = h(y,z).

(prop 4) Let p \in S be a point of a regular surface S and let \mathbf{x} : U \subset R^{2} \to R^{3} be a map with p \in \mathbf{x}(U) \subset S s.t. conditions 1 and 3 of (Def 1) holds. Assume that \mathbf{x} is one-to-one. then \mathbf{x}^{-1} is continuous.

(subsection 2.3.) Change of Parameters : Differentiable Function on Surfaces

(Change of Parameters)(Prop 1) Let p be a point of a regular surface S , and let \mathbf{X} : U \subset R^{2} \to S, y : V \subset R^{2} \to S be two parametrization of S s.t. p \in \mathbf{x}(U) \cap y(V) = W. Then the “Change of coordinates” h = \mathbf{x}^{-1} \bullet y : y^{-1}(W) \to \mathbf{x}^{-1}(W) is a diffeomorphism ; that is , h is differentiable and has a differentiable inverse h^{-1}.

(Def 1) Let f : V \subset S \to R be a function defined in an open subset V of a regular surface S. Then f is said to be differentiable at p \in V if, for some parametrization x : U \subset R^{2} \to S with p \in x(U) \subset V, the composition f \bullet x : U \subset R^{2} \to R is differentiable at x^{-1}(p) . f is differentiable in V if it is differentiable at all points of V. 

(Def) Two regular surfaces S_{1}, S_{2} are diffeomorphic if there exists a differentiable map \phi : S_{1} \to S_{2} with a differentiable inverse \phi^{-1} : S_{2} \to S_{1} . such a \phi is called a diffeomorphism from S_{1} to S_{2}.

(Def 2) A parametrized surface x : U \subset R^{2} \to R^{3} is a differentiable map x from an open set U \subset R^{2} into R^{3}. The set x(U) \subset R^{3} is called the trace of x. x is regular if the differential dx_{q} : R^{2} \to R^{3} is one-to-one for all q \in U (the vectors \partial x / \partial u , \partial x / \partial v are linearly independent for all q \in U) . A point p \in U where dx_{q} is not one-to-one is called a singular point of x.

(Prop 2) Let x : U \subset R^{2} \to R^{3} be a regular parametrized surface and let q \in U. Then there exists a neighborhood V of q in R^{2} s.t. x(V) \subset R^{3} is a regular surface.

(subsection 2.4.) The tangent plane ; The differential of a map

(prop 1) Let x : U \subset R^{2} \to S be a parametrization of a regular surface S and let q \in U. The vector subspace of dimension 2, dx_{q} (R^{2}) \subset R^{3} coincides with the set of tangent vectors to S at x(q).

The plane dx_{q}(r^{2}) , which passes through x(q) = p , which does not depend on the parametrization x, will be called the tangent plane to S at p and will be denoted T_{p}(S).

(Def) The coordinates of a vector w \in T_{p}(S) in the basis associated to a parametrization x are determined as follows. w is the velocity vector \alpha’(0) of a curve \alpha = x \bullet \beta, where \beta : (-\epsilon, \epsilon) \to U is given by \beta(t) = (u(t), v(t)) , with \beta(0) = q = x^{-1}(p).

(prop2) In the discussion above, given w, the vector \beta ‘(0) does not depend on the choice of \alpha. The map d\phi_{p} : T_{p}(S_{1}) \to T_{\phi(p)}(S_{2}) defined by d\phi_{p}(w) = \beta’(0) is linear. 

(Def) The linear map d\phi_{p} defined by (prop2) is called the differential of \phi at p \in S_{1}. In a similar way we define the differential of a (differentiable) function f : U \subset S \to R at p \in U as a linear map df_{p} : T_{p}(S) \to R. 

A mapping \phi : U \subset S_{1} \to S_{2} is a local diffeomorphism at p \in U if there exists a neighborhood V \subset U of p s.t. \phi restricted to V is a diffeomorphism onto an open set \phi(V) \subset S_{2}.

(prop 3) If S_{1} and S_{2} are regular surfaces and \phi : U \subset S_{1} \to S_{2} is a differentiable mapping of an open set U \subset S_{1} s.t. the differential d\phi_{p} of \phi at p \in U is an isomorphism, then \phi is a local diffeomorphism at p.

(subsection 2.5.) The First Fundamental form ; Area

(Def) The natural Inner product of R^{3} \supset S induces on each tangent plane T_{p}(S) of a regular surface S an inner product, to be denoted by < , >_{p} : If w_{1}, w_{2} \in T_{p} (S) \subset R^{3} , then <w_{1}, w_{2}>_{p} is equal to the inner product of w_{1} and w_{2} as vectors in R^{3}. There corresponds a quadratic form I_{p} : T_{p}(S) \to R given by I_{p}(w) = <w,w>_{p} = |w|^{2} \ge 0.

(Def 1) The quadratic form I_{p} on T_{q}(S), defined as above, is called the first fundamental form of the regular surface S \subset R^{3} at p \in S.

(Def) For a regular surface S, a (regular) domain of S is an open and connected subset of S s.t. its boundary is the image of a circle by a differentiable homeomorphism which is regular (that is, its differential is nonzero) except at a finite number of points. A region of S is the union of a domain with its boundary. A region of S \subset R^{3} is bounded if it is contained in some ball of R^{3}.

(Def 2) Let R \subset S be a bounded region of a regular surface contained in the coordinate neighborhood of the parametrization x : U \subset R^{2} \to S. The positive number \int \int_{Q} |x_{u} \wedge x_{v}| du dv = A(R), Q = x^{-1}(R) is called the area of R.

(subsection 2.6.) Orientation of Surfaces

(Def 1) A regular surface S is called orientable if it is possible to cover it with a family of coordinate neighborhoods in such a way that if a point p \in S belongs to two neighborhoods of this family, then the change of coordinates has positive Jacobian at p. The choice of such a family is called an orientation of S, and S, in this case, is called oriented. If such a choice is not possible, the surface is called nonorientable.

If a regular surface can be covered by two coordinate neighborhoods whose intersection is connected, then the surface is orentable.

(Prop1) A regular surface S \subset R^{3} is orientable iff there exists a differentiable field of unit normal vectors N : S \to R^{3} on S.

(prop 2) If a regular surface is given by S = {(x,y,z) \in R^{3} : f(x,y,z) = a}, where f : U \subset R^{3} \to R is differentiable and a is a regular value of f, then S is orientable.

(subsection 2.7.) A Characterization of Compact Orientable Surfaces

(Def) Let S \subset R^{3} be an orientable surface. On the normal line through p \in S, an open interval I_{p} around p of length, say, 2 \epsilon_{p} (\epsilon_{p} varies with p) in such a way that if p \neq q \in S, then I_{p} \cap I_{q} = \empty. Thus, the union \bigcup I_{p} , p \in S, constitutes an open set V of R^{3}, which contains S and has the property that through each point of V there passes a unique normal line to S; V is then called a tubular neighborhood of S.

(Prop 1) Let S be a regular surface and x : U \to S be a parametrization of a neighborhood of a point p = x(u_{0}, v_{0}) \in S. Then there exists a neighborhood W \subset x(U) of p in S and a number \epsilon >0 s.t. the segments of the normal lines passing through points q \in W, with center at q and length 2 \epsilon, are disjoint. (That is, W has a tubular neighborhood.)

(prop 2) Assume the existence of a tubular neighborhood V \subset R^{3} of an orientable surface S \subset R^{3}, and choose an orientation for S. Then the function g : V \to R , defined as the oriented distance form a point of V to the foot of the unique normal line passing through this point, is differentiable and has zero as a regular value.

(Bolzano-Weierstrass) (Prop 1) Let A \subset R^{3} be a compact set. Then every infinite subset of A has at least one limit point in A.

(Heine-Borel) (Prop 2) Let A \subset R^{3} be a compact set and {U_{\alpha}} be a family of open sets of A s.t. \bigcup_{\alpha} U_{\alpha} = A. Then it is possible to choose a finite number U_{k_{1}}, U_{k_{2}}, …, U_{k_{n}} of U_{\alpha} s.t. \bigcup U_{k_{i}} = A , i = 1,…,n.

(Lebesque) (prop 3) Let A \subset R^{3} be a compact set and {U_{\alpha}} be a family of open sets of A s.t. \bigcup_{\alpha} U_{\alpha} = A. Then there exists a number \delta >0 (The Lebesgue number of the family {U_{\alpha}}) s.t. whenever two points p,q \in A are at a distance d(p,q) < \delta then p and q belong to some U_{\alpha}.

(Prop 3) Let S \subset R^{3} be a regular, compact, orientable surface. Then there exists a number \epsilon >0 s.t. whenever p, q \in S the segments of the normal lines of length 2 \epsilon , centered in p and q, are disjoint( that is, S has a tubular neighborhood).

(Thm) Let S \subset R^{3} be a regular compact orientable surface. Then there exists a differentiable function g : V \to R , defined in an open set V \subset R^{3}, with V \supset S (precisely a tubular neighborhood of S), which has zero as a regular value and is such that S = g^{-1}(0). 

(subsection 2.8.) A geometric definition of Area

(Def) For a region R \subset S we define a partition \mathcal{P} of R into a finite number of regions R_{i}, that is, we write R = \bigcup_{i} R_{i} , where intersection of two such regions R_{i} is either empty or made up of boundary points of both regions. The diameter of R_{i} is the supremum of the distances (in R^{3}) of any two points in R_{i}. The largest diameter of the R_{i}’s of a given partition \mathcal{P} is called the norm \mu of \mathcal{P}. If we take a partition of each R_{i}, we obtain a second partition of R, which is said to refine \mathcal{P}.

Given a partition R = \bigcup_{i} R_{i} of R, we choose arbitrarily points p_{i} \in R_{i} and project R_{i} onto the tangent palne at p_{i} in the direction of normal line at p_{i}; this projection is denoted by \bar{R} and its area b A(\bar{R}) . 

If, by choosing partitions \mathcal{P}_{1}, …, \mathcal{P}_{n}, … more and more refined s.t. the norm \mu_{n} of \mathcal{P}_{n} converges to zero, there exists a limit of \sum_{i} A(\bar{R}_{i}) and this limit is independent of all choices. R has an area A(R) defined by A(R) = \lim_{\mu_{n} \to 0} \sum_{i} A(\bar{R_{i}}).

(Prop 1) Let x : U \to S be a coordinate system in a regular surface S and let R = x(Q) be a bounded region of S contained in x(U). Then R has an area given by A(R) = \int \int_{Q} |x_{u} \wedge x_{v}| du dv.

(Appendix) A brief review of continuity and Differentiability

(Prop 1) F : U \subset R^{n} \to R^{m} is continuous iff each component function f_{i} : U \subset R^{n} \to R , i = 1,…,m, is continuous.

(Prop 2) A map F : U \subset R^{n} \to R^{m} is continuous at p \in U iff , given a neighborhood V of F(p) in R^{m} there exists a neighborhood W of p in R^{n} s.t. F(W) \subset V.

(Prop 3) Let F : U \subset R^{n} \to R^{m} and G : V \subset R^{m} \to R^{k} be continuous maps, where U and V are open sets s.t. F(U) \subset V. Then G \bullet F : U \subset R^{n} \to R^{k} is a continuous map.

(Intermediate Value Theorem) (Prop 4) Let f : [a,b] \to R be a continuous function defined on the closed interval [a,b] . Assume that f(a) and f(b) have opposite signs; that is, f(a)f(b) < 0. Then there exists a point c \in (a,b) s.t. f(c) = 0.

(prop 5) Let f : [a,b] be a continuous function defined in the closed interval [a,b]. Then f reaches its maximum and its minimum in [a,b]; that is, there exists points x_{1}, x_{2} \in [a,b] s.t. f(x_{1}) \le f(x) \le f(x_{2}) for all x \in [a,b].

(Heine-Borel) (prop 6) Let [a,b] be a closed interval and let I_{\alpha} , \alpha \in A be a collection of open intervals in [a,b] s.t. \bigcup_{\alpha} I_{\alpha} = [a,b] . Then it is possible to choose a finite number I_{k_{1}}, I_{k_{2}}, …, I_{k_{n}} of I_{\alpha} s.t. \bigcup I_{k_{i}} = I, i = 1,…,n.

(subsection B) Differentiability in R^{n}

(Def 1) Let F : U \subset R^{n} \to R^{m} be a differentiable map. To each p \in U we associate a linear map dF_{p} : R^{n} \to R^{m} which is called the differential of F at p and is defined as follows. Let w \in R^{n} and let \alpha : (- \epsilon, \epsilon) \to U be a differentiable curve s.t. \alpha(0) = p, \alpha’(0) = w. By the chain rule, the curve \beta = F \bullet \alpha : (-\epsilon , \epsilon) \to R^{m} is also differentiable. Then dF_{p}(w) = \beta’(0) .

(prop 7.) The above definition of dF_{p} does not depend on the choice of the curve which passes through p with tangent vector w, and dF_{p} is , in fact, a linear map.

(The Chain rule for Maps) (Prop 8) Let F : U \subset R^{n} \to R^{m} and G : V \subset R^{m} \to R^{k} be differentiable maps, where U and V are open sets s.t. F(U) \subset V. Then G \bullet F : U \to R^{k} is a differentiable map, and d(G \bullet F)_{p} = dG_{F(p)} \bullet dF_{p} , p \in U.

(Prop 9) Let f : U \subset R^{n} \to R be a differentiable function defined on a connected open subset U of R^{n}. Assume that df_{p} : R^{n} \to R is zero at every point p \in U. Then f is constant on U.

(Inverse Function Theorem) Let F : U \subset R^{n} \to R^{n} be a differentiable mapping and suppose that at p \in U the differential dF_{p} : R^{n} \to R^{n} is an isomorphism. Then there exists a neighborhood V of p in U and a neighborhood W of F(p) in R^{n} s.t. F:V \to W has a differentiable inverse F^{-1} : W \to V.

(Def) A differentiable mapping F : V \subset R^{n} \to W \subset R^{n}, where V and W are open sets, is called a diffeomorphism of V with W if F has a differentiable inverse.

