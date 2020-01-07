---



layout: post



title : (Calculus on Manifolds) Integration



date : 2018-01-20 11:54:04 +0900



---

(section 3) Integration

(subsection) Basic definitions

(Def) a partition of a rectangle [a_{1}, b_{1}] \times \cdots \times [a_{n}, b_{n}] is a collection P = (P_{1}, \cdots, P_{n}) , where each P_{i} is a partition of the interval [a_{i},b_{i}].

P = (P_{1}, \cdots, P_{n}) divides [a_{1},b_{1}] \times \cdots \times [a_{n}, b_{n}] into N = N_{1}, \cdots, N_{n} subrectangles. These subrectangles will be called subrectangles of the partition P.

(Def) Supose that A is a rectangle, f : A \to \mathbf{R} is a bounded function, and P is a partition of A. For each subrectangle S of the partition let m_{S}(f) = \inf {f(x) : x \in S} , M_{s}(f) = \sup{f(x) : x \in X}, and let v(S) be the volume of S. [The volume of a rectangle [a_{1}, b_{1}] \times \cdots \times [a_{n}, b_{n}] , and also of (a_{1}, b_{1}) \times \cdots \times (a_{n}, b_{n}) , is defined as (b_{1} – a_{1}) \cdot … \cdot (b_{n} – a_{m}) ] . the lower and upper sums of f for P are defined by

L(f,P) = \sum_{S} m_{S}(f) \cdot v(S) and U(f,P) = \sum_{S} M_{S}(f) \cdot v(S).

(Lem 3.1) Suppose the partition P’ refines P (that is, each subrectangle of P’ is contained in a subrectangle of P). Then L(f,P) \le L(f,P’) and U(f,P’) \le U(f,P) .

(Cor 3.2) If P and P’ are any two partitions, then L(f,P’) \le U(f,P).

The lease upper bound of all lower sums for f is less than or equal to the greatest lower bound of all upper sums for f.

(Def) A function f : A \to \mathbf{R} is called integrable on the rectangle A if f is bounded and \sup{L(f,P)} = \inf{U(f,P)} . This common number is then denoted \int_{A} f, and called the integral of f over A. Often, the notation \int_{A} f(x^{1}, \cdots, x^{n} ) dx^{1} \cdots dx^{n} is used.

(Thm 3-3) A bounded function f : A \to \mathbf{R} is integrable iff for every \epsilon >0 there is a partition P of A s.t. U(f,P) – L(f,P) < \epsilon.

(Prop)

Let f: A \to \mathbf{R} be a constant function, f(x) = c. \int_{A} f = c \cdot v(A).

Let f:[0,1] \times [0,1] \to \mathbf{R} be defined by f(x,y) = \begin{cases} 0 & if x is rational, \\ 1 & if x is irrational.\end{cases} . f is not integrable.

(subsection) Measure Zero and Content Zero

(Def) A subset A of \mathbf{R}^{n} has (n-dimensional) measure 0 if for every \epsilon >0 there is a cover {U_{1}, U_{2}, U_{3}, \cdots } of A by closed rectangles s.t. \sum_{i = 1}^{\infty} v(U_{i}) < \epsilon.

A set with only finitely many points has measure 0.

(Thm 3.4) If A = A_{1} \cup A_{2} \cup A_{3} \cdots and each A_{i} has measure 0, then A has measure 0.

(Def) A subset A of \mathbf{R}^{n} has (n-dimensional) content 0 if for every \epsilon>0 there is a finite cover {U_{1}, \cdots, U_{n} } of A by closed rectangles such that \sum_{i = 1}^{n} v(U_{i}) < \epsilon.

(Thm 3.5) If a < b, then [a,b] \subset \mathbf{R} does not have content 0. In fact, if {U_{1}, \cdots, U_{n} } is a finite cover of [a,b] by closed intervals, then \sum_{i = 1}^{n} v(U_{i}) \ge b-a.

(Thm 3.6) If A is compact and has measure 0, then A has content 0.

(subsection) Integrable functions

(Lem 3.7) Let A be a closed rectangle and let f : A \to \mathbf{R} be a bounded function s.t. o(f,x) < \epsilon for all x \in A. Then there is a partition P of A with U(f,P) – L(f,P) < \epsilon \cdot v(A).

(Thm 3.8) Let A be a closed rectangle and f : A \to \mathbf{R} a bounded function. Let B = {x : f is not continuous at x}, then f is integrable iff B is a set of measure 0.

(Def) If C \subset \mathbf{R}^{n}, the characteristic function \chi_{C} of C is defined by \chi_{C}(x) = \begin{cases} 0 & x \notin C, \\ 1 & x \in C .\end{cases} 

If C \subset A for some closed rectangle A and f : A \to \mathbf{R} is bounded, then \int_{C} f is defined as \int_{A} f \cdot \chi_{C}, provided f \cdot \chi_{C} is integrable.

(Thm 3.9) The function \chi_{C} : A \to \mathbf{R} is integrable iff the boundary of C has measure 0, (and hence content 0).

(Def) A bounded set C whose boundary has measure 0 is called Jordan-measurble. The integral \int_{C} 1 is called (n-dimensional) content of C, or the (n-dimensional) volume of C. one-dimensional is often called length, and two-dimensional volume, area.

(subsection) Fubini’s Theorem

(Def) If f : A \to \mathbf{R} is a bounded function on a closed rectangle, then whether or not f is integrable, the least upper bound of all lower sums, and the greatest lower bound of all upper sums, both exist. They are called the lower and upper integrals of f on A, and denoted \mathbf{L} \int_{A} f and \mathbf{U} \int_{A} f.

(Fubini’s Theorem) (Thm 3.10) Let A \subset \mathbf{R}^{n} and B \subset \mathbf{R}^{m} be closed rectangles, and let f : A \times B \to \mathbf{R} be integrable. for x \in A let g_{x} : B \to \mathbf{R} be defined by g_{x} (y) = f(x,y) and let 

\mathcal{L}(x) = \mathbf{L} \int_{B} g_{x} = \mathbf{L} \int_{B} f(x,y) dy,

\mathcal{U}(x) = \mathbf{U} \int_{B} g_{x} = \mathbf{U} \int_{B} f(x,y) dy.

Then \mathcal{L} and \mathcal{U} are integrable on A and

\int_{A \times B} f = \int_{A} \mathcal{L} = \int_{A} (\mathbf{L} \int_{B} f(x,y) dy) dx,

\int_{A \times B} f = \int_{A} \mathcal{U} = \int_{A} (\mathbf{U} \int_{B} f(x,y) dy) dx,

The integrals on the right side are called iterated integrals for f.

(Prop)

\int_{A \times B} f = \int_{A} (\int_{B} f(x,y) dy) dx, if f is continuous.

In the case g_{x} is not integrable for a finite number of x \in A, then \int_{A \times B} f = \int_{A} (\int_{B} f(x,y) dy) dx, provided that \int_{B} f(x,y) dy is defined arbitrarily, say as 0, when it does not exist.

Let f : [0,1] \times [0,1] \to \mathbf{R} be defined by f(x,y) = \begin{cases}1 & if x is irrational \\ 1 & if x is rational and y is irrational \\ 1 - \frac{1}{q} & if x = \frac{p}{q} in lowest terms and y is rational  \end{cases} , Then f is integrable and \int_{[0,1] \times [0,1]} f = 1. Now \int_{0}^{1} f(x,y) dy = 1 if x is irrational, and does not exist if x is rational.

If A = [a_{1}, b_{1} ] \times \cdots \times [a_{n}, b_{n} ] and f : A \to \mathbf{R} is sufficiently nice, \int_{A} f = \int_{a_{n}}^{b_{n}} ( \cdots ( \int_{a_{1}}^{b_{1}} f(x^{1} , \cdots, x^{n}) dx^{1}) \cdots ) dx^{n}.

If C \subset A \times B, Fubini’s theorem can be used to evaluate \int_{C} f, since this is \int_{A \times B} \chi_{C} f.

(subsecton) Partitions of unity

(Thm 3.11) Let A \subset \mathbf{R}^{n} and let \mathcal{O} be an open cover of A. Then there is a collection \Phi| of C^{\infty} functions \phi defined in an open set containing A, with the following properties :

For each x \in A we have 0 \le \phi(x) \le 1.

For each x \in A there is an open set V containing x s.t. all but finitely many \phi \in \Phi are 0 on V.

For each x \in A we have \sum_{\phi \in \Phi} \phi(x) = 1 ( by (2) for each x this sum is finite in some open set containing x)

For each \phi \in \Phi there is an open set U in \mathcal{O} s.t. \phi = 0 outside of some closed set containing in U.

A collection \Phi satisfying 1st and 3rd property is called a C^{\infty} partition of unity for A. If \Phi also satisfies 4th property , it is said to be subordinate to the cover \mathcal{O}.

(prop) Let C \subset A be compact. only finitely many \phi \in \Phi are not 0 on C.

(Def) An open cover \mathcal{O} of an open set A \subset \mathbf{R}^{n} is admissible if each U \in \mathcal{O} is contained in A. If \Phi is subordinate to \mathcal{O}, f : A \to \mathbf{R} is bounded in some open set around each point of A, and {x : f is discontinuous at x} has measure 0, then each \int_{A} \phi \cdot |f| exists. we define f to be integrable (in the extended sense) if \sum_{\phi \in \Phi} \int_{A} \phi \cdot |f| converges.

(Thm 3.12) If \Psi is another partition of unity, subordinate to an admissible cover \mathcal{O}’ of A< then \sum_{\psi \in \Psi} \int_{A} \psi \cdot |f| also converges, and \sum_{\phi \in \Phi} \int_{A} \phi \cdot f = \sum_{\psi \in \Psi} \int_{A} \psi \cdot f.

If A and f are bounded, then f is integrable in the extended sense.

If A is Jordan-measurable and f is bounded, then this definition of \int_{A} f agrees with the old one.

(subsection) Change of Variable)

(Prop) If g : [a,b] \to \mathbf{R} is continuously differentiable and f : \mathbf{R} to \mathbf{R} is continuous, then, \int_{g(a)}^{g(b)} f = \int_{a}^{b} (f \bullet g) \cdot g’ .

(Thm 3.13) Let A \subset \mathbf{R}^{n} be an open set and g : A \to \mathbf{R}^{n} a 1-1, continuously differentiable function s.t. det g’(x) \neq 0 for all x \in A. If f: g(A) \to \mathbf{R} is integrable, then \int_{g(A)} f = \int_{A} (f \bullet g) |det g’ | .

(Sard’s Theorem) (Thm 3.14) Let g : A \to \mathbf{R}^{n} be continuously differentiable, where A \subset \mathbf{R}^{n} is open, and let B = { x \in A : det g’(x) = 0} . Then g(B) has measure 0.

