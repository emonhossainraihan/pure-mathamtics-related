---



layout: post



title : [Abstract Algebra] CHomological Algebra



date : 2018-01-20 14:52:24 +0900



---

(Section 44) Homological Algebra

(subsection) Chain complexes and Mappings

(Def) For a simplical complex X, we get chain groups C_{k} (X) and maps \partian_{k} , as indicated in the diagram.

with \partial_{k-1} \partial_{k} = 0. Abstract purely algrbraic portion of this situation and consider any sequence of abelian groups A_{k} and homomorphisms \partial_{k} : A_{k} \to A_{k-1} such that \partial_{k-1} \partial_{k} = 0 for k \ge 1. Often A_{k} = 0 for k < 0 and k > n in applications.

(Def 44.1) Chain complex \langel A, \partial \rangle is a doubly infinite sequence A = { \cdots , A_{2} , A_{1}, A_{0}, A_{-1} , A_{-2}, \cdots } of abelian groups A_{k}, together with a collection \partial = {\partial_{k} | k \in \mathbb{Z} } of homomorphisms s.t. \partial_{k} : A_{k} \to A_{k-1} and \partial_{k-1} \partial_{k} = 0.

(Thm 44.2) If A is a chain complex, then the image under \partial_{k} is a subgroup of the kernel of \partial_{k-1}.

(Def 44.3) If A is a chain complex, then the kernel Z_{k} (A) of \partial_{k} is the group of k-cycles, and the image B_{k} (A) = \partial_{k+1} [A_{k+1}] is the group of k-boundaries. The factor group H_{k} (A) = Z_{k} (A) / B_{k} (A) is the kth homology group of A.

(Fundamental lemma) (Thm 44.4) Let A and A’ with collections \partial and \partial ‘ of homomorphisms be chain complexes, and suppose that there is a collection f of hoomorphisms f_{k} : A_{k} \to A’_{k} as indicated in the diagram .

Suppose, furthermore, that every square is commutative, that is, f_{k-1} \partial_{k} = \partial’_{k} f_{k} for all k, Then f_{k} induces a natural homomorphism f_{*k} : H_{k} (A) \to H_{k} (A’).

(Def) If the collections of maps f, \partial, and \partial’ have the property f_{k-1} \partial_{k} = \partial’_{k}, that the squares are commutative, then f commutes with \partial.

(Def 44.5) A chain complex \langle A’ , \partial’ \rangle is a subcomplex of a chain complex \langle A , \partial \rangle , if for all k, A_{k}’ is a subgroup of A_{k{ and \partial’_{k} (C) = \partial_{k} (c) for every c \in A’_{k} , that is \partial’_{k} and \partial_{k} have the same effect on elements of the subgroup A’_{k} of A_{k}.

(subsection) Relative Homology

(Def) Suppose that A’ is a subcomplex of the chain complex A. simplical subcomplex Y of a simplical complex X. We can then naturally consider C_{k} (Y) a subgroup of C_{k}(X). \partial_{k} [C_{k} (Y) ] \le C_{k-1} (Y)

If A’ is a subcomplex of the chain complex A, we can form the collection A/A’ of factor groups A_{k}/A’_{k} . a collection \bar{\partial} of homomorphisms \bar{\partial_{k} } : ( A_{k} / A’_{k} ) \to (A_{k-1} / A’_{k-1}) : \bar{\partial_{k}} (c + A’_{k}) = \partial_{k} (c) + A’_{k-1} for c \in A_{k}. then \bar{\partial}_{k-1} \bar{\partial}_{k} = 0

(Thm 44.7) If A’ is a subcomplex of the chain complex A, then the collection A/A’ of factor groups A_{k} / A’_{k} together with collection \bar{\partial} of homomorphisms \bar{\partial}_{k} defined by \bar{\partial_{k}} (c + A’_{k}) = \partial_{k} (c) + A’_{k-1} for c \in A_{k} is a chain complex.

(Def) The homology group H_{k} (A/A’) is the kth relative homology group of A modulo A’.

(subsection) Exact Homology Sequence of a Pair

(Lem 44.14) Let A’ be a subcomplex of a chain complex A. Let j be the collection of natural homomorphisms j_{k} : A_{k} \to (A_{k}/A’_{k}). Then j_{k-1} \parital_{k} = \bar{\partial}_{k} j_{k}, that is, j commutes with \partial.

(Thm 44.15) the map j_{k} of (Lem 44.14) induces a natural homomorphism j_{*k} : H_{k} (A) \to H_{k} (A/A’) .

(Lem 44.16) The map \partial_{*k} : H_{k} (A/A’) \to H_{k-1} (A’) : \partial_{*k}(h) = \partial_{k} (c) + B_{k-1} (A’) is well defined and is a homomorphism of H_{k} (A/A’) into H_{k-1} (A’).

(Lem 44.17) Let i_{*k} be the map i_{*k} : H_{k}(A’) \to H_{k}(A) induced from collection i of injection mappings i_{k} : A’_{k} \to A_{k} : i_{k}(c) = c for c \in A’_{k}. We can construct a following diagram.

The groups in diagram, together with given maps, form a chain complex.

(Def 44.18) A sequence of groups A_{k} and homomorphisms \parital_{k} forming a chain complex is an exact sequence if all the homology groups of the chain complex are 0, that is, if for all k we have that the image under \partial_{k} is equal to the kernel of \partial_{k-1}.

(Thm 44.19) The groups and maps of the chain complex in diagram (Lme 44.17) form an exact sequence.

(Def 44.20) The exact sequence in diagram (Lem 44.17) is the exact homology sequence of the pair (A,A’).

