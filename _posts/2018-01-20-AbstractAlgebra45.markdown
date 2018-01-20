---



layout: post



title : [Abstract Algebra] CFactorization



date : 2018-01-20 14:52:34 +0900



---

(Section IX) Factorization

(Section 45) Unique Factorization Domains

(Def 45.1) Let R be a commutative ring with unity and let a, b \in R. If there exists c \in R s.t. b = ac, then a divides b (or a is a factor of b), denoted by a|b .

We read a \nmid b as “a does not divide b.”

(Def 45.2) an element u of a commutative ring with unity R is a unit of R if u divides 1, that is, if u has a multiplicative inverse in R. Two elements a, b \in R are associated in R if a = bu, where u is a unit in R.

(Def 45.4) A nonzero element p that is not a unit of an integral domain D is an irreducible of D if in every factorization p = ab in D has the property that either a or b is a unit.

(Def 45.5) An integral domain D is a unique factorization domain (UFD) if the following conditions are satisfied.

Every element of D that is neither 0 nor a unit can be factored into a product of a finite number of irreducibles.

If p_{1} \cdots p_{r} and q_{1} \cdots q_{s} are two factorizations of the same element of D into irreducibles, then r = s and the q_{j} can be renumbered so that p_{i} and q_{i} are associates.

(Def 45.7) An integral domain D is a principal ideal domain (PID) if every ideal in D is a principal ideal.

(subsection) Every PID is a UFD

(Def 45.8) If {A_{i} | i \in I} is a collection of sets, then the union \bigcup_{i \in I} A_{i} of the sets A_{i} is the set of all x s.t. x \in A_{i} for at least one i \in I.

(Lem 45.9) Let R be a commutative ring and let N_{1} \subseteq N_{2} \subseteq \cdots be an ascending chain of ideals N_{i} in R. Then N = \bigcup_{i} N_{i} is an ideal of R.

(Ascending Chain condition for a PID) (Lem 45.10) Let D be a PID. If N_{1} \subseteq N_{2} \subseteq \cdots is an ascending chain of ideals N_{i}, then there exists a positive integer r s.t. N_{r} = N_{s} for all s \ge r. Equivalently, every strictly ascending chain of ideals (all inclusions proper) in a PID is of finite length. 

We express this by saying that the ascending chain condition (ACC) holds for ideals in a PID.

(Thm 45.11) Let D be a PID. Every element that is neither 0 nor a unit in D is a product of irreducibles.

(Lem 45.12) An ideal \langle p \rangle in a PID is maxial iff p is an irreducible.

(Lem 45.13) In a PID, if an irreducible p divides ab, then either p | a or p | b.

(Cor 45.14) If p is an irreducible in a PID and p divides the product a_{1}a_{2} \cdots a_{n} for a_{i} \in D , then p | a_{i} for at least one i.

(Def 45.15) A nonzero nonunit element p of an integral domain D is a prime if, for all a, b \in D, p | ab implies either p | a or p | b.

(Thm 45.17) Every PID is a UFD.

(Fundamental Theorem of Arithmetic) (Cor 45.18) The integral domain \mathbb{Z} is a UFD.

(subsection) If D is a UFD, then D[x] is a UFD

(Def 45.19) Let D be a UFD and let a_{1}, a_{2}, \cdots , a_{n} be nonzero elements of D. An element d of D is a greatest common divisor (gcd) of all of the a_{i} if d | a_{i} for i = 1, \cdots ,n and any other d’ \in D that divides all the a_{i} also divides d.

(Def 45.21) Let D be a UFD. a nonconstant polynomial f(x) = a_{0} + a_{1} x + \cdots + a_{n} x^{n} in D[x] is primitive if 1 is a gcd of the a_{i} for i = 0,1, …, n.

(Lem 45.23) If D is a UFD, then for every nonconstant f(x) \in D[x] we have f(x) = (c)g(x), where c \in D, g(x) \in D[x], and g(x) is primitive. The element c is unique up to a unit factor in D and is the content of f(x). Also g(x) is unique up to a unit factor in D.

(Gauss’s Lemma) (Lem 45.25) If D is a UFD, then a product of two primitive polynomials in D[x] is again primitive.

(Cor 45.26) If D is a UFD, then a finite product of primitive polynomials in D[x] is again primitive.

(Lem 45.27) Let D be a UFD and let F be a field of quotients of D. Let f(x) \in D[x], where (degree f(x)) > 0. If f(x) is an irreducible in D[x], then f(x) is also an irreducible in F[x]. Also, if f(x) is primitive in D[x] and irreducible in F[x], then f(x) is irreducible in D[x].

(Cor 45.28) If D is a UFD and F is a field of quotients of D, then a nonconstant f(x) \in D[x] factors into a product of two polynomials of lower degrees r and s in F[x] iff it has a factorization into polynomials of the same degrees r and s in D[x].

(Thm 45.29) If D is a UFD, then D[x] is a UFD.

(Cor 45.30) If F is a field and x_{1} , \cdots x_{n} are indeterminates, then F[x_{1}, \cdots x_{n} ] is a UFD.

