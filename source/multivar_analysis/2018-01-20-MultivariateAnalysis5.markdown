---



layout: post



title : (Calculus on Manifolds) Integration on Manifolds



date : 2018-01-20 11:56:04 +0900



---

(Section 5) Integration on Manifolds

(subsection) Manifolds

(Def) If U and V are open sets in \mathbf{R}{n}, a differentiable function h : U \to V with a differentiable inverse h^{-1} : V \to U will be called a diffeomorphism.

‘Differentiable’ henceforth means C^{\infty}.

(Def) A subset M of \mathbf{R}^{n} is called a k-dimensional manifold (in \mathbf{R}^{n}) if for every point x \in M the following condition is satisfied :

(M) There is an open set U containing x, an open set V \subset \mathbf{R}^{n}, and a diffeomorphism h : U \to V s.t. h(U \cap M) = V \cap (\mathbf{R}^{k} \times {0}) = {y \in V : y^{k+1} = \cdots = y^{n} = 0}.

We say U \cap M is up to diffeomorphism \mathbf{R}^{k} \times {0}.

(Def) n-sphere S^{n}, defined as {x \in \mathbf{R}^{n+1} : |x| = 1}.

(Thm 5.1) Let A \subset \mathbf{R}^{n} be open and let g : A \to \mathbf{R}^{p} be a differentiable function s.t. g’(x) has rank p whenever g(x) = 0. Then g^{-1} (0) is an (n-p)-dimensional manifold in \mathbf{R}^{n}.

(Thm 5.2) A subset M of \mathbf{R}^{n} is a k-dimensional manifold iff for each point x \in M the following coordinate condition is satisfied :

(C) There is an open set U containing x, an open set W \subset \mathbf{R}^{k}, and a 1-1 differentiable function f : W \to \mathbf{R}^{n} s.t. f(W) = M \cap U, f’(y) has a rank k for each y \in W, f^{-1} : f(W) \to W is continuous. 

such a function f is called a coordinate system around x.

(Def) The half-space H^{k} \subset \mathbf{R}^{k} is defined as {x \in \mathbf{R}^{k} : x^{k} \ge 0}. A subset M of \mathbf{R}^{n} is a k-dimensional manifold-with-boundary if for every point x \in M either condition (M) or the following condition is satisfied:

(M’) There is an open set U containing x, an open set V \subset \mathbf{R}^{n}, and a diffeomorphism h : U \to V s.t. h(U \cap M) = V \cap (H^{k} \times {0}) = {y \in V : y^{k} \ge 0 and y^{k+1} = \cdots = y^{n} = 0}

and h(x) has kth component 0.

(Def) The set of all points x \in M for which condition M’ is satisfied is called the boundary of M and denoted \partial M.

(subsection) Fields and forms on Manifolds

(Def) Let M be a k-dimensional manifold in \mathbf{R}^{n} and let f : W \to \mathbf{R}^{n} be a coordinate system around x = f(a). Since f’(a) has rank k, the linear transformation f_{*} : \mathbf{R}^{k}_{a} \to \mathbf{R}^{n}_{x} is 1-1, and f_{*}(\mathbf{R}^{k}_{a}) is a k-dimensional subspace of \mathbf{R}^{n}_{x}. If g: V \to \mathbf{R}^{n} is another coordinate system, with x = g(b), then g_{*} (\mathbf{R}^{k}_{b}) = f_{*}(f^{-1} \bullet g)_{*}(\mathbf{R}^{k}_{b}) = f_{*}(\mathbf{R}^{k}_{a}). Thus the k-dimensional subspace f_{*}(\mathbf{R}^{k}_{b}) does not depend on the coordinate system f. This subspace is denoted M_{x}, and is called the tangent space of M at x.

a natural inner product T_{x} on M_{x}, induced by that on \mathbf{R}^{n}_{x} : if v,w \in M_{x} define T_{x}(v,w) = \langle v,w \rangle_{x}.

(prop) Suppose that A is an open set containing M, and F is differentiable vector field on A s.t. F(x) \in M_{x} for each x \in M. If f: W \to \mathbf{R}^{n} is a coordinate system, there is a unique (differentiable) vector field G on W s.t. f_{*}(G(a)) = F(f(a)) for each a \in W.

(Def) Consider a function F which merely assigns a vector F(x) \in M_{x} for each x \in M ; such a function is called a vector field on M.

define F to be differentiable if G corresponding to F is differentiable.

(Def) a function \omega which assigns \omega(x) \in \Lambda^{p}(M_{x}) for each x \in M is called a p-form on M. 

If f : W \to \mathbf{R}^{n} is a coordinate system, then f^{*} \omega is a p-form on W; we define \omega to be differentiable if f^{*} \omega is.

(Thm 5.3) There is a unique (p+1)-form d\omega on M s.t. for every coordinate system f : W \to \mathbf{R}^{n} we have f^{*}(d\omega) = d(f^{*} \omega).

(Def) when choosing an orientation \mu_{x} for each tangent space M_{x} of a manifold M, such choices are called consistent provided that for every coordinate system f : W \to \mathbf{R}^{n} and a,b \in W the relation [f_{*} ((e_{1})_{a}), \cdots, f_{*}((e_{k})_{a})] = \mu_{f(a)} holds iff [f_{*} ((e_{1})_{b}), \cdots, f_{*}((e_{k})_{b})] = \mu_{f(b)}.

(Def) Suppose orientations \mu_{x} have been chosen consistently. If f: W \to \mathbf{R}^{n} is a coordinate system s.t. [f_{*} ((e_{1})_{a}), \cdots, f_{*}((e_{k})_{a})] = \mu_{f(a)} for one, and hence for every a \in W, then f is called orientation-preserving.

If f is not orientation-preserving and T: \mathbf{R}^{k} \to \mathbf{R}^{k} is a linear transformation with det T = -1, then f \bullet T is orientation-preserving. Therefore there is an orientation-preserving coordinate system around each point.

(Def) A manifold for which orientations \mu_{x} can be chosen consistently is called orientable, and a particular choice of the \mu_{x} is called an orientation \mu of M. A manifold together with an orientation \mu is called an oriented manifold.

(prop) If M is a k-dimensional manifold-with-boundary and x \in \partial M, then (\partial M)_{x} is a (k-1)-dimensional subspace of the k-dimensional vector space M_{x}. Thus there are exactly two unit vectors in M_{x} which are perpendicular to (\partial M)_{x}.

(Def) If f : W \to \mathbf{R}^{n} is a coordinate system with W \subset H^{k} and f(0) = x, then only one of these unit vectors is f_{*}(v_{0}) for some v_{0} with v^{k} <0. This unit vector is called the outward unit normal n(x).

(Def) Suppose that \mu is an orientation of a k-dimensional manifold-with-boundary M. if M is orientable, \parital M is also orientable, and an orientation \mu for M determines an orientation \partial \mu for \partial M, called the induced orientation.

If we apply these definitions to H^{k} with the usual orientation, we find that the induced orientation on \mathbf{R}^{k-1} = {x \in H^{k} : x^{k} = 0} is (-1)^{k} times the usual orientation.

(Def) If M is an oriented (n-1)-dimensional manifold in \mathbf{R}^{n}, a substitute for outward unit normal can be defined. If [v_{1}, \cdots, v_{n-1}] = \mu_{x} , we choose n(x) in \mathbf{R}^{n}_{x} so that n(x) is a unit vector perpendicular to M_{x} and [n(x), v_{1}, \cdots, v_{n-1}] is the usual orientation of \mathbf{R}^{n}_{x} . We still call n(x) the outward unit normal to M (determined by \mu).

Conversely, if a continuous family of unit normal vectors n(x) is defined on all of M, then we can determine the orientation of M.

(subsection) Stoke’s Theorem on Manifolds

(Def) If \omega is a p-form on a k-dimensional manifold-with-boundary M and c is a singular p-cube in M, we define \int_{c} \omega = \int_{[0,1]^{p}} c^{*} \omega.

In the case p = k there is an open set W \supset [0,1]^{k} and a coordinate system f : W \to \mathbf{R}^{n} s.t. c(x) = f(x) for x \in [0,1]^{k};

if M is oriented, the singular k-cube c is called orientation-preserving if f is.

(Thm 5.4) If c_{1}, c_{2} : [0,1]^{k} \to M are two orientation-preserving singular k-cubes in the oriented k-dimensional manifold M and \omega is a k-form on M s.t. \omega = 0 outside of c_{1}([0,1]^{k}) \cap c_{2}([0,1]^{k}), then \int_{c_{1}} \omega = \int_{c_{2}} \omega.

(Def) Let \omega be a k-form on an oriented k-dimensional manifold M. If there is an orientation-preserving singular k-cube c in M s.t. \omega = 0 outside of c([0,1]^{k}) , we define \int_{m} \omega = \int_{c} \omega. 

\int_{M} \omega does not depend on the choice of c.

(prop) Suppose noe that \omega is an arbitrary k-form on M. There is an open cover \mathcal{O} of M s.t. for each U \in \mathcal{O} there is an orientation-preserving singular k-cube c with U \subset c([0,1]^{k}) .

(Def) Let \Phi be a partition of unity for M subordinate to this cover. We define \int_{M} \omega = \sum_{\phi \in \Phi} \int_{m} \phi \cdot \omega  provided the sum converges as describes in the discussion preceding Theorem 3-12.

(Def) All our definitions could have been given for a k-dimensional manifold-with-boundary M with orientation \mu.

(Stokes’ Theorem) (Thm 5.5) If M is a compact oriented k-dimensional manifold-with-boundary and \omega is a (k-1)-form on M, then \int_{m} d\omega = \int_{\partial M} \omega. (Here \partial M is given the induced orientation).

(subsection) The Volume element

(Def) Let M be a k-dimensional manifold (or manifold-with-boundary) in \mathbf{R}^{n}, with an orientation \mu. If x \in M, then \mu_{x} and the inner product T_{x} we defined previously determine a volume element \omega(x) \in \Lambda^{k}(M_{x}) . We obtain a nowhere-zero k-form \omega on M, which is called the volume element on M (determined by \mu) and denoted dV. 

(Def) the volume of M is defined as \int_{M} dV, provided this integral exists, which is certainly the case if M is compact.

volume is called length or surface area for one-and two-dimensional manifolds, and dV is denoted ds (the element of length) or dA (or dS, the element of surface area).

(Thm 5.6) Let M be an oriented two-dimensional manifold (or manifold-with-boundary) in \mathbf{R}^{3} and let n be the unit outward normal. Then 

dA = n^{1} dy \wedge dz + n^{2} dz \wedge dx + n^{3} dx \wedge dy.

Moreover, on M we have

n^{1} dA = dy \wedge dz.

n^{2} dA = dz \wedge dx.

n^{3} dA = dx \wedge dy.

(prop) If c : [0,1] to \mathbf{R}^{n} is differentiable and c([0,1]) is a one-dimensional manifold-with-boundary, the length of c([0,1]) is the least upper bound of the lengths of inscribed broken lines. For c:[0,1]^{2} \to \mathbf{R}^{n}, it is not true.

(subsection) The classical theorems

(Green’s Theorem) (Thm 5.7) Let M \subset \mathbf{R}^{2} be a compact two-dimensional manifold-with-boundary. Suppose that \alpha, \beta : M \to \mathbf{R} are differentiable. Then \int_{\partial M} \alpha dx + \beta dy = \int_{M} (D_{1} \beta – D_{2} \alpha) dx \wedge dy = \int_{M} \int (\frac{\partial \beta}{\partial x}- \frac{\parital \alpha }{\partial y}) dx dy.

(Divergence Theorem) (Thm 5.8) Let M \subset \mathbf{R}^{3} be a compact three-dimensional manifold-with-boundary and n the unit outward normal on \partial M. Let F be a differentiable vector field on M. Then \int_{m} div F dV = \int_{\partial M} \langle F, n \rangle dA.

This equation is also written in terms of three differentiable functions \alpha, \beta, \gamma : M \to \mathbf{R} :

\int \int_{M} \int (\frac{\partial \alpha }{\partial x} + \frac{\partial \beta}{\partial y} +\frac{\partial \gamma}{\partial z}) dV = \int_{\partial M} \int (n^{1} \alpha +n^{2} \beta + n^{3} \gamma) dS.

(Stokes’ Theorem) (Thm 5.9) Let M \subset \mathbf{R}^{3} be a compact oriented two-dimensional manifold-with-boundary and n the unit outward normal on M determined by the orientation of M. Let \partial M have the induced orientation. Let T be the vector field on \partial M with ds(T) = 1 and let F be a differentiable vector field in an open set containing M. Then \int_{M} \langle ( \nabla \times F), n \rangle dA = \int_{\partial M} \langle F, T \rangle ds.

This equation is sometimes written 

\int_{\partial M} \alpha dx + \beta dy + \gamma dz = \int_{M} \int [n^{1} (\frac{\partial \gamma }{\partial y } - \frac{\partial \beta }{\partial z}) + n^{2}(\frac{\partial \alpha }{\partial z} - \frac{\partial \gamma }{\partial x })  + n^{3}(\frac{\partial \beta }{\partial x } - \frac{ \partial \alpha }{\partial y})  ] dS.

(Def) If F(x) is the velocity vector of a fluid at x (at some time) then \int_{\partial M} \langle F,n \rangle dA is the amount of fluid ‘diverging’ from M. Consequently the condition div F = 0 expresses the fact that the fluid is incompressible. If M is a disc, the \int_{\partial M} \langle F, T \rangle ds mesures the amount that the fluid curls around the center of the disc. If this is zero for all discs, then \nabla \times F = 0 , and the fluid is called irroational.



