---



layout: post



title : Integration on Chains



date : 2018-01-20 11:55:04 +0900



---

(Section 4) Integration on Chains

(subsection) Algebraic Preliminaries

(Def) If V is a vector space (over \mathbf{R}), we will denote the k-fold product V \times \cdots \times V by V^{k} . 

A function T : V^{k} \to \mathbf{R} is called multilinear if for each i with 1 \le i \le k we have T(v_{1} , \cdots , v_{i} + v_{i}’ , \cdots , v_{k}) = T(v_{1} , \cdots, v_{i} , \cdots, v_{k} ) + T(v_{1} , \cdots, v_{i}’ , \cdots, v_{k} ) , T(v_{1}, \cdots, av_{i} , \cdots, v_{k}) = aT(v_{1}, \cdots, v_{i} , \cdots, v_{k}) .

(Def) A multilinear function T : V^{k} \to \mathbf{R} is called a k-tensor on V and the set of all k-tensors, denoted \mathcal{J}^{k} (V) and a \in \mathbf{R} we define (S+T) (v_{1}, \cdots, v_{k}) = S(v_{1}, \cdots, v_{k}) + T(v_{1}, \cdots, v_{k}) , (aS)(v_{1}, \cdots, v_{k}) = a \cdot S(v_{1} , \cdots, v_{k} ) .

(Def) If S \in \mathcal{J}^{k} (V) and T \in \mathcal{J}^{l} (V) , we define the tensor product S \otimes T  \in \mathcal{J}^{k+1} (V) by S \otimes T (v_{1}, \cdots, v_{k} , v_{k+1}, \cdots, v_{k+l}) = S(v_{1}, \cdots, v_{k}) \cdot T(v_{k+1}, \cdots, v_{k+l}) .

(prop)

(S_{1} + S_{2}) \otimes T = S_{1} \otimes T + S_{2} \otimes T,

S \otimes (T_{1} + T_{2}) = S \otimes T_{1} + S \otimes T_{2},

(aS) \otimes T = S \otimes (aT) = a(S \otimes T),

(S \otimes T) \otimes U = S \otimes (T \otimes U).

(Thm 4.1) Let v_{1} , \cdots, v_{n} be a basis for V, and let \phi_{1} , \cdots, \phi_{n} be the dual basis , \phi_{i} (v_{j}) = \delta_{ij}. Then the set of all k-fold tensor products \phi_{i_{1}} \otimes \cdots \otimes \phi_{i_{k}} 1 \le i_{1}, \cdots, i_{k} \le n is a basis for \mathcal{J}^{k} (V) , which therefore has dimension n^{k}.

(Def) If f : V \to W is a linear transformation, a linear transformation f^{*} : \mathcal{J}^{k} (W) \to \mathcal{J}^{k}(V) is defined by f^{*}T(v_{1}, \cdots, v_{k}) = T(f(v_{1}) , \cdots, f(v_{k})) for T \in \mathcal{J}^{k}(W) and v_{1}, \cdots, v_{k} \in V. It is easy to verify that f^{*} (S \otimes T) = f^{*}S \otimes f^{*}T.

(Def) Inner product on V to be a 2-tensor T such that T is symmetric, that is T(v,w) = T(w,v) for v,w \in V and such that T is positive definite, that is, T(v,v) >0 if v \neq 0. We distinguish \langle , \rangle as the usual inner product on \mathbf{R}^{n}.

(Thm 4.2) If T is an inner product on V, there is a basis v_{1}, \cdots, v_{n} for V s.t. T(v_{i}, v_{j}) = \delta_{ij} . (Such a basis is called orthonormal with respct to T.) Consequently there is an isomorphism f : \mathbf{R}^{n} \to V s.t. T(f(x), f(y)) = \langle x, y \rangle for x, y \in \mathbf{R}^{n}. In other words f^{*}T = \langle , \rangle.

(Def) A k-tensor \omega \in \mathcal{J}^{k}(V) is called alternating if \omega(v_{1}, \cdots, v_{i}, \cdots, v_{j}, \cdots, v_{k}) = - \omega(v_{1}, \cdots, v_{j}, \cdots, v_{i}, \cdots, v_{k}) for all v_{1}, \cdots, v_{k} \in V.

The set of all alternating k-tensors is clearly a subspace \Lambda^{k}(V) of \mathcal{J}^{k}(V).

(Def) the sign of a permutation \sigma, denoted \sgn \sigma, is +1 if \sigma is even and -1 if \sigma is odd. If T \in \mathcal{J}^{k}(V), we define Alt(T) by Alt(T)(v_{1}, \cdots, v_{k}) = \frac{1}{k!} \sum_{\sigma \in S_{k}} \sgn \sigma \cdot T(v_{\sigma (1)} , \cdots, v_{\sigma(k)} ), where S_{k} is the set of all permutations of the numbers 1 to k.

(Thm 4.3)

If T \in \mathcal{J}^{k}(V), then Alt (T) \in \Lambda^{k}(V).

If \omega \in \Lambda^{k} (V), then Alt(\omega) = \omega.

If T \in \mathcal{J}^{k} (V), then Alt(Alt(T)) = Alt(T).

(Def) The wedge product \omega \wedge \eta \in \Lambda^{k+l} (V) by \omega \wedge \eta = \frac{(k+l)!}{k!l!} Alt(\omega \otimes \eta).

(prop) (\omega_{1} + \omega_{2}) \wedge \eta = \omega_{1} \wedge \eta + \omega_{2} \wedge \eta,

\omega \wedge (\eta_{1} + \eta_{2} ) = \omega \wedge \eta_{1} + \omega \wedge \eta_{@},

a \omega \wedge \eta = \omega \wedge a \eta = a(\omega \wedge \eta),

\omega \wedge \eta = (-1)^{kl} \eta \wedge \omega,

f^{*}(\omega \wedge \eta) = f^{*} (\omega) \wedge f^{*} (\eta)

(Thm 4.4) 

If S \in \mathcal{J}^{k}(V) and T \in \mathcal{J}^{l}(V) and Alt(S) = 0, then Alt(S \otimes T) = Alt(T \otimes S ) = 0.

Alt(Alt(\omega \otimes \eta) \otimes \theta) = Alt(\omega \otimes \eta \otimes \theta) = Alt(\omega \otimes Alt(\eta \otimes \theta)).

If \omega \in \Lambda^{k}(V), \eta \in \Lambda^{l}(V), and \theta \in \Lambda^{m} (V), then (\omega \wedge \eta) \wedge \theta = \omega \wedge (\eta \wedge \theta) = \frac{(k + l + m)!}{k!l!m!} Alt(\omega \otimes \eta \otimes \theta) .

(Thm 4.5) If v_{1}, \cdots , v_{n} is a basis for V and \phi_{1}, \cdots, \phi_{n} is the dual basis, The set of all \phi_{i_{1}} \wedge \cdots \wedge \phi_{i_{k}} 1 \le i_{1}, < i_{2} < \cdots < i_{k} \le n is a basis for \Lambda^{k} (V), which therefore has dimension \binom{n}{k} = \frac{n!}{k!(n-k)!}.

If V has dimension n, \Lambda^{n} (V) has dimension 1. Thus all alternating n-tensors on V are multiples of any non-zero one.

(Thm 4.6) Let v_{1}, \cdots, v_{n} be a basis for V, and let \omega \in \Lambda^{n} (V). If w_{o} = \sum_{j = 1}^{n} a_{ij}v_{j} are n vectors in V, then \omega(w_{1}, \cdots, w_{n}) = det(a_{ij}) \cdot \omega(v_{1}, \cdots, v_{n}) .

(Def) a nonzero \omega \in \Lambda^{n}(V) splits the bases of V into two disjoint groups, those with \omega(v_{1}, \cdots, v_{n}) > 0 and those for which \omega(v_{1}, \cdots, v_{n}) < 0 ; this criterion is independent of \omega and can always be used to divide the bases of V into two disjoint groups. Either of these two groups is called an orientation for V.

The orientation to which a basis v_{1}, \cdots, v_{n} belongs is denoted [v_{1}, \cdots, v_{n}] and the other orientation is denoted –[v_{1}, \cdots, v_{n} ] . In \mathbf{R}^{n} we define the usual orientation as [e_{1}, \cdots, e_{n} ] .

(Def) For a general vector space V, if an inner product T for V is given. If an orientation \mu for V has also ben given, it follows that there is a unique \omega \in \Lambda^{n} (V) such that \omega(v_{1}, \cdots, v_{n}) = 1 whenever v_{1}, \cdots, v_{n} is an orthonormal basis such that [v_{1}, \cdots, v_{n}] = \mu. This unique \omega is called the volume element of V, determined by the inner product T and orientation \mu.

(Def) If v_{1}, \cdots, v_{n-1} \in \mathbf{R}^{n} and \phi is defined by \phi(w) = det \begin{pmatrix} v_{1} \\ \vdots \\ v_{n-1} \\ w \end{pmatrix}. then \phi \in \Lambda^{1}(\mathbf{R}^{n}) ; therefore there is a unique z \in \mathbf{R}^{n} s.t. \langle w , z \rangle = \phi (w) = det \begin{pmatrix} v_{1} \\ \vdots \\ v_{n-1} \\ w \end{pmatrix} . This z is denoted v_{1} \times \cdots \times v_{n-1} and called the cross product of v_{1}, \cdots, v_{n-1} .

(prop) v_{\sigma(1)} \times \cdots \times v_{\sigma(n-1)} = \sgn \sigma \cdot v_{1} \times \cdots \times v_{n-1},

v_{1} \times \cdots \times av_{i} \times \cdots \times v_{n-1} = a \times (v_{1} \times \cdots \times v_{n-1} ) ,

v_{1} \times \cdots \times (v_{i} + v_{i} ‘) \times \cdots \times v_{n-1} = v_{1} \times \cdots \times v_{i} \times \cdots \times v_{n-1} + v_{1} \times \cdots \times v_{i}’ \times \cdots \times v_{n-1} .

(subsection) Fields and Forms

(Def) If p \in \mathbf{R}^{n} , the sets of all pairs (p,v) , for v \in \mathbf{R}^{n} , is denoted \mathbf{R}^{n}_{p}, and called the tangent space of \mathbf{R}^{n} at p. This set is made into a vector space by (p,v) + (p,w) = (p , v+w) , a \cdot (p,v) = (p, av).

define p + v to be the end point of (p,v). write (p,v) as v_{p} .

(Def) Usual inner product \langle , \rangle_{p} for \mathbf{R}^{n}_{p} is defined by \langle v_{p} , w_{p} \rangle_{p} = \langle v , w \rangle, and the usual orientation for \mathbf{R}^{n}_{p}  is [(e_{1})_{p} , \cdots , (e_{n})_{p}] .

(Def) A vector field is a function F s.t. F(p) \in \mathbf{R}^{n}_{p} for each p \in \mathbf{R}^{n} . For each p there are numbers F^{1}(p) , \cdots, F^{n} (p) s.t. F(p) = F^{1}(p) \cdot (e_{1})_{p} + \cdots + F^{n}(p) \cdot (e_{n})_{p} . We obtain n component functions F^{i} : \mathbf{R}^{n} \to \mathbf{R}.

Vector field F is called continuous, differentiable, etc., if the functions F^{i} are. 

Operations on vectors yield operations on vector fields when applied at each point separately.

(Def) divergence, div F of F, as \sum_{i = 1}^{n} D_{i}F^{i}. \nabla = \sum_{i = 1}^{n} D_{i} \cdot e_{i} , div(F) = \langle \nabla , F \rangle . 

(Def) If n = 3 we write (\nabla \times F) (p) = (D_{2} F^{3} – D_{3} F^{2} )(e_{1})_{p} + (D_{3} F^{1} – D_{1}F^{3})(e_{2})_{p} + (D_{1} F^{2} – D_{2}F^{1})(e_{3})_{p} . The vector field \nabla \times F is called curl F.

(Def) a function \omega with \omega(p) \in \Lambda^{k}(\mathbf{R}^{n}_{p}) . such a function is called a k-form on \mathbf{R}^{n}, or a differential form. If \phi_{1}(p) , \cdots, \phi_{n}(p) is the dual basis to (e_{1})_{p} , \cdots, (e_{n})_{p}, then \omega(p) = \sum_{i_{1} < \cdots < i_{k}} \omega_{i_{1}, \cdots, i_{k}} (p) \cdot [\phi_{i_{1}} (p) \wedge \cdots \wedge \phi_{i_{k}}(p)] for certain functions \omega_{i_{1}, \cdots, i_{k}} .

The form \omega is called continuous, differentiable, etc., if these functions are.

The sum \omega + \eta, product f \cdot \omega, and wedge product \omega \wedge \eta are defined in the obvious way.

(Def) If f : \mathbf{R}^{n} \to \mathbf{R} is differentiable, then Df(p) \in \Lambda^{1} (\mathbf{R}^{n} . we obtain a 1-form df, defined by df(p)(v_{p}) = Df(p)(v).

(Def) Let x^{i} denote the function \pi_{i}. Since dx^{i}(p)(v_{p}) = d\pi^{i} (p)(v_{p}) = D\pi^{i} (p)(V) = v^{i} , dx^{1}(p), \cdots, dx^{n}(p) is just the dual basis to (e_{1})_{p} , \cdots, (e_{n})_{p} . Thus every k-form \omega can be written \omega = \sum_{i_{1} < \cdots < i_{k}} \omega_{i_{1}, \cdots, i_{k}} dx^{i_{1}} \wedge \cdots dx^{i_{k}} 

(Thm 4.7) If f : \mathbf{R}^{n} \to \mathbf{R} is differentiable, then df = D_{1}f \cdot dx^{1} + \cdots + D_{n}f \cdot dx^{n}. In classical notation, df = \frac{\partial f}{\partial x^{1}} dx^{1} + \cdots + \frac{\partial f }{\partial x^{n}} dx^{n}.

(Def) Consider now a differentiable function f : \mathbf{R}^{n} \to \mathbf{R} we have a linear transformation Df(p) : \mathbf{R}^{n} \to \mathbf{R}^{m} . we produce linear transformation f_{*} : \mathbf{R}^{n}_{p} \to \mathbf{R}^{m}_{f(p)} defined by f_{*}(v_{p}) = (Df(p)(v))_{f(p)}. This induces a linear transformation f^{*} : \Lambda^{k}(\mathbf{R}^[m]_{f(p)}) \to \Lambda^{k}(\mathbf{R}^{n}_{p}) . If \omega is a k-form on \mathbf{R}^{m} we can therefore define a k-form f^{*} \omega on \mathbf{R}^{n} by (f^{*} \omega) (p) = f^{*}(\omega(f(p))).

This means that if v_{1}, \cdots, v_{k} \in \mathbf{R}^{n}_{p}, then we have f^{*} \omega(p) (v_{1}, \cdots, v_{k}) = \omega(f(p))(f_{*}(v_{1}, \cdots, f_{*}(v_{k})). 

(Thm 4.8) If f: \mathbf{R}^{n} \to \mathbf{R}^{m} is differentiable, then

f^{*}(dx^{i}) = \sum_{j = 1}^{n} D_{j}f^{i}\cdot dx^{j} = \sum_{j = 1}^{n} \frac{\partial f^{i}}{\partial x^{j}} dx^{j}.

f^{*} (\omega_{1} + \omega_{2}) = f^{*}(\omega_{1}) + f^{*} (\omega_{2}) .

f^{*} (g \cdot \omega) = (g \bullet f) \cdot f^{*} \omega.

f^{*} (\omega \wedge \eta) = f^{*} \omega \wedge f^{*} \eta.

(Thm 4.9) If f : \mathbf{R}^{n} \to \mathbf{R}^{n} is differentiable, then f^{*} (h dx^{1} \wedge \cdots \wedge dx^{n}) = (h \bullet f)(det f’) dx^{1} \wedge \cdots \wedge dx^{n}.

(Def) If  \omega = \sum_{i_{1} < \cdots < i_{k}} \omega_{i_{1}, \cdots, i_{k}} dx^{i_{1}} \wedge \cdots dx^{i_{k}} , we define a (k+1)-form d\omega, the differential of \omega, by d\omega = \sum_{i_{1} < \cdots < i_{k}} d \omega_{i_{1}, \cdots, i_{k}} \wedge dx^{i_{1}} \wedge \cdots dx^{i_{k}} = \sum_{i_{1} < \cdots < i_{k}} \sum_{\alpha = 1}^{n} D_{\alpha}(\omega_{i_{1}, \cdots, i_{k}} ) \cdot dx^{\alpha} \wedge dx^{i_{1}} \wedge \cdots dx^{i_{k}}

(Thm 4.10) 

d(\omega + \eta) = d\omega + d\eta.

If \omega is a k-form and \eta is an l-form, then d(\omega \wedge \eta) = d\omega \wedge \eta + (-1)^{k} \omega \wedge d\eta.

d(d\omega)) = 0. Briefly, d^{2} = 0.

If \omega is a k-form on \mathbf{R}^{m} and f : \mathbf{R}^{n} \to \mathbf{R}^{m} is differentiable, then f^{*} (d\omega) = d(f^{*} \omega).

(Def) a form \omega is called closed if d \omega = 0 and exact if \omega = d \eta, for some \eta.

(Def) An open set A \subset \mathbf{R}^{n} with the properyty that whenever x \in A, the line segment from 0 to x is contained in A; such an open set is called star-shaped with respect to 0.

(Poincare Lemma) (Thm 4.11) If A \subset \mathbf{R}^{n} is an open set star-shaped with respect to 0, then every closed form on A is exact.

(subsection) Geometric preliminaries

(Def) A singular n-cube in A \subset \mathbf{R}^{n} is a continuus function c : [0,1]^{n} \to A (here [0,1]^{n} denotes the n-fold product [0,1] \times \cdots \times [0,1]). \mathbf{R}^{0} and [0,1]^{0} both denote {0}.

A singular 1-cube is often called a curve.

The standard n-cube I^{n} : [0,1]^{n} \to \mathbf{R}^{n} defined by I^{n} (x) = x for x \in [0,1]^{n}.

(Def) a finite sum of singular n-cubes with integer coefficients is called an n-chain in A. For each singular n-chain c in A we shall define an (n-1)-chain in A called the boundary of c and denoted \partial c.

(Def) For each i with 1 \le i \le n we define two singular (n-1)-cubes I^{n}_{(i,0)} and I^{n}_{(i,1)} as follows. If x \in [0,1]^{n-1}, then

I^{n}_{(i,0)} (x) = I^{n}(x^{1} , \cdots, x^{i-1}, 0, x^{i}, \cdots, x^{n-1}) = (x^{1} , \cdots, x^{i-1}, 0, x^{i}, \cdots, x^{n-1}),

I^{n}_{(i,1)} (x) = I^{n}(x^{1} , \cdots, x^{i-1}, 1, x^{i}, \cdots, x^{n-1}) = (x^{1} , \cdots, x^{i-1}, 1, x^{i}, \cdots, x^{n-1}).

We call I^{n}_{(i,0)} the (i,0)-face of I^{n} and I^{n}_{(i,1)} the (i,1)-face.

we then define \partial I^{n} = \sum_{i = 1}^{n} \sum_{\alpha = 0,1} (-1)^{i+\alpha} I^{n}_{(i + \alpha)} .

(Def) For a general singular n-cube c: [0,1]^{n} \to A we define the (i,\alpha) -face, c_{(i,\alpha)} = c \bullet (I^{n}_{(i,\alpha)}) and then define \partial c = \sum_{i = 1}^{n} \sum_{\alpha = 0,1} (-1)^{i+\alpha} c_{(i,\alpha)}. 

We define the boundary of an n-chain \sum a_{i}c_{i} by \partial (\sum a_{i} c_{i}) = \sum a_{i} \partial(c_{i}) .

(Thm 4.12) If c is an n-chain in A, then \partial(\partial c) = 0. Briefly, \partial^{2} = 0.

(subsection) The fundamental theorem of calculus

(Def) If \omega is a k-form on [0,1]^{k}, then \omega = f dx^{1} \wedge \cdots \wedge dx^{k} for a unique function f. we define \int_{[0,1]^{k}} \omega = \int_{[0,1]^{k}} f. we could also write this as \int_{[0,1]^{k}} f dx^{1} \wedge \cdots \wedge dx^{k} = \int_{[0,1]^{k}} f(x^{1}, \cdots, x^{k}) dx^{1} \cdots dx^{k} . If \omega is a k-form on A and c is a singular k-cube in A, we define \int_{c} \omega = \int_{[0,1]^{k}} c^{*} \omega.

(Def) If c : {0} \to A is a singular 0-cube in A we define \int_{c} \omega = \omega(c(0)) . The integral of \omega over a k-chain c = \sum a_{i} c_{i} is defined by \int_{c} \omega = \sum a_{i} \int_{c{i}} \omega. The integral of a 1-form over a 1-chain is often called a line integral.

(prop) If P dx + Q dy is a 1-form on \mathbf{R}^{2} and c:[0,1] \to \mathbf{R}^{2} is a singular 1-cube, 

\int_{c} P dx + Q dy = \lim \sum_{i = 1}^{n} [c^{1} (t_{i}) – c^{1}(t_{i-1})] \cdot P(c(t^{i})) + [c^{2} (t_{i}) – c^{2}(t_{i-1})] \cdot Q(c(t^{i})) 

where t_{0}, \cdots, t_{n} is a partition of [0,1], the choice of t^{i} in [t_{i-1}, t_{i}] is arbitrary, and the limit is taken over all partitions as the maximum of |t_{i} – t_{i-1}| goes to 0.

(Def) Analogous definitions for surface integrals, integrals of 2-forms over singular 2-cubes.

(Stoke’s Theorem) (Thm 4.13) if \omega is a (k-1)-form on an open set A \subset \mathbf{R}^{n} and c is a k-chain in A, then \int_{c} d\omega = \int_{\partial c} \omega.

