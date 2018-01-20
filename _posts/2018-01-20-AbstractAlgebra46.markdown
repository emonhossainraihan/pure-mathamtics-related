---



layout: post



title : (Abstract Algebra) CEuclidean Domains



date : 2018-01-20 14:52:44 +0900



---

(Section 46) Euclidean Domains

(Def 46.1) Euclidean norm on an integral domain D is a function \nu mapping the nonzero elements of D into the nonnegative integers s.t. the following conditions are satisfied.

For all a,b \in D with b \neq 0, there exist q and r in D s.t. a = bq + r, where either r = 0 or \nu (r) < \nu (b).

For all a, b \in D, where neither a nor b is 0, \nu (a) \le \nu (ab).

An integral domain D is a Euclidean domain if there exists a Euclidean norm on D.

(Thm 46.4) Every Euclidean domain is a PID.

(Cor 46.5) A Euclidean domain is a UFD.

(subsection) Arithmetic in Euclidean Domains

(Thm 46.6) For a Euclidean domain with a Euclidean norm \nu, \nu(1) is minimal among all \nu (a) for nonzero a \in D, and u \in D is a unit iff \nu (u) = \nu (1).

(Euclidean Algorithm) (Thm 46.9) Let D be a Euclidean domain with a Euclidean norm \nu, and let a and b be nonzero elements of D. Let r_{1} be as in first condition for a Euclidean norm, that is a = bq_{1} + r_{1} where either r_{1} = 0 or \nu (r_{1}) < \nu (b) . If r_{1} \neq 0, let r_{2} be s.t. b = r_{1} q_{2} + r_{2} where either r_{2} = 0 or \nu (r_{2}) < \nu (r_{1}) . In general, let r_{i+1} be s.t. r_{i-1} = r_{i} q_{i+1} + r_{i+1} where either r_{i+1} = 0 or \nu (r_{i+1}) < \nu (r_{i}) . Then the sequence r_{i}, r_{2}, \cdots must terminate with some r_{s} = 0. If r_{1} = 0, then b is a gcd of a and b. If r_{1} \neq 0 and r_{s} is the first r_{i} = 0, then a gcd of a and b is r_{s-1}. Furthemore, if d is a gcd of a and b, then there exist \lambda and \mu in D s.t. d = \lambda a + \mu b.

