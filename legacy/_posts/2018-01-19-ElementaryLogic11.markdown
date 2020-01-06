---

layout: post

title : (Elementary Logic)  Formalized Theory

date : 2018-01-19 13:52:14 +0900

---

11	Formalized Theory

11.1	Elementary theory : a theory formalized by means of elementary logic

11.2	Introduction

11.2.1	Deductive theory T formalized in the first order predicate calculus : a pair of sets T = <Δ,Γ> where Δ is a set of non-logical constants of L containing at least one predicate of degree ≥ 1 and Γ is a set of sentences of L satisfying the conditions

11.2.1.1	 All non-logical constants occurring in members of Γ are members of Δ

11.2.1.2	 Deductively closed : Every sentence of T that is a consequence of Γ is a member of Γ

11.2.2	Non-logical Vocabulary of T = <Δ,Γ> : Δ

11.2.3	Assertions, Theses of T = <Δ,Γ> : Γ

11.2.3.1	Deductive theory is uniquely determined by its non-logical vocabulary and its assertions.

11.2.4	Deductive theory T formalized in the first order predicate calculus with identity ( or with identity and operation symbols) : Similar, but now referring to L_{1} (or L’)

11.2.5	Consistent ( a theory T) : no sentence and its negation are both asserted by T

11.2.6	Complete ( a theory T) : For any sentence of T, either that sentence or its negation is asserted by T.

11.2.6.1	Every inconsistent theory is automatically complete

11.2.7	Independent (a set of sentences Γ) : no element Φ of Γ ~ {Φ} (special notation ~)

11.2.8	Decidable ( a set of sentences Γ) : there is a step-by-step procedure which, applied to an arbitrary expression Φ, will decide in a finite number of steps whether or not Φ belongs to Γ.

11.2.9	Axiomatizable ( a theory T) : among the assertions of a given theory T there is a decidable subset ① of which all the others are consequences

11.2.9.1	Set of axioms of T : ①

11.2.9.2	Axiomatic theory : T 

11.2.10	Heteronomous system : an axiom system proposed next and judged first on the basis of whether or not the resulting theorems coincide with the assertions

11.2.11	Autonomous : axiom system proposed first and the theses of the theory are defined as those sentences of the theory following from the axioms

11.2.12	Evaluation of axiom system

11.2.12.1	Consistency

11.2.12.1.1	Semantically : give an interpretation under which all the axioms are true

11.2.12.1.2	Syntactically : without reference to interpretations, there is no sentence Φ s.t. both Φ and -Φ are derivable from the axioms

11.2.12.2	Complete : theory from an axiom system is complete

11.2.12.3	Independence : give each axiom an interpretation under which it is false but the remaining axioms are true

11.2.12.4	Categorical : all its models are isomorphic

11.2.12.4.1	Any consistent axiom system has infinitely many models.

11.2.12.4.2	(Isomorphic model) Given a set of sentences Γ of L’, interpretation I_{1} and I_{2} are isomorphic models of Γ iff 

11.2.12.4.2.1	I_{1} and I_{2} are models of Γ

11.2.12.4.2.2	 There is a 1-1 relation between the domains of I_{1} and I_{2} associating with each element e of the domain of I_{1} exactly one element e* of the domain of I_{2}

11.2.12.4.2.3	For each sentential letter Φ occurring in Γ, I_{1}(Φ) = I_{2}(Φ)

11.2.12.4.2.4	For each individual constant β occurring in Γ, I_{2}(β) = I_{1}(β)*

11.2.12.4.2.5	For each n-ary predicate θ occurring in Γ, the n-tuple <t_{1}, t_{2}, …, t_{n}> ∈ I_{1}(θ) iff <t_{1}*, t_{2}*, .., t_{n}*> ∈ I_{2}(θ), for all elements t_{1}, t_{2}, .. , t_{n} of the domain of I_{1}

11.2.12.4.2.6	For each n-ary operation θ occurring in Γ, the n-tuple <t_{1}, t_{2}, …, t_{n}, η> ∈ I_{1}(θ) iff <t_{1}*, t_{2}*, .., t_{n}*, η*> ∈ I_{2}(θ), for all elements t_{1}, t_{2}, .. , t_{n}, η of the domain of I_{1}

11.2.12.4.3	If there are models with different cardinality, the theory is not categorical.

11.2.12.4.4	Representation theorem : While not all models of the theory of groups are isomorphic to one another, every such model is isomorphic to a group of transformations.

11.3	Aristotelian syllogistic

11.3.1	  T1 

11.3.1.1	Non-logical vocabulary of T1 : binary predicates A^{2}, E^{2}, I^{2}, O^{2}

11.3.1.2	Axioms of assertions

11.3.1.2.1	(x)(y)(z)((A_{yz}&A_{xy})\\(\implies\)A_{xz}) (Barbara)

11.3.1.2.2	(x)(y)(z)((E_{yz}&A_{xy})\\(\implies\)E_{xz}) (Celarent)

11.3.1.2.3	(x)(y)(I_{xy} \\(\implies\) I_{yx}) (Conversion of ‘I’)

11.3.1.2.4	(x)(y)(E_{xy} \\(\implies\) E_{yx}) (Conversion of ‘E’)

11.3.1.2.5	(x)(y)(A_{xy} \\(\implies\) I_{yx}) (Conversion of ‘A’)

11.3.1.2.6	(x)(y)(E_{xy} \\(\implies\) -I_{yx}) (Definition of ‘E’)

11.3.1.2.7	(x)(y)(O_{xy} \\(\implies\) -A_{yx}) (Definition of ‘O’)

11.3.1.3	 Evaluation of T1

11.3.1.3.1	T1 is consistent

11.3.1.3.2	T1 is not complete

11.3.1.3.3	T1 is not independent

11.3.1.3.4	T1 is not categorical

11.3.1.4	 TH : Brevity convention

11.3.1.4.1	Any instance of an axiom or previously proved theorem may be entered on a line, with the empty set of premise numbers

11.3.1.4.2	Ψ may enter the line if Φ_{1}, …, Φ_{n} appear on earlier lines and Ψ is a tautological consequence of { Φ_{1}, …, Φ_{n} } and an instance of an axiom or previously proved theorem; as premise numbers of the new line take all premise-numbers of those earlier lines.

11.4	The theory of betweenness

11.4.1	T2 : axiomatized theory formulated in the first order predicate calculus with identity

11.4.1.1	Non-logical vocabulary : B^{3} (ternary)

11.4.1.2	Assertions : sentences that are true under every interpretation I satisfying :

11.4.1.2.1	The domain of I is the set of all points on some (Euclidean) straight line

11.4.1.2.2	I assigns to B^{3} the relation of betweenness “② is between ① and ③” Among points on this straight line.

11.4.1.3	Evaluation of T2

11.4.1.3.1	T2 is consistent

11.4.1.3.2	T2 is complete

11.4.1.4	Axioms of assertions

11.4.1.4.1	(x)(y)(Bxyx \\(\implies\) x = y)

11.4.1.4.2	(x)(y)(z)(u)((Bxyu & Byzu) \\(\implies\) Bxyz)

11.4.1.4.3	(x)(y)(z)(u)(((Bxyz & Byzu) & y != z) \\(\implies\) Bxyu)

11.4.1.4.4	(x)(y)(z)((Bxyz v Bxzy ) b (Bzxy)

11.4.1.4.5	(∃x)(∃y)x != y

11.4.1.4.6	(x)(y) (x != y \\(\implies\) (∃z)(Bxyz & y != z))

11.4.1.4.7	(x)(y)(x != y \\(\implies\) (∃z)(Bxzy & (z != x & z != y)))

11.5	Groups; Boolean algebras

11.5.1	T3 : Theory of groups formalized in the language L’

11.5.1.1	Non-logical vocabulary of T3 : 

11.5.1.1.1	(Group addition) binary operation symbol f^{2}

11.5.1.1.2	(Group complementation) : singulary operation symbol f^{1}

11.5.1.1.3	(identity element) : individual constant e

11.5.1.2	Assertions

11.5.1.2.1	 Conventions : Suppose τ, τ’ are terms or the result of previous application of these conventions

11.5.1.2.1.1	(τ + τ’) \\(\Longleftarrow\) f^{2}ττ’

11.5.1.2.1.2	Τ* for f^{1}τ

11.5.1.2.2	Axioms of assertions

11.5.1.2.2.1	(x)(y)(z) x + (y + z) = (x + y) + z

11.5.1.2.2.2	(x) x + e = x

11.5.1.2.2.3	(x) x + x* = e

11.5.1.3	Evaluation of T3

11.5.1.3.1	T3 is consistent

11.5.1.3.2	T3 is not complete

11.5.1.3.3	T3 is independent

11.5.1.3.4	T3 is not categorical

11.5.2	T4 : Boolean algebras : first order predicate calculus with identity and operation symbols

11.5.2.1	Non-logical vocabulary 

11.5.2.1.1	 F^{1}, f^{2}, g^{2}, n, e

11.5.2.1.2	Convention

11.5.2.1.2.1	(τ U τ’) \\(\Longleftarrow\) f^{2}ττ’

11.5.2.1.2.2	(τ ∩ τ’) \\(\Longleftarrow\) g^{2}ττ’

11.5.2.1.2.3	Τ* \\(\Longleftarrow\) f^{1}τ

11.5.2.1.2.4	0 \\(\Longleftarrow\) n

11.5.2.1.2.5	1 \\(\Longleftarrow\) e

11.5.2.2	Axioms for assertions

11.5.2.2.1	(x)(y) x ∩ y = y ∩ x

11.5.2.2.2	(x)(y) x U y = y U x

11.5.2.2.3	(x)(y)(z) x ∩ ( y ∩ z ) = (x ∩ y) ∩ z

11.5.2.2.4	(x)(y)(z) x U ( y U z ) = (x U y) U z

11.5.2.2.5	(x)(y) x ∩ (x U y ) = x

11.5.2.2.6	(x)(y) x U (x ∩ y ) = x

11.5.2.2.7	(x)(y)(z) x ∩ ( y U z ) = (x ∩ y) U (x ∩ z)

11.5.2.2.8	(x)(y)(z) x U ( y ∩ z ) = (x U y) ∩ (x U z)

11.5.2.2.9	 (x) x ∩ x* = 0

11.5.2.2.10	(x) x U x* = 1

11.5.2.2.11	0 != 1

11.5.2.3	Evaluation of T4

11.5.2.3.1	T4 is consistent

11.5.2.3.2	T4 is not complete

11.5.2.4	Dual of a theorem is a theorem

11.5.2.4.1	Dual : interchange of ∩ and U in a sentence of T4

11.6	Definition

11.6.1	To introduce notation that does not belong to the vocabulary of the theory but may improve readability of the formulas and render their content more clear

11.6.1.1	Metalinguistic sentence asserting that a given symbol of the object language means the same as some other object language expression

11.6.1.2	As an object language sentence of a certain form (usually an identity or biconditional or a generalized identity or biconditional, with the new symbol appearing on the left side alone or in a simple context)

11.6.2	Definition can lead to contradiction not just by its forms but also by the content of the theory

11.6.3	Criteria of Definition

11.6.3.1	Creative ( a definition ) : Generates new theorems in which the defined symbol does not occur 

11.6.3.2	Definition should make the defined symbol eliminable

11.6.3.2.1	Resistance to circular definitions

11.6.3.3	Let T = (Δ,Γ) be theory. Let θ be a non-logical constant that does not belong to Δ. Let Φ be a sentence of L’ containing θ and otherwise formulated solely in terms of the vocabulary Δ. If we add Φ to the theses of T we get new theory T’ = (Δ U {θ} , {all sentences of T’ that are consequences of Γ U {Φ}}).

11.6.3.3.1	 As a definition of θ related to T, Satisfies the criterion of eliminability ( a sentence Φ) : for every formula Ψ of T’, there is a formula χ of T’ s.t. all closures of Ψ\\(\iff\\)χ are theses of T’ and χ does not contain θ.

11.6.3.3.2	 As a definition of θ related to T, Satisfies the criterion of non-creativity ( a sentence Φ) : every thesis of T’ that does not contain θ is a thesis of T

11.6.4	Construction of formally correct definitions

11.6.4.1	Let T be a theory formulated in L’, and suppose θ is a non-logical constant which does not occur in T.

11.6.4.2	If the constant θ is an n-ary predicate, Let definition be a sentence of form (α_{1})..(α_{n})(θα_{1}…α_{n} \\(\iff\\) ω), where ω is a formula of T and α_{1}…α_{n} are distinct and are all the variables occurring free in ω.

11.6.4.3	If the constant θ is a sentential letter, Let definition be a sentence θ \\(\iff\\) ω where ω is a sentence of T.

11.6.4.4	If the constant θ is an individual constant, Let definition be a sentence (α)(α = θ \\(\iff\\) ω) where ω is a formula of T and having α as its only free variable, and the corresponding sentence (∃β)(α)(α = β \\(\iff\\) ω) with β a variable distinct from α, is a thesis of T.

11.6.4.5	 If the constant θ is an n-ary operation symbol,, Let definition be a sentence of form (γ_{1})..(γ_{n})(α)(α = θγ_{1}…γ_{n} \\(\iff\\) ω), where α, γ_{1}…α_{n} are distinct and are all the variables occurring free in ω. Θ does not occur in ω, and the corresponding uniqueness condition (γ_{1})..(γ_{n})(∃β)(α)(α = β\\(\iff\\) ω) with β distinct from α, γ_{1}, …, γ_{n} is a thesis of T.

11.6.5	Definability 

11.6.5.1	Definable in the theory T ( a non-logical constant θ) : there is among the theses of T a formally correct definition of θ relative to the theory T – θ

11.6.5.1.1	T-θ : from the non-logical vocabulary of a theory T remove a constant θ, and from the theses of T we remove all those containing θ

11.6.5.2	 Padoa’s principle : Non-logical constant θ is not definable in a theory T If we can give two models of T that differ in what they assign to θ but are otherwise the same.

