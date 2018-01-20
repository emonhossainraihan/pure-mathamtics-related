---



layout: post



title : \[Calculus on Manifolds] Functions on Euclidean Space



date : 2018-01-20 11:52:04 +0900



---

(Section 1) Functions on Euclidean Space

(subsection) Norm and Inner Product

(Def) Euclidean n-space \mathbf{R}^{n} is defined as the set of all n-tuples (x^{1}, \cdots, x^{n}) of real numbers x^{i} . An element of \mathbf{R}^{n} is often called a point in \mathbf{R}^{n} , and \mathbf{R}^{1}, \mathbf{R}^{2}, \mathbf{R}^{3} are often called the line, the plane, and space, respectively. If x denotes an element of \mathbf{R}^{n}, then x is an n-tuple of numbers, the ith one of which is denoted x^{i} ;. thus we can write x = (x^{1}, \cdots, x^{n}).

(Def) a point in \mathbf{R}^{n} is also called a vector in \mathbf{R}^{n}, because \mathbf{R}^{n}, with x + y = (x^{1} + y^{1}, \cdots, x^{n} + y^{n}) and ax = (ax^{1}, \cdots, ax^{n}) , as operations, is a vector space. 

(Def) The length of a vector x, the norm |x| of x and defined by \x| = \sqrt{(x^{1})^{2} + \cdots + (x^{n})^{2}} . 

(Thm 1.1) If x , y \in \mathbf{R}^{n} and a \in \mathbf{R} , then 

|x| \ge 0, and |x| = 0 iff x = 0

| \sum_{i = 1}^{n} x^{i} y^{i} | \le |x| \cdot |y| ; equality holds iff x and y are linearly depencent.

|x + y| \le |x| + |y| .

|ax| = |a| \cdot |x|.

(Def) The quantity \sum_{i = 1}^{n} x^{i} y^{i} is called the inner product of x and y and denoted \langle x,y \rangle.

(Thm 1.2) If x, x_{1}, x_{2} and y, y_{1}, y_{2} are vectors in \mathbf{R}^{n} and a \in \mathbf{R}, then

\langle x , y \rangle = \langle y, x \rangle (symmetry)

\langle ax , y \rangle = \langle x , ay \rangle = a \langle x , y \rangle \langle x_{1} + x_{2} , y \rangle = \langle x_{1} , y \rangle + \langle x_{2} , y \rangle , \langle x , y_{1} + y_{2} \rangle = \langle x , y_{1} \rangle + \langle x , y_{2} \rangle (bilinearity)

\langle x , x \rangle \ge 0 and \langle x , x \rangle = 0 iff x = 0 ( positive definiteness)

|x| - \sqrt{ \langle x , x \rangle }

\langle x , y \rangle = \frac{|x + y|^{2} - |x – y|^{2}}{4} (polarization identity)

(Def) The vector (0, \cdots, 0) will be denoted simply 0. The usual basis of \mathbf{R}^{n} is e_{1} , \cdots, e_{n} where e_{i} = (0, \cdots, 1, \cdots, 0) with the 1 in the ith place.

(Def) If T : \mathbf{R}^{n} \to \mathbf{R}^{m} is a linear transformation, the matrix of T with respect to the usual bases of \mathbf{R}^{n} and \mathbf{R}^{m} is the m \times n matrix A = (a_{ij}) , where T(e_{i}) = \sum_{j = 1}^{m} a_{ji}e_{j} – the coefficients of T(e_{i}) appear in the ith column of the matrix.

If S : \mathbf{R}^{m} \to \mathbf{R}^{p} has the p \times m matrix B, then S \bullet T has the p \times n matrix BA.

(Def) if x \in \mathbf{R}^{n} and y \in \mathbf{R}^{m}, then (x,y) denotes (x^{1} , \cdots, x^{n} , y^{1}, \cdots, y^{m}) \in \mathbf{R}^{n+m}

(subsection) Subsets of Euclidean Space

(Def) If A \subset \mathbf{R}^{m} and B \subset \mathbf{R}^{n}, then A \times B \subset \mathbf{R}^{m+n} is defined as the set of all (x,y) \in \mathbb{R}^{m+n} with x \in A and y \in B.

If A \subset \mathbf{R}^{m}, B \subset \mathbf{R}^{n} and C \subset \mathbf{R}^{p}, then (A \times B) \times C = A \times (B \times C) , and denoted simply A \times B \times C.

(Def) The set [a_{1}, b_{1}] \times \cdots \times [a_{n} , b_{n}] \subset \mathbf{R}^{n} is called a closed rectangle in \mathbf{R}^{n}, while the set (a_{1}, b_{1}) \times \cdots \times (a_{n} , b_{n}) \subset \mathbf{R}^{n} is called an open rectangle. 

a set U \subset \mathbf{R}^{n} is called open if for each x \in U there is an open rectangle A s.t. x \in A \subset U. a subset C of \mathbf{R}^{n} is closed if \mathbf{R}^{n} – C is open.

(prop) If A \subset \mathbf{R}^{n} and x \in \mathbf{R}^{n}, then one of three possibilities must hold.

There is an open rectangle B s.t. x \in B \subset A. (Interior of A)

There is an open rectangle B s.t. x \in B \subset \mathbf{R}^{n} – A. (Exterior of A)

If B is any open rectangle with x \in B, then B contains points of both A and \mathbf{R}^{n} – A. (Boundary of A)

(Def) A collection \mathcal{O} of open sets is an open cover of A, or briefly , covers A , if every points x \inA is in some open set in the collection \mathcal{O}.

(Def) A set A is called compact if every open cover \mathcal{O} contains a finite subcollection of open sets which also covers A.

(Heine-Borel)(Thm 1.3)  The closed interval [a,b] is compact.

(Thm 1.4) If B is compact and \mathcal{O} is an open cover of {x} \times B, then there is an open set U \subset \mathbf{R}^{n} containing x s.t. U \times B is covered by a finite number of sets in \mathcal{O}.

(Cor 1.5) If A \subset \mathbf{R}^{n} and B \subset \mathbf{R}^{m} are compact, then A \times B \subset \mathbf{R}^{n+m} is compact.

(Cor 1.6) A_{1} \times \cdots \times A_{k} is compact if each A_{i} is. In particular, a closed rectangle in \mathbf{R}^{k} is compact.

(Cor 1.7) A closed bounded subset of \mathbf{R}^{n} is compact. The converse is also true.

(subsection) Functions and Continuity

(Def) A function from \mathbf{R}^{n} to \mathbf{R}^{m} (a vector-valued function of n variables) is a rule which associates to each point in \mathbf{R}^{n} some point in \mathbf{R}^{m}; the point a function f associates to x is denoted f(x).

Notation f : A \to \mathbf{R}^{m} indicates that f(x) is defined only for x in the set A, which is called the domain of f. 

If B \subset A, we define f(B) as the set of all f(x) for x \in B, and if C \subset \mathbf{R}^{m} we define f^{-1}(C) = {x \in A : f(x) \in C} .

(Def) If f : A \to \mathbf{R}^{m} and g : B \to \mathbf{R}^{p}, where B \subset \mathbf{R}^{m}, then the composition g \bullet f is defined by g \bullet f (x) = g(f(x)) ; the domain of g \bullet f is A \cap f^{-1}(B). If f : A \to \mathbf{R}^{m} is 1-1, we define f^{-1} : f(A) \to \mathbf{R}^{n} by the requirement that the f^{-1} (z) is the unique x \in A with f(x) = z.

(Def) A function f : A \to \mathbf{R}^{m} determines m component functions f^{1}, \cdots, f^{m} : A \to \mathbf{R} by f(x) = (f^{1}(x), \cdots, f^{m}(x)) . 

(Def) If \pi : \mathbf{R}^{n} \to \mathbf{R}^{n} is the identity function, \pi(x) = x, then \pi^{i} (x) = x^{i} ; the function \pi^{i} is called the ith projection function.

(Def \lim_{x \to a} f(x) = b means, for every number \epsilon >0 there is a number \delta>0 s.t. |f(x) – b| < \epsilon for all x in the domain of f which satisfy 0< |x-a| < \delta.

(Def) A function f : A \to \mathbf{R}^{m} is called continuous at a \in A if \lim_{x \to a} f(x) = f(a), and f is simply called continuous if it is continuous at each a \in A.

(Thm 1.8) If A \subset \mathbf{R}^{n}, a function f : A \to \mathbf{R}^{m} is continuous iff for every open set U \subset \mathbf{R}^{m} there is some open set V \subset \mathbf{R}^{n} s.t. f^{-1}(U) = V \cap A.

(Thm 1.9) If f : A \to \mathbf{R}^{m} is continuous, where A \subset \mathbf{R}^{n}, and A is compact, then f(A) \subset \mathbf{R}^{m} is compact.

(Def) If f : A \to \mathbf{R} is bounded, the extent to which f fails to be continuous at a \n A can be measured in a precise way. For \delta >0 let 

M(a, f, \delta) = \sup{f(x) : x \in A and |x-a| < \delta},

m(a, f, \delta) = \inf{f(x) : x \in A and |x-a| < \delta}.

The oscillation o(f,a) of f at a is defined by o(f,a) = \lim_{\delta \to 0} [M(a,f,\delta) – m(a,f,\delta)]. 

(Thm 1.10) The bounded function f is continuous at a iff o(f,a) = 0.

(Thm 11.1) Let A \subset \mathbf{R}^{n} be closed. If f : A \to \mathbf{R} is any bounded function, and \epsilon >0, then {x \in A : o(f,x) \ge \epsilon } is closed.

