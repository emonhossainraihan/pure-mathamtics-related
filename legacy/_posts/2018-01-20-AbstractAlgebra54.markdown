---



layout: post



title : (Abstract Algebra) Illustrations of Galois Theory



date : 2018-01-20 14:54:04 +0900



---

(Section 54) Illustrations of Galois Theory

(subsection) Symmetric Functions

(Def) Let F be a field, and let y_{1}, \cdots , y_{n} be indeterminates. There are some natural automorphisms of F(y_{1}, \cdots , y_{n}) leaving F fixed, those defined by permutations of {y_{1}, \cdots , y_{n} . Let \sigma be a permutation of {1, \cdots , n}, that is, \sigma \in S_{n}. Then \sigma gives rise to a natural map \bar{\sigma} : F(y_{1}, \cdots , y_{n}) \to F(y_{1}, \cdots , y_{n} ) given by \bar{\sigma} \biggl( \frac{f(y_{1} , \cdots, y_{n} ) }{ g(y_{1}, \cdots, y_{n}) } \biggr) = \frac{f(y_{\sigma (1)} , \cdots, y_{\sigma (n)} ) }{ g(y_{\sigma (1)}, \cdots, y_{\sigma (n)})} for f(y_{1}, \cdots, y_{n}) , g(y_{1}, \cdots, y_{n}) \in F[y_{1}, \cdots , y_{n} ] , with g(y_{1}, \cdots, y_{n}) \neq 0. \bar{sigma} is an automorphism of F(y_{1}, \cdots, y_{n}) leaving F fixed.

The elements F(y_{1}, \cdots, y_{n}) left fixed by all \bar{\sigma} , for all \sigma \in S_{n}, are those rational functions that are symmetric in the indeterminates y_{1}, \cdots , y_{n} .

(Def 54.1) An element of the field F(y_{1}, \cdots , y_{n}) is a symmetric function in y_{1}, \cdots , y_{n} over F, if it is left fixed by all permutations of y_{1}, \cdots , y_{n}, in the sense as explained above.

(Thm 54.2) Let s_{1}, \cdots , s_{n} be the elementary symmetric functions in the indeteminates y_{1}, \cdots , y_{n} . Then every symmetric function of y_{1}, \cdots, y_{n} over F is a rational function of the elementary symmetric funcitons, 

Also, F(y_{1}, \cdots, y_{n} ) is a finite normal extension of degree n! of F(s_{1}, \cdots , s_{n}) , and the Galois group of this extension is naturally isomorphic to S_{n}.

