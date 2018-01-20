---

layout: post

title :[Elementary Logic]  Identity and Terms

date : 2018-01-19 13:52:12 +0900

---

9	Identity and Terms

9.1	Identity; the language L_{1}

9.1.1	Leibniz’s Law : if two things are identical, then whatever is true of the one is true of the other.

9.1.2	I^{2}_{1} : a logical constant that stands for the relation of identity in the domain of the relevant interpretation

9.1.3	L_{1} : first order predicate calculus with identity

9.1.3.1	Interpretation for the language L_{1} : nonempty domain D together with an assignment that associates with each individual constant of L_{1} an element of D, with each n-ary predicate other than I^{2}_{1} an n-ary relation among elements of D, with the predicate I^{2}_{1} the identity relation among elements of D, and with each sentential letter of L_{1} one of truth values T or F.

9.1.3.1.1	Every Interpretation of L_{1} is an interpretation of L, but not for converse.

9.1.3.2	Derivation in L_{1} : finite sequence of consecutively numbered lines each consisting of a sentence of L_{1} together with a set of premise-numbers.

9.1.3.2.1	Rules : P,T,C,US,UG,E and..

9.1.3.2.2	The sentence β = β may be entered on a line, with the empty set of premise-numbers

9.1.3.2.3	If a sentence Φ is like a sentence Ψ except that β and γ have been exchanged at one or more places, then Φ may be entered on a line if Ψ and β = γ appear on earlier lines; as premise-numbers of the new line take those of the earlier lines.

9.1.3.3	Derivation of Φ from Γ : a sentence Φ appears on the last line and all premises of that line belong to a set of sentences Γ

9.1.3.4	Derivable from a set of sentences Γ (a sentence Φ) : there is a derivation of Φ from Γ.

9.1.3.5	Φ is derivable from Γ iff Φ is a consequence of Γ.

9.1.3.6	Class : Division of all the individual constants of L_{1} s.t. constants α, β are assigned to the same class iff the sentence α = β is in Δ.

9.1.3.6.1	[(metalinguistic variable)] = the class to which (metalinguistic variable) belongs

9.1.3.7	8.( III ) 

9.1.3.8	Completeness of the predicate calculus with identity

9.1.3.9	(Löwenheim-Skolem theorem of L_{1}) : if Γ is a consistent set of sets of L_{1}, then Γ is satisfiable by an interpretation having a finite or denumerably infinite domain.

9.1.3.10	 A theorem of Logic (a sentence Φ) : Φ is derivable from the empty set of sentences.

9.2	Parenthetical remark

9.2.1	Frege’s solution about identity : The truth of an identity sentence requires only that the two terms have same denotation

9.2.2	Objectionable feature

9.2.2.1	The identity relation among the element of one domain will be different from that among the elements of another

9.2.2.2	Identity relation cannot be a member of themselves.

9.3	Terms ; the Language L’

9.3.1	Operation symbol : new kind of symbol ~ functor, function sign

9.3.2	L’ : first order predicate calculus with identity and operation symbols

9.3.2.1	Result of adding operation symbols to L_{1}.

9.3.2.2	Symbol classification

9.3.2.2.1	Variables

9.3.2.2.2	Constants

9.3.2.2.2.1	Logical constants U { I^{2}_{1} }

9.3.2.2.2.2	Non-logical constants

9.3.2.2.2.2.1	Predicates – { I^{2}_{1} }

9.3.2.2.2.2.2	Operation symbols : lower-case italic letters ‘a’ through ‘t’ with or without numerical subscripts and superscripts

9.3.2.2.2.2.2.1	Individual constant : operation symbol without superscript

9.3.2.2.2.2.2.2	N-ary operation symbol : operation symbol having as superscript a numeral for the positive integer n.

9.3.2.3	N-ary predicate, sentential letter, individual symbol, formula ,sentence, bound/free occurrences are equally defined

9.3.2.4	Term : individual symbol or built up from individual and operation symbol by a finite number of following rules

9.3.2.4.1	If τ_{1}, τ_{2}, …, τ_{n} are terms and θ is an operation symbol of degree n, then θτ_{1}τ_{2}…τ_{n} is a term.

9.3.2.5	Atomic formula : expression either a sentential letter or the form πτ_{1}τ_{2}…τ_{n}, where π is n-ary predicate and τ_{1},τ_{2},…,τ_{n} are terms.

9.3.3	Interpretation of L’ : non-empty domain D together with an assignment that associates

9.3.3.1	Each individual constant of L’ an element of D

9.3.3.2	Each n-ary operation symbol an n-ary operation with respect to D

9.3.3.3	Each sentential letter of L’ one of truth values T or F

9.3.3.4	Each n-ary predicate an n-ary relation among elements of D

9.3.3.5	The binary predicate I^{2}_{1} the identity relation among elements of D

9.3.4	the value under an interpretation (a constant term τ) 

9.3.4.1	if τ is an individual constant, the value of τ under I is the element of D which I assign to τ

9.3.4.2	if τ = θτ_{1}τ_{2}…τ_{n}, where τ_{1}, τ_{2}, …, τ_{n} are terms and θ is an operation symbol of degree n, then the value of the function I (θ)

9.3.5	To define ‘True under I’ we need only one change the definition given for L and L_{1}

9.3.5.1	If Φ is atomic and not a sentential letter, the Φ is true under I iff the values under I of the (constant) terms of Φ are related by the relation that I assigns to the predicate of Φ.

9.3.6	Notion valid, consequence, consistet, normal assignment, tautologous, tautological consequence, truth-functionally consistent, Derivation, derivation of Φ from Γ, derivable are all same.

9.3.7	Amended US, I from inference rules. It is complete.

