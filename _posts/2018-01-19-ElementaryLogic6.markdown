---

layout: post

title :[Elementary Logic]  Tautologous Sentences

date : 2018-01-19 13:52:09 +0900

---

6	Tautologous Sentences

6.1	Definition of tautology

6.1.1	No atomic sentence is tautologous

6.1.2	Normal assignment

6.1.2.1	An assignment A of the truth values T and F to all the sentences of L is called normal iff for each sentence Φ of L,

6.1.2.1.1	A assigns exactly one of the truth values T/F to Φ

6.1.2.1.2	If Φ = -Ψ, then A assigns T to Φ iff A do not assign T to Ψ

6.1.2.1.3	If Φ = ( Ψ V χ ) for sentences Ψ,χ then A assigns T to Φ iff A assigns T to Ψ or T to χ or both

6.1.2.1.4	If Φ = ( Ψ & χ ) for sentences Ψ,χ then A assigns T to Φ iff A assigns T to Ψ and T to χ 

6.1.2.1.5	If Φ = ( Ψ \\(\implies\) χ ) for sentences Ψ,χ then A assigns T to Φ iff A assigns F to Ψ or T to χ or both

6.1.2.1.6	If Φ = ( Ψ \\(\iff\\) χ ) for sentences Ψ,χ then A assigns T to Φ iff A assigns T to both Ψ and χ or assigns F to both

6.1.3	A sentence Φ is tautologous (is a tautology) iff it is assigned the truth value T by every normal assignment of truth values T and F to the sentences of L

6.1.3.1	Every tautologous sentence is valid

6.1.4	A sentence Φ is a tautological consequence of a set of sentences Γ iff Φ is assigned the truth value T by every normal assignment that assigns the truth value T to all sentences of Γ.

6.1.4.1	A sentence Φ is a tautological consequence of a set of sentences Γ iff

6.1.4.1.1	Γ is empty and Φ is tautologous or

6.1.4.1.2	There are sentences Ψ_1, Ψ_2, … ,Ψ_n which belongs to Γ and are such that ((…(Ψ_1 & Ψ_2)& … & Ψ_n) \\(\implies\) Φ) is tautologous.

6.1.5	A set of sentences Γ is truth-functionally consistent iff there is at least one normal assignment that assigns the truth value T to all members of Γ

6.1.5.1	Truth-functionally inconsistent

6.2	Tautologous SC sentences; truth tables

6.2.1	For any sentence Φ, if Φ does not contain any quantifiers, then Φ is tautologous iff Φ is valid.

6.2.1.1	For any SC sentence Φ, Φ is tautologous iff Φ is valid.

6.2.1.2	For any sentence Φ, Φ is tautologous iff there is a tautologous SC sentence Ψ s.t. Φ is substitution instance of Ψ.

6.2.1.2.1	Substitution instance of SC sentence Ψ ( sentence Φ) : result of replacing sentential letters of Ψ by sentences.

6.2.2	Truth table method

6.2.2.1	A Truth value normal assignment gives to an SC sentence is determined by  truth values it gives to occurring sentential letters 

6.2.2.2	Suppose an SC sentence Φ containing n distinct sentential letters, there are 2^n different ways truth values T and F can be assigned to these n letters.

6.3	Deciding whether sentences are tautologous

6.3.1	Basic truth-functional component of a sentence Ψ( a sentence Φ) : Φ is atomic or general and occurs free in Ψ at least once.

6.3.2	Associated with a sentence Ψ (a SC sentence Φ) : Φ is obtained from Ψ by putting occurrences of sentential letters for all free occurrences in Ψ of its basic truth-functional components

6.3.3	For any sentences Φ, Ψ , if Ψ is an SC sentence associated with Φ, then Φ is tautologous iff Ψ is tautologous.

6.3.3.1	Construct an SC sentence Ψ associated with Φ.

6.3.3.2	By a truth-table, test Ψ for tautologousness.

6.3.3.3	Decide whether Φ is tautologous.

6.4	Rules of derivation for SC sentences

6.4.1	SC derivation : finite sequence of consecutively numbered lines, each consisting of an SC sentence together with list of numbers. ~ proof

6.4.1.1	P (Introduction of premises) Any SC sentence may be entered on a line with the line number taken as the only premise-number

6.4.1.2	MP (Modus Ponens) Ψ may be entered on a line if Φ and (Φ \\(\implies\) Ψ) appear on earlier lines; as premise-numbers of the new line take all premise-numbers of those earlier lines.

6.4.1.3	MT (Modus Tollens) Φ may be entered on a line if Ψ and (-Φ \\(\implies\) -Ψ) appear on earlier lines ; as premise-numbers of the new line take all premise-numbers of those earlier lines.

6.4.1.4	C (Conditionalization) (Φ \\(\implies\)Ψ) may be entered on a line if Ψ appear on earlier lines ; as premise-numbers of the new line take all premise-numbers of those earlier lines. With the exception of any that is the line number of a line on which Φ appears.

6.4.1.5	D (Definitional interchange) if Ψ is obtained from Φ by replacing an occurrence of a sentence χ in Φ by an occurrence of a sentence to which χ is definitionally equivalent, then Ψ may be entered on a line if Φ appears on an earlier line; as premise-numbers of the new line take all premise-numbers of those earlier lines

6.4.1.5.1	(Φ V Ψ) is definitionally equivalent to (-Φ\\(\implies\)-Ψ) 

6.4.1.5.2	(Φ & Ψ) is definitionally equivalent to -(Φ\\(\implies\)-Ψ) 

6.4.1.5.3	(Φ \\(\iff\\) Ψ) is definitionally equivalent to ((Φ\\(\implies\)Ψ)&(Ψ\\(\implies\)Φ)) 

6.4.2	SC derivation of Φ from Γ : an SC sentence Φ appears on the last line and premises belongs to a set of SC sentences Γ

6.4.2.1	SC derivable from a set of SC sentences of Γ (an SC sentence Φ) : exists SC derivation of Φ from Γ

6.4.2.2	SC Theorem ( an SC sentence Φ) : Φ is SC derivable from (empty set of sentences)

6.4.3	Any SC sentence that is a substitution instance of a previously proved SC theorem may enter on a line of proof with the empty set of premise-numbers.

6.4.3.1	Ψ may enter on a line if Φ_1, Φ_2, ..,Φ_n appear on earlier line and the conditional (Φ_1 \\(\implies\) (Φ_2 \\(\implies\) … \\(\implies\) (Φ_n \\(\implies\) Ψ)..)) is a substitution instance of already proved SC theorem.

