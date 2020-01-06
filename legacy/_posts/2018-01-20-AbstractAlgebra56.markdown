---



layout: post



title : (Abstract Algebra) Insolvability of the Quintic



date : 2018-01-20 14:54:24 +0900



---

(Section 56) Insolvability of the Quintic

(subsection) Extensions by Radicals

(Def 56.1) An extension K of a field F is an extension of F by radicals if there are elements \alpha_{1} , \cdots, \alpha_{r} \in K and positive integers n_{1}, \cdots, n_{r} s.t. K = F(\alpha_{1}, \cdots, \alpha_{r}) , \alpha_{1}^{n_{1}} \in F and \alpha_{i}^{n_{i}} \in F(\alpha_{1}, \cdots, \alpha_{i-1}) for 1 < i \le r. A polynomial f(x) \in F[x] is solvable by radicals over F if the splitting field E of f(x) over F is contained in an extension of F by radicals.

(Lem 56.3) Let F be a field of characteristic 0, and let a \in F . If K is the splitting field of x^{n} -a over F, then G(K/F) is a solvable group.

(Thm 56.4) Let F be a field of characteristic zero, and let F \le E \le K \le \bar{F}, where E is a normal extension of F and K is an extension of F by radicals. Then G(E/F) is a solvable group.

(subsection) Insolvability of the Quintic

(Def) Let y_{1} \in \mathbb{R} be transcendental over \mathbb{Q}, y_{1} \in \mathbb{R} be transcendental over \mathbb{Q}(y_{1}) , and so on, until we ger y_{5} \in \mathbb{R} transcendental over \mathbb{Q} (y_{1}, \cdots , y_{4} ). It can be shown by a counting argument that such transcendental real numbers exist. Transcendentals found in this fashion are independent transcendental elements over \mathbb{Q}. 

(Def) Elementary symmetry functions in the y_{i}, namely

s_{1} = y_{1} + y_{2} + \cdots + y_{5}

s_{2} = y_{1}y_{2} + y_{1}y_{3} + y_{1}y_{4} + y_{1}y_{5} + y_{2}y_{3} + \cdots + y_{3}y_{5} + y_{4}y_{5} , 

\vdots

s_{5} = y_{1}y_{2}y_{3}y_{4}y_{5}

(Thm 56.6) Let y_{1}, \cdots, y_{5} be independent transcendental real numbers over \mathbb{Q}. The polynomial f(x) = \prod_{i = 1}^{5} (x-y_{i}) is not solvable by radicals over F = \mathbb{Q} (s_{1}, \cdots, s_{5}) , where s_{i} is the ith elementary symmetric function in y_{1}, \cdots , y_{5}.



