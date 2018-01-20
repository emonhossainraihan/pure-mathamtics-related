---

layout: post

title :[Elementary Logic]  Formalized Language L

date : 2018-01-19 13:52:06 +0900

---

3	Formalized Language L

3.1	Grammar of L

3.1.1	Expression of L : finite length strings of symbols

3.1.1.1	Variables : u~z with/w/o subscripts

3.1.1.1.1	Subscript : lower right Arabic numerals

3.1.1.2	Constants

3.1.1.2.1	–, V, (, ), &, \\(\implies\), \\(\iff\\), ∃

3.1.1.2.2	Non-logical constants

3.1.1.2.2.1	Predicates : capital Italic letter

3.1.1.2.2.1.1	N-ary predicate : superscript n

3.1.1.2.2.1.1.1	Superscript : upper right Arabic numerals

3.1.1.2.2.1.2	Sentential letter : no superscript

3.1.1.2.2.2	Individual constants : a ~ t

3.1.1.3	Individual symbol : variable or individual constant

3.1.1.4	Atomic formula : a sentential letter or n-ary predicate with a string of length n of individual symbols

3.1.1.4.1	General : a formula not an atomic formula, begins with a universal / existential quantifier

3.1.1.4.2	Molecular : a formula not an atomic formula, otherwise

3.1.1.5	Formula : atomic formula or built up from one or more atomic formulas by a finite number of applications as :

3.1.1.5.1	If Φ is a formula, then -Φ is a formula

3.1.1.5.1.1	Negation

3.1.1.5.2	If Φ and Ψ are formulas, then (ΦVΨ) , (Φ&Ψ), (Φ\\(\implies\)Ψ), (Φ\\(\iff\\)Ψ) are formulas

3.1.1.5.2.1	Disjunction(ΦVΨ), Conjunction(Φ&Ψ), conditional(Φ\\(\implies\)Ψ) ( antecedent, consequent), biconditional(Φ\\(\iff\\)Ψ)

3.1.1.5.3	If Φ is a formula and (α)Φ and (∃α)Φ are formulas 

3.1.1.5.3.1	Universal Quantifier : (α) 

3.1.1.5.3.2	Existential Quantifier : (∃α)

3.1.1.5.3.3	Universal generalization (α)Φ, Existential generalization (∃α)Φ

3.1.1.6	Occurrence of a variable α in formula Φ

3.1.1.6.1	Bound : within an occurrence in Φ of a formula of the form (α)Ψ or of the form (∃α)Ψ

3.1.1.6.2	Free occurrence 

3.1.1.7	Occurrence of a formula Ψ in formula Φ

3.1.1.7.1	Bound : within an occurrence in Φ of a formula of the form (α)θ or (∃α)θ

3.1.1.7.2	Free occurrence

3.1.1.8	Order of a formula

3.1.1.8.1	Order 1 : Atomic formulas

3.1.1.8.2	Order of Disjunction, Conjunction, conditional, bidirectional is 1 + (Maximum order of two formulas)

3.1.1.8.3	Order n formula Φ \\(\implies\) -Φ, (α)Φ (∃α)Φ is order n+1 where α is variable

3.2	Notational conventions

3.2.1	Outermost parentheses are occasionally omitted

