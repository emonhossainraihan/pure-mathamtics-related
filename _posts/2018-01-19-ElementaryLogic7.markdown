---

layout: post

title :[Elementary Logic]  Rules of Inference for L

date : 2018-01-19 13:52:10 +0900

---

7	Rules of Inference for L

7.1	Basic rules; derivability

7.1.1	Impossibility of a decision procedure for validity

7.1.2	Impossibility of step-by-step procedure for deciding whether given sentence is a consequence of other sentences

7.1.3	Derivation : finite sequence of consecutively numbered lines with premise-numbers of the line

7.1.3.1	P (Introduction of premises) : Any sentence may be entered on a line with the line number taken as the only premise-number

7.1.3.2	T (Tautological inference) : Any sentence may enter on a line if it is a tautological consequence of a set of sentences that appear on earlier lines; as premise-numbers of the new line take all premise-numbers of those earlier lines

7.1.3.3	C (Conditionalization) : (Φ \\(\implies\)Ψ) may be entered on a line if Ψ appear on earlier lines ; as premise-numbers of the new line take all premise-numbers of those earlier lines. With the exception of any that is the line number of a line on which Φ appears.

7.1.3.4	US (Universal specification) The sentence Φ α/β may enter on a line if (α)Φ appears on an earlier line; as premise-numbers of the new line take all premise-numbers of those earlier lines

7.1.3.5	UG (Universal generalization) The sentence (α)Φ may enter on a line if Φ α/β appears on an earlier line and β occurs neither in Φ nor in any premise of that earlier line; as premise-numbers of the new line take all premise-numbers of those earlier lines

7.1.3.6	E (Existential quantification) The sentence (∃α)Φ may enter on a line if –(α)-Φ appears on an earlier line or vice versa; as premise-numbers of the new line take all premise-numbers of those earlier lines

7.1.4	Derivation of Φ from Γ : a derivation in which a sentence Φ appears on the last line and all premises of that line belong to a set of sentences Γ

7.1.4.1	derivable from the set of sentences Γ ( a sentence Φ ) : there is a derivation of Φ from Γ

7.2	The short-cut rules EG, ES and Q

7.2.1	EG (Existential generalization) : The sentence (∃α)Φ may enter on a line if Φ α/β appears on an earlier line; as premise-numbers of the new line take all premise-numbers of those earlier lines

7.2.2	ES (Existential specification) : Suppose (∃α)Ψ appears on line I of a derivation, that Φ α/β appears as a premise on a later line j, and that Φ appears on a still later line k; and suppose further that the constant β occurs neither in Φ,Ψ, nor in any premise of line k other than Φ α/β ; than may enter on a new line. As premise-numbers of the new line take all those of lines I and k, except the number j.

7.2.3	Q (Quantifier exchange) The sentence –(∃α)Φ may enter on a line if (α)-Φ appears on earlier line, or vice versa; similarly for the pairs {(∃α)-Φ, -(α)Φ },{–(∃α)-Φ ,(α)Φ },{–(∃α)Φ , -(α)-Φ }; as premise-numbers of the new line take all premise-numbers of those earlier lines.

7.3	Theorems of logic

7.3.1	A Theorem of logic (a sentence Φ) : Φ is derivable from the empty set of sentences ~ theorem

7.3.1.1	A sentence Φ is derivable from a set of sentences Γ iff Φ is consequence of Γ

7.3.1.2	Φ is a theorem of logic iff Φ is valid.

