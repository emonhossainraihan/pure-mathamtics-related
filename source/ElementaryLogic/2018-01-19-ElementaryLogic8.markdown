---

layout: post

title : (Elementary Logic)  Some Metatheorems

date : 2018-01-19 13:52:11 +0900

---

8	Some Metatheorems

8.1	Replacement, negation and duality, prenex normal form

8.1.1	Φ^{α_1, α_2, …,α_n}_{β_1,β_2, …,β_n} : For any formula Φ, result of replacing all free occurrences of distinct variables (α_1, α_2, …,α_n) by occurrences of individual symbols (β_1,β_2, …,β_n) respectively.

8.1.2	String of quantifiers : a quantifier | result of prefixing a quantifier to a shorter string of quantifiers

8.1.2.1	A string of universal quantifiers : a universal quantifier | result of prefixing a universal quantifier to a shorter string of quantifiers

8.1.2.2	A string of existential quantifiers : an existential quantifier | result of prefixing an existential quantifier to a shorter string of quantifiers

8.1.3	Closure of formula Ψ (a formula Φ)  : Φ is sentence and Φ = Ψ or Φ is the result of prefixing a string of universal quantifiers to Ψ

8.1.4	\\(\Vdash\\)Φ : every closure of Φ is a theorem of logic 

8.1.5	( I )If Φ^{α_1, α_2, …,α_n}_{β_1,β_2, …,β_n} is a theorem of logic (where β_1,β_2, …,β_n are distinct individual constants not occurring in Φ) , then\\(\Vdash\\)Φ

8.1.5.1	Pf) UG

8.1.6	( II )If one closure of Φ is a theorem of logic, then \\(\Vdash\\)Φ

8.1.6.1	Pf) US

8.1.7	( III )If \\(\Vdash\\)Φ and \\(\Vdash\\)Φ \\(\implies\) Ψ, then \\(\Vdash\\)Ψ

8.1.7.1	Pf) US

8.1.8	( IV )Generalization

8.1.8.1	\\(\Vdash\\)(α)(α’)Φ \\(\iff\\) (α)(α’)Φ

8.1.8.2	\\(\Vdash\\)(∃α)(∃α’)Φ \\(\iff\\) (∃α)(∃α’)Φ

8.1.8.3	\\(\Vdash\\)(α)(Φ & Ψ) \\(\iff\\) (Φ & (α)Ψ) if α does not occur free in Φ

8.1.8.4	\\(\Vdash\\)(α)(∃α’)(Φ & Ψ) \\(\iff\\) ((α)Φ & (∃α’)Ψ) if α does not occur free in Φ

8.1.9	( V ) If \\(\Vdash\\)Ψ\\(\iff\\)Ψ’, then

8.1.9.1	\\(\Vdash\\)-Ψ\\(\iff\\)-Ψ

8.1.9.2	\\(\Vdash\\)(Ψ & χ) \\(\iff\\) (Ψ’ & χ)

8.1.9.3	\\(\Vdash\\)( χ & Ψ ) \\(\iff\\) ( χ & Ψ’ )

8.1.9.4	\\(\Vdash\\) ( Ψ V χ ) \\(\iff\\) ( Ψ’ V χ )

8.1.9.5	\\(\Vdash\\) ( χ V Ψ ) \\(\iff\\) ( χ V Ψ’ )

8.1.9.6	\\(\Vdash\\) (Ψ \\(\implies\) χ) \\(\iff\\) (Ψ’\\(\implies\)χ)

8.1.9.7	\\(\Vdash\\) (χ \\(\implies\) Ψ) \\(\iff\\) (χ \\(\implies\)Ψ’)

8.1.9.8	\\(\Vdash\\) (Ψ \\(\iff\\) χ) \\(\iff\\) (Ψ’ \\(\iff\\) χ)

8.1.9.9	\\(\Vdash\\) (χ \\(\iff\\) Ψ) \\(\iff\\) ( χ \\(\iff\\) Ψ’)

8.1.9.10	\\(\Vdash\\) (α)Ψ \\(\iff\\) (α)Ψ’

8.1.9.11	\\(\Vdash\\) (∃α)Ψ \\(\iff\\) (∃α)Ψ

8.1.9.11.1	 pf) I, III, IV

8.1.10	 (Replacement)

8.1.10.1	Suppose that Φ’ is like Φ except for containing an occurrence of Ψ’ where Φ contains an occurrence of Ψ, and suppose that \\(\Vdash\\)Ψ\\(\iff\\)Ψ’. Then \\(\Vdash\\)Φ\\(\iff\\)Φ’, and \\(\Vdash\\)Φ iff \\(\Vdash\\)Φ’

8.1.10.1.1	Pf) V, I, III

8.1.11	(Definition of equivalence) : for any formulas Φ and Ψ, Φ is equivalent to Ψ iff \\(\Vdash\\)Φ\\(\iff\\)Ψ

8.1.12	(Rewriting of bound variables) if formulas (α)Φ and (α’)Φ’ are alike except that former has occurrences of α where and only where the latter has occurrences of α’, then they are equivalent. Similarly for (∃α)Φ and (∃α’)Φ’.

8.1.12.1	Pf) I

8.1.13	(Negation theorem) Suppose that a formula Φ contains no occurrences of \\(\implies\) and \\(\iff\\) and that Φ’ is obtained from Φ by exchanging & and v, exchanging universal and the corresponding existential quantifiers, and by repacing atomic formulas by their negations. Then Φ’ is equivalent to -Φ.

8.1.14	(Definition of Prenex normal form) ( a formula Φ ) : Φ is either quantifier-free or consists of a string of quantifiers followed by a quantifier-free formula.

8.1.15	(Prenex normal form) : For any formula Φ there is an equivalent formula Ψ that is in prenex normal form.

8.1.15.1	Pf) reduction to prenex normal form, (Replacement), (Negation theorem), IV

8.1.15.2	If a sentence Φ has a prenex normal form in the prefix of which no existential quantifier precedes any universal quantifier, then the validity of Φ is decidable.

8.1.16	(X) if \\(\Vdash\\)Φ and if Ψ is the result of replacing all atomic formulas in Φ by their negations, then \\(\Vdash\\)Ψ

8.1.17	(Duality) if \\(\Vdash\\)Φ\\(\iff\\)Ψ and neither \\(\implies\) nor \\(\iff\\) occurs in Φ and Ψ, and if Φ* and Ψ* are obtained from Φ and Ψ, respectively, by exchanging & and v, and universal and the corresponding existential quantifiers, then \\(\Vdash\\)Φ*\\(\iff\\)Ψ* ; similarly if \\(\Vdash\\)Φ\\(\iff\\)Ψ, then \\(\Vdash\\)Ψ* \\(\implies\) Φ*

8.1.17.1	Pf) (Replacement), (Negation theorem), (X)

8.2	Soundness and consistency

8.2.1	Sound ( a system of inference rules) : any conclusion derived by their use will be a consequence of the premises from which it is obtained

8.2.1.1	Assertion

8.2.1.1.1	Any sentence appearing on the first line of a derivation is a consequence of the premises of that line

8.2.1.1.2	Any sentence appearing on the latter line is a consequence of its premises if all sentences appearing on earlier lines are consequence of theirs

8.2.1.2	Any sentence appearing on a line of a derivation is a consequence of the premises of that line

8.2.1.3	If a sentence Φ is derivable from a set of sentences Γ, then Φ is a consequence of Γ.

8.2.2	Consistent ( a system of inference rules ) : there is no sentence Φ such that both Φ and -Φ are derivable from (Universal set)

8.2.2.1	Transform T(Φ) (a sentence Φ) : SC sentence which is the result of deleting all individual symbols, quantifiers, and predicate superscripts from Φ

8.3	Completeness

8.3.1	Complete ( a system of inference rules ) : One can derive, from any given set of sentences, any consequence of that set

8.3.1.1	Consistent with respect to derivability ( a set of sentences Γ ) : the sentence ‘P&-P’ is not derivable from Γ ~ d-consistent

8.3.1.1.1	For any sentence Φ and set of sentences Γ, Φ is derivable form Γ iff ΓU{-Φ} is not d-consistent

8.3.1.1.2	For any set of sentences Γ, Γ is d-consistent iff at least one sentence Φ from L is not derivable from Γ

8.3.1.2	Maximal d-consistent (a set of sentences Γ) iff Γ is d-consistent and not properly included in any d-consistent set Δ.

8.3.1.2.1	Φ€Δ iff -Φ !∈ Δ

8.3.1.2.2	Φ∈Δ iff Φ is derivable from Δ

8.3.1.2.3	(Φ v Ψ) ∈ Δ iff Φ ∈ Δ  or Ψ ∈ Δ

8.3.1.2.4	(Φ & Ψ) ∈ Δ iff Φ ∈ Δ and Ψ ∈ Δ

8.3.1.2.5	(Φ \\(\implies\) Ψ) ∈ Δ iff Φ !∈ Δ or Ψ ∈ Δ, or both

8.3.1.2.6	(Φ \\(\iff\\) Ψ) ∈ Δ iff Φ, Ψ ∈ Δ or Φ, Ψ !∈ Δ

8.3.1.3	ω-complete ( a set of sentences Γ ) : for every formula Φ and variable α, if (∃α)Φ belongs to Γ, then there is an individual constant β s.t. Φ α/β also belongs to Γ.

8.3.1.4	Suppose Δ is maximal d-consistent and ω-complete, then

8.3.1.4.1	(α)Φ ∈ Δ iff for every individual constant β, Φ α/β ∈ Δ

8.3.1.4.2	(∃α)Φ ∈ Δ iff for some individual constant β, Φ α/β ∈ Δ

8.3.2	Principle lemma for completeness

8.3.2.1	( I ) for any set of sentences Γ, if Γ is d-consistent, then it is consistent.

8.3.2.1.1	( I’ ) for any set of sentences Γ, if Γ is d-consistent and all indices of individual constants occurring in the sentences of Γ are even, then it is consistent.

8.3.2.1.2	( II ) For any set of sentences Γ, if Γ satisfies the hypothesis of I’, then there is a set of sentences Δ that includes Γ and is maximal d-consistent and ω-complete.

8.3.2.1.2.1	Assume that all the sentences of L can be arranged in an infinite list Φ_1, Φ_2, … Φ_n with following properties.

8.3.2.1.2.1.1	Each sentence of L occurs at least one in the list

8.3.2.1.2.1.2	For each sentence of the form (∃α)Φ, there is at least one I such that Φ_i = (∃α)Φ and Φ_(i+1) = Φ α/β, where β is a ‘new’ individual constant

8.3.2.1.3	( III ) every maximal d-consistent, ω-complete set of sentences is consistent.

8.3.2.1.3.1	Corollary : every maximal d-consistent ,ω-complete set of sentences is satisfiable by an interpretation having a domain equinumerous with the positive integers. ( denumerably infinite domain)

8.3.2.1.4	Corollary of ( I ) : For any set of sentences Γ, if Γ is d-consistent, then it is satisfiable by an interpretation having a denumerably infinite domain.

8.3.2.1.5	(Löwenheim-Skolem theorem) : if Γ is a consistent set of sentences, then Γ is satisfiable by an interpretation having a denumerably infinite domain.

8.4	A proof procedure for valid sentences

8.4.1	If a given sentence is valid, then there exists procedures which generates a proof of that sentence.

8.4.1.1	Given an arbitrary valid sentence Φ, we can reduce Φ to a sentence Ψ in prenex normal form.

8.4.1.2	Procedure ( a valid sentence Φ in prenex normal form ) :

8.4.1.2.1	Enter -Φ on the first line as a premise.

8.4.1.2.2	Derive a prenex normal form Ψ from -Φ.

8.4.1.2.3	Construct a sequence of lines satisfying the following two conditions, until a truth-functional inconsistency appears:

8.4.1.2.3.1	Whenever any universal generalization (α)θ appears on a line, particular instances θ α/β (for all individual constants β occurring in the sequence, and in any case for at least one individual constant β) shall appear on later lines, inferred by US.

8.4.1.2.3.2	Whenever any existential generalization (∃α)θ appears on a line, θ α/β (for some new individual constant β ) shall appear as a premise on a later line.

8.4.1.2.4	When a truth-functional inconsistency appears, derive ‘P&-P’ by rule T, apply ES to transfer dependence to -Φ, conditionate to obtain the theorem -Φ \\(\implies\) (P&-P), and apply T to obtain the theorem Φ.

