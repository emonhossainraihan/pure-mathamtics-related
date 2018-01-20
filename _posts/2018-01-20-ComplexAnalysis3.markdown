---



layout: post



title : [Complex Analysis] Meromorphic Functions and the Logarithm



date : 2018-01-20 09:52:04 +0900



---

(Section 3) Meromorphic Functions and the Logarithm

(subsection 1) Zeros and poles

(Def) A point singularity of a function f is a complex number z_{0} s.t. f is defined in a neighborhood of z_{0} but not at the point z_{0} itself. We also call such points isolated singularities.

A complex number z_{0} is a zero for the holomorphic function f if f(z_{0}) = 0. In particular, analytic continuation shows that the zeros of a non-trivial holomorphic functions are isolated.

(prop) If f is holomorphic in \Omega and f(z_{0}) = 0 for some z_{0} \in \Omega, then there exists an open neighborhood U of z_{0} s.t. f(z) \neq 0 for all z \in U – {z_{0}} , unless f is identically zero.

(Thm 1.1.) Suppose that f is holomorphic in a connected open set \Omega, has a zero at a point z_{0} \in Omega, and does not vanish identically in \Omega. Then there exists a neighborhood U \subset \Omega of z_{0} , a non-vanishing holomorphic function g on U, and a unique positive integer n s.t. f(z) = (z-z_{0})^{n}g(z) for all z \in U.

(Def) in the case of above theorem, we say that f has a zero of order n (or multiplicity n) at z_{0}. If a zero is of order 1, we say that it is simple.

(Def) a deleted neighborhood of z_{0} to be an open disc centered at z_{0}, minus the point z_{0}, that is, the set {z: 0 < |z-z_{0}| < r} for some r>0. Then, we say that a function f defined in a deleted neighborhood of z_{0} has a pole at z_{0}, if the function 1/f, defined to be zero at z_{0}, is holomorphic in a full neighborhood of z_{0}.

(Thm 1.2.) If f has a pole at z_{0} \in \Omega, then in a neighborhood of that point there exists a non-vanishing holomorphic function h and a unique positive integer n s.t. f(z) = (z-z_{0})^{-n} h(z).

(Def) the integer n is called the order(or multiplicity) of the pole, and describes the rate at which the function grows near z_{0}. If the pole is of order 1, we say that it is simple.

(Thm 1.3.) If f has a pole of order n at z_{0}, then f(z) = \frac{a_{-n}}{(z-z_{0})^{n}} + \frac{a_{-n+1}}{(z-z_{0})^{n-1}} + \cdots + \frac{a_{-1}}{(z-z_{0})} + G(z), where G is a holomorphic function in a neighborhood of z_{0}.

(Def) The sum \frac{a_{-n}}{(z-z_{0})^{n}} + \frac{a_{-n+1}}{(z-z_{0})^{n-1}} + \cdots + \frac{a_{-1}}{(z-z_{0})} is called the principal part of f at the pole z_{0} , and the coefficient a_{-1} is the residue of f at that pole. We write res_{z_{0}} f = a_{-1}. 

(Thm 1.4.) If f has a pole of order n at z_{0}, then res_{z_{0}} f = \lim_{z \to z_{0}} \frac{1}{(n-1)!} (\frac{d}{dz})^{n-1} (z-z_{0})^{n} f(z).

(subsection 2) The residue formula

(Thm 2.1.) Suppose that f is holomorphic in an open set containing a circle C and its interior, except for a pole at z_{0} inside C. Then \int_{C} f(z)dz = 2\pi i res_{z_{0}} f.

(Cor 2.2.) Suppose that f is holomorphic in an open set containing a circle C and its interior, except for poles at the points z_{1}, …, z_{N} inside C. Then \int_{C} f(z) dz = 2\pi i \sum_{k = 1}^{N} res_{z_{k}} f.

(Cor 2.3.) Suppose that f is holomorphic in an open set containing a toy contour \gamma and its interior, except for poles at the points z_{1},, …, z_{N} inside \gamma. Then \int_{\gamma} f(z) dz = 2\pi i \sum_{k = 1}^{N} res_{z_{k}} f.

(Def) The identity \int_{\gamma} f(z) dz = 2\pi i \sum_{k = 1}^{N} res_{z_{k}} f is referred to as the residue formula.

(subsection 3) Singularities and meromorphic functions

(Def) Let f be a function holomorphic in an open set \Omega except possibly at one point z_{0} in \Omega. If we can define f at z_{0} in such a way that f becomes holomorphic in all of \Omega, we say that z_{0} is a removable singularity for f.

(Riemann’s theorem on removable singularities) (Thm 3.1.) Suppose that f is holomorphic in an open set \Omega except possibly at a point z_{0} in \Omega. If f is bounded on \Omega – {z_{0}} , then z_{0} is a removable singularity.

(Cor 3.2.) Suppose that f has an isolated singularity at the point z_{0}. Then z_{0} is a pole of f iff |f(z)| \to \infty as z \to z_{0}.

(Def) Isolated singularities belong to one of three categories : Removable singularities (f bounded near z_{0}), Pole singularities (|f(z)| \to \infty as z \to z_{0}) , Essential singularities. Any singularity that is not removable or a pole is defined to be an essential singularity.

(Casorati-Weierstrass) (Thm 3.3.) Suppose f is holomorphic in the punctured disc D_{r}(z_{0}) – {z_{0}} and has an essential singularity at z_{0}. Then, the image of D_{r}(z_{0}) – {z_{0}} under f is dense in the complex plane.

(Def) A function f on an open set \Omega is meromorphic if there exists a sequence of points {z_{0}, z_{1},z_{2},…} that has no limit poits in \Omega, and such that 

the function f is holomorphic in \Omega – {z_{0}, z_{1}, z_{2}, …}, and 

f has poles at the points {z_{0}, z_{1}, z_{2},…} .

If f is holomorphic for all large values of z, we consider F(z) = f(1/z), which is now holomorphic in a deleted neighborhood of the origin. We say that f has a pole at infinity if F has a pole at the origin. Similarly, we can speak of f having an essential singularity at infinity, or a removable singularity (hence holomorphic) at infinity in terms of the corresponding behavior of F at 0. A meromorphic function in the complex plane that is either holomorphic at infty or has a pole at infinity is said to be meromorphic in the extended complex plane.

(Thm 3.4.) The meromorphic functions in the extended complex plane are the rational functions.

(Def) Consider the Euclidean space \mathbb{R}^{3} with coordinates (X,Y,Z) where the XY-plane is identified with \mathbb{C} . We denote by \mathbb{S} the sphere centered at (0,0,1/2) and of radius 1/2; Also, we let \mathcal{N} = (0,0,1) denote the north pole of the sphere. 

(Def) Given any point W = (X,Y,Z) on \mathbb{S} different from the north pole, the line joining \mathcal{N} and W intersects the XY-plane in a single point which we denote by w = x + iy; w is called the stereographic projection of W. This geometric construction gives a bijective correspondence between points on the punctured sphere \mathbb{S} – {\mathcal{N}} and the complex plane; It is described analytically by the formulas x = \frac{X}{1-Z} and y = \frac{Y}{1-Z} giving w in terms of W, and X = \frac{x}{x^{2} + y^{2} + 1}, Y = \frac{y}{x^{2} + y^{2} + 1} , and Z = \frac{x^2 + y^{2} }{x^{2} + y^{2} + 1} giving W in terms of w.

(Def) Identifying infinity with the point \mathcal{N} on \mathbb{S}, we see that the extended complex plane can be visualized as the full two-dimensional sphere \mathbb{S}; this is the Riemann sphere. Since this construction takes the unbounded set \mathbb{C} into the compact set \mathbb{S} by adding one point, the Riemann sphere is sometimes called the one-point compactification of \mathbb{C}.

(subsection 4) The argument principle and applications

(Argument principle) (Thm 4.1.) Suppose f is meromorphic in an open set containing a circle C and its interior. If f has no poles and never vanishes on C, then \frac{1}{2\pi i} \int_{C} \frac{f’(z)}{f(z)}dz = (number of zeros of f inside C) minus (number of poles of f inside C), where the zeros and poles are counted with their multiplicities.

(Cor 4.2.) The above theorem holds for toy contours.

(Rouche’s theorem) (Thm 4.3.) Suppose that f and g are holomorphic in an open set containing a circle C and its interior. If |f(z)| > |g(z)| for all z \in C, then f and f+g have the same number of zeros inside the circle C.

(Def) A mapping is said to be open if it maps open sets to open sets.

(Open mapping theorem) (Thm 4.4.) If f is holomorphic and non-constant in a region \Omega, then f is open.

(Def) Refer to the maximum of a holomorphic function f in an open set \Omega as the maximum of its absolute value |f| in \Omega.

(Maximum modulus principle) (Thm 4.5.) If f is a non-constant holomorphic function in a region \Omega, then f cannot attain a maximum in \Omega.

(Cor 4.6.) Suppose that \Omega is a region with compact closure \bar{Omega}. If f is holomorphic on \Omega and continuous on \bar{\Omega} then \sup_{z \in \Omega} |f(z)| \le \sup_{z \in \bar{\Omega} - \Omega} |f(z)|. 

(subsection 5) Homotopies and simply connected domains

(Def) Let \gamma_{0} and \gamma_{1} be two curves in an open set \Omega with common end-points. So if \gamma_{0}(t) and \gamma_{1}(t) are two parametrizations defined on [a,b], we have \gamma_{0}(a) = \gamma_{1}(a) = \alpha and \gamma_{0}(b) = \gamma_{1}(b) = \beta. These two curves are said to be homotopic in \Omega if for each 0 \le s \le 1 there exists a curve \gamma_{s} \subset \Omega, parametrized by \gamma_{s}(t) defined on [a,b] , s.t. for every s \gamma_{s}(a) = \alpha and \gamma_{s}(b) = \beta, and for all t \in [a,b] \gamma_{s}(t)|_{s = 0} = \gamma_{0}(t) and \gamma_{s}(t)|_{s=1} = \gamma_{1}(t). Moreover, \gamma_{s}(t) should be jointly continuous in s \in [0,1] and t \in [a,b].

(Thm 5.1.) If f is holomorphic in \Omega, then \int_{\gamma_{0}} f(z) dz = \int_{\gamma_{1}} f(z) dz whenever the two curves \gamma_{0} and \gamma_{1} are homotopic in \Omega.

(Def) A region \Omega in the complex plane is simply connected if any two pair of curves in \Omega with the same end-points are homotopic.

(Thm 5.2.) Any holomorphic function in a simply connected domain has a primitive.

(Cor 5.3.) If f is holomorphic in the simply connected region \Omega, then \int_{\gamma} f(z)dz = 0 for any closed curve \gamma in \Omega.

(subsection 6) The complex logarithm

(Def) To make sense of the logarithm as a single-valued function, we must restrict the set on which we define it. This is the so-called choice of a branch or sheet of the logarithm.

(Thm 6.1.) Suppose that \Omega is simply connected with 1 \in \Omega, and 0 \notin \Omega. Then in \Omega there is a branch of the logarithm F(z) = log_{\Omega}(z) so that 

F is holomorphic in \Omega,

e^{F(z)} = z for all z \in \Omega,

F(r) = log r whenever r is a real number and near 1.

In other words, each branch \log_{\Omega}(z) is an extension of the standard logarithm defined for positive numbers.

(Def) In the slit plane \Omega = \mathbb{C} – {(-\infty, 0]} we have the principle branch of the logarithm log z = log r + i \theta where z = re^{i\theta} with |\theta| < \pi.

(Thm 6.2.) If f is a nowhere vanishing holomorphic function in a simply connected region \Omega, then there exists a holomorphic function g on \Omega s.t. g(z) = e^{g(z)} . 

The function g(z) in the theorem can be denoted by log f(z), and determines a branch of that logarithm.

(subsection 7) Fourier series and harmonic functions

(Thm 7.1.) The coefficients of the power series expansion of f are given by a_{n} = \frac{1}{2\pi r^{n}} \int_{0}^{2\pi} f(z_{0} + re^{i\theta}) e^{-in\theta} d\theta for all n \ge 0 and 0 < r < R. Moreover, 0 = \frac{1}{2\pi r^{n}} \int_{0}^{2 \pi} f(z_{0} + re^{i\theta}) e^{-in\theta} d \theta whenever n < 0.

(Mean-value property) (Cor 7.2.) If f is holomorphic in a disc D_{R}(z_{0}), then f(z_{0}) = \frac{1}{2\pi} \int_{0}^{2\pi} f(z_{0} + re^{i\theta}) d\theta , for any 0 < r < R. 

(Cor 7.3.) If f is holomorphic in a disc D_{R}(z_{0}) , and u = Re(f), then u(z_{0}) = \frac{1}{2\pi} \int_{0}^{2\pi} u(z_{0} + re^{i\theta}) d\theta, for any 0 < r < R. 

