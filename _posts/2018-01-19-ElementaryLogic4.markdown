---

layout: post

title :[Elementary Logic]  Interpretations and Validity

date : 2018-01-19 13:52:07 +0900

---

4	Interpretations and Validity

4.1	Interpretations of L : Given a sentence Φ in L assign a denotation to each non-logical constant occurring in Φ

4.1.1	Specify Universe of discourse : non-empty domain D

4.1.2	Assign to each individual constant an element of D

4.1.3	Assign to each n-ary predicate an n-ary relation among element of D

4.1.4	Assign to each sentential letter one of truth values T or F

4.2	Truth : Φ is true under I

4.2.1	Let I be any interpretation and Φ be any quantifier-free sentence of L

4.2.1.1	If Φ is sentential letter, then Φ is true under I iff I assigns T to Φ

4.2.1.2	If Φ is atomic and not a sentential , then Φ is true under I iff the objects I assigns to the individual constants of Φ are related by the relation that I assigns to the predicate of Φ

4.2.1.3	If Φ = - Ψ, then Φ is true under I iff Ψ is not true under I

4.2.1.4	If Φ = (Ψ V χ) for sentences Ψ, χ, then Φ is true under I iff Ψ is true under I or χ is true under I or both

4.2.1.5	If Φ = (Ψ & χ) for sentences Ψ, χ, then Φ is true under I iff Ψ is true under I and χ is true under I 

4.2.1.6	If Φ = (Ψ \\(\implies\) χ) for sentences Ψ, χ, then Φ is true under I iff Ψ is not true under I or χ is true under I or both

4.2.1.7	If Φ = (Ψ \\(\iff\\) χ) for sentences Ψ, χ, then Φ is true under I iff either Ψ and χ are both true or both not true under I.

4.2.2	Φ is false under I iff Φ is not true under I

4.2.3	Every quantifier-free sentence is an atomic sentence or is a molecular compound of shorter sentences

4.2.4	Let I and I’ be interpretations of L, and β be an individual constant; the I is β-variant of I’ iff I and I’ are the same or differ only in what they assign to β

4.2.5	Let Φ be any sentence of L, α a variable, and β the first individual constant not occurring in Φ. 

4.2.5.1	If Φ is sentential letter, then Φ is true under I iff I assigns T to Φ

4.2.5.2	If Φ is atomic and not a sentential , then Φ is true under I iff the objects I assigns to the individual constants of Φ are related by the relation that I assigns to the predicate of Φ

4.2.5.3	If Φ = - Ψ, then Φ is true under I iff Ψ is not true under I

4.2.5.4	If Φ = (Ψ V χ) for sentences Ψ, χ, then Φ is true under I iff Ψ is true under I or χ is true under I or both

4.2.5.5	If Φ = (Ψ & χ) for sentences Ψ, χ, then Φ is true under I iff Ψ is true under I and χ is true under I 

4.2.5.6	If Φ = (Ψ \\(\implies\) χ) for sentences Ψ, χ, then Φ is true under I iff Ψ is not true under I or χ is true under I or both

4.2.5.7	If Φ = (Ψ \\(\iff\\) χ) for sentences Ψ, χ, then Φ is true under I iff either Ψ and χ are both true or both not true under I.

4.2.5.8	If Φ = (α)Ψ, then Φ is true under I iff Ψ α/β is true under every β-variant of I

4.2.5.8.1	α/β : replace all free occurrences of α by occurrences of some individual constant β

4.2.5.9	If Φ = (∃α)Ψ, then Φ is true under I iff Ψ α/β is true under at least one β-variant of I

4.2.6	Φ is true/false under I = I assigns the truth-value T/F to Φ

4.2.7	Complete Interpretations : for each element of the domain of I, there is an individual constant to which I assigns that element as denotation

4.2.7.1	Φ is true under all complete interpretations iff Φ is true under all interpretations

4.3	Validity, Consequence, Consistency

4.3.1	Valid (a sentence Φ) : Φ is true under every interpretation

4.3.1.1	Not valid : a nonempty set D and an assignment of appropriate entities to the non-logical constants of L which makes Φ false exists

4.3.2	Consequence of a set of sentences Γ ( a sentence Φ) : there is no interpretation under which all the sentences of Γ are true and Φ is false

4.3.3	Consistent ( a set of sentences Γ ) : there is an interpretation under which all the sentences of Γ are true

4.3.4	Deduction theorem : For any sentence Φ, Φ is a consequence of the sentences Γ together with a sentence Ψ iff (Ψ \\(\implies\) Φ) is a consequence of Γ alone.

