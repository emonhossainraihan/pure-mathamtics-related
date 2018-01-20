---



layout: post



title :  Computations of Homology Groups



date : 2018-01-20 14:52:14 +0900



---

(Section 42) Computations of Homology Groups

(Def) If a space is divided up into pieces in such a way that near each point the space can be deformed to look like a part of some Euclidean space \mathbb{R}^{n} and the pieces into which the space was divided appear after this deformation as part of a simplical complex, then the original division of the space is a triangulation of the space.

homology groups of the space are defined formally as in the last section.

(Prop) invariance properties of homology groups.

The homology groups of a space are defined in terms of a triangulation, but is the same (isomorphic) groups no matter how the space is trangulated.

If one triangulated space is homeomorphic to another, the homology groups of the two spaces are the same (isomorphic) in each dimension n.

(Def) n-sphere S^{n} is the set of all points a distance of 1 unit from the origin in (n+1)-dimensional Euclidean space \mathbb{R}^{n+1}. The n-cell or n-ball E^{n} is the set of all points in \mathbb{R}^{n} a dinstance \le 1 from the origin.

(subsection) Connected and Contractable Spaces

(Def) A space is connected if any two points in it can be joined by a path lying totally in the space. If a space is not connected, it is split up into a number of pieces, each of which is connected buy no two of which can be joined by a path in space. These pieces are the connected components of the space.

(Thm 42.4) If a space X is trangulated into a finite number of simplexes, then H_{0} (X) is isomorphic to \mathbb{Z} \times \mathbb{Z} \times \cdots \times \mathbb{Z}, and the Betti number m of factors \mathbb{Z} is the number of connected componenets of X.

(Def) a space is contractible if it can be compressed to a point without being torn or cut, but always kept within the space it originally occupied.

(Thm 42.6) If X is a contractible space triangulated into a finite number of simplexes, then H_{n} (X) = 0 for n \ge 1.

E^{n} is contractable for n \ge 1, so H_{1} (E^{n}) = 0 for i > 0.

(prop) For n > 0, H_{n} (S^{n}) and H_{0}(S^{n}) are isomorphic to \mathbb{Z}, while H_{i} (S^{n}) = 0 for 0 < i < n.

(Def) an element of H_{n} (X), that is, a coset of B_{n} (X) in Z_{n} (X), a homology class. Cycles in the same homology class are homologous.

(Section 43) More Homology computations and applications

(Def) one-sided closed surface, the Klein bottle. the 1-dimensional homology group will have a nontrivial torsion subgroup reflecting the twist in the surface.

(subsection) Euler Characteristic

(Def) Let X be a finite simplical complex consisting of simplexes of dimension 3 and less, Let n_{0} be the total number of vertices in the triangulation, n_{1} the number of edges, n_{2} the number of 2-simplexes, and n_{3} the number of 3-simplexes. The number n_{0} – n_{1} + n_{2} – n_{3} = \sum_{i = 0}^{3} (-1)^{i} n_{i} is same no matter how the space X is triangulated. This number is the Euler characteristic \chi (X) of the space. 

(Thm 43.7) Let X be a finite simplical complex (or triangulated space) of dimension \le 3. Let \chi (X) be the Euler characteristic of the space X, and let \beta_{j} be the Betti number of H_{j} (X). Then \chi (X) = \sum_{j = 0}^{3} (-1)^{j} \beta_{j} . This theorem holds also for X of dimension greater than 3, with the extension of the definition of the Euler characteristic to dimension greater than 3.

(subsection) Mapping of Spaces

(prop) a continuous function f mapping a space X into a space Y gives rise to a homomorphism f_{*n} mapping H_{n} (X) into H_{n} (Y) for n >0.

(prop) If z \in \mathbb{Z}_{n} (X), and if f(z), regarded as the result of picking up z and setting it down in Y in the naively obvious way, should be an n-cycle in Y, then f_{*n} (z + B_{n} (X)) = f(z) + B_{n} (Y). That is, if z represents a homology class in H_{n} (X) and f(z) is an n-cycle in Y, then f(z) represents the image homology class under f_{*n} of the homology class containing z.

(Def) a fixed point is some x \in E^{n} s.t. f(x) = x.

(Brower Fixed-point Theorem) (Thm 43.12) A continuous map f of E^{n} into itself has a fixed point for n \ge 1.

