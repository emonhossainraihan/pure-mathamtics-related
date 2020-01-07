---

layout: post

title : (Elementary Logic)  Axioms for L_{1}

date : 2018-01-19 13:52:13 +0900

---

10	Axioms for L_{1}

10.1	Introduction

10.1.1	Axioms : easily recognizable valid sentences

10.1.2	 (Modus Ponens) : A sentence Φ follows from sentences Ψ and χ by modus ponens iff χ = (Ψ -> Φ)

10.1.3	Definitionally equivalent to a formula Ψ ( a formula Φ ) : formulas χ, θ, Φ_{1}, Φ_{2} s.t. Φ and Ψ are alike except that one contains an occurrence of χ at some place where the other contains an occurrence of θ, and either

10.1.3.1	 Χ = (Φ_{1} v Φ_{2}) and θ = (-Φ_{1} -> Φ_{2}) 

10.1.3.2	 Χ = (Φ_{1} & Φ_{2}) and θ = -(Φ_{1} -> -Φ_{2})

10.1.3.3	 Χ = (Φ_{1} \\(\iff\\) Φ_{2}) and θ = ((Φ_{1}-> Φ_{2}) & (Φ_{2}-> Φ_{1}))

10.1.3.4	 Χ = (∃α)Φ_{1} and θ = -(α)-Φ_{1}

10.1.4	 Proof : a finite sequence of sentences, each of which is an axiom or is definitionally equivalent to an earlier sentence of the sequence or follows from earlier sentences by modus ponens.

10.1.5	 Theorem (a sentence Φ) : Φ is the last line of a proof.

10.1.5.1	\\(\vdash\\) Φ : all closures of Φ are theorems.

10.1.6	 Notation : Φ, Ψ, χ are formulas. α is variables. β γ are individual symbols. P, Q, R, T are expressions.

10.1.7	If Φ and Φ ->Ψ are theorems, then Ψ is a theorem.

10.1.8	If Φ is a sentence, Φ->Φ is a theorem.

10.1.9	If Φ, Ψ, χ are sentences, (Ψ -> χ)-> ((Φ->Ψ) ->(Φ->χ)) is a theorem.

10.1.10	If Φ->Ψ and Ψ->χ are theorems, then Φ->χ is a theorem.

10.1.11	(Mathematical induction) : All the positive integers have some given property P ? 

10.1.11.1	(weak induction) 

10.1.11.1.1	1 has the property P

10.1.11.1.2	For every positive integer k, if k has the property P, then k+1 has the property P

10.1.11.2	(Strong induction)

10.1.11.2.1	For each positive integer k, if all positive integers less than k have the property P, then k has the property P.

10.1.12	Q(Φ->Ψ) ->(QΦ->QΨ) is a theorem, if Q is a string of universal quantifiers containing every variable that occurs free in Φ or Ψ.

10.1.13	If QΦ and Q(Φ->Ψ) are theorems, then QΨ is a theorem, where Q is a string of universal quantifiers.

10.1.14	\\(\vdash\\)(Ψ->χ)->((Φ->Ψ)->(Φ->χ))

10.1.15	If Q(Φ->Ψ) and Q(Ψ->χ) are theorems, then Q(Φ->χ) is a theorem.

10.1.16	\\(\vdash\\)Q(Φ->Ψ) ->(QΦ->QΨ)

10.1.17	\\(\vdash\\)QΦ->Φ

10.1.18	\\(\vdash\\)Φ->QΦ, if no variable in Q occurs free in Φ.

10.1.19	\\(\vdash\\)QΦ->PΦ, if every variable in P is either in Q or does not occur free in Φ.

10.1.20	If Ψ and χ are closures of Φ, then Ψ->χ is a theorem, and χ is a theorem if Ψ is a theorem.

10.1.21	If \\(\vdash\\) Φ and \\(\vdash\\)Φ->Ψ, then \\(\vdash\\)Ψ.

10.1.22	If \\(\vdash\\)Φ and Ψ is definitionally equivalent to Φ, then \\(\vdash\\)Ψ.

10.1.23	If \\(\vdash\\)Φ->Ψ and \\(\vdash\\)Ψ->χ, then \\(\vdash\\)Φ->χ

10.1.24	\\(\vdash\\)Φ iff \\(\vdash\\)QΦ->QΨ

10.1.25	If \\(\vdash\\)Φ->Ψ, then \\(\vdash\\)QΦ->QΨ

10.2	Sentential calculus (lo\\(\Vvdash\\) bo\\(\Vvdash\\) ,full of one-liner theorems)

10.2.1	(Replacement) : If \\(\vdash\\)Φ\\(\iff\\)Ψ and χ is like θ except for having an occurrence of Φ at some place where θ has an occurrence of Ψ, then \\(\vdash\\)χ\\(\iff\\)θ and \\(\vdash\\)χ iff \\(\vdash\\)θ.

10.3	Quantification theory (lo\\(\Vvdash\\) bo\\(\Vvdash\\), full of one-liner theorems)

10.4	Identity, further quantification theory, and substitution

10.4.1	(Substitution) If Φ is a theorem and Ψ is a substitution-instance of Φ, then Ψ is a theorem.

10.4.1.1	Stencil : an expression either a sentence of L_{1} or is obtainable from such a sentence by putting the counters ①, ②, ③, .. where that sentence contains occurrences of individual constants.

10.4.1.2	Substitute σ for θ in Φ ( σ : stencil of degree n, θ : n-ary predicate other than I^{2}_{1}, Φ : a sentence in L_{1} ) : for each occurrence of θδ_{1}δ_{2}..δ_{n} in Φ where δ_{1},δ_{2},..,δ_{n} are individual symbols, put σ(δ_{1},δ_{2},..,δ_{n})

10.4.1.3	Legitimate ( a substitution) : If in this substitution we have at all places obeyed the rule that no variable shall occur bound at any place in any substituted σ(δ_{1},δ_{2},..,δ_{n}) unless it already occurs bound at that place in σ

10.4.1.4	A substitution-instance of a sentence Φ ( a sentence Ψ) : Ψ can be obtained from Φ by a legitimate substitution.

10.5	Proofs from assumptions

10.5.1	Proof of the sentence Φ from the assumptions Γ (a set of sentences Γ) : Φ is the last term of the sequence and each term of the sequence is either an axiom or one of the assumptions Γ or follows from earlier terms by modus ponens or definitional interchange.

10.5.2	 Γ\\(\Vvdash\\)Φ : there is a proof of Φ from the assumptions Γ

10.5.3	(empty set) \\(\Vvdash\\) Φ iff Φ is a theorem

10.5.4	If Φ ∈ Γ, then Γ \\(\Vvdash\\) Φ

10.5.5	If Γ \\(\Vvdash\\) Φ and Γ ⊂ Δ, then Δ \\(\Vvdash\\) Φ

10.5.6	If Γ \\(\Vvdash\\) Φ and Δ \\(\Vvdash\\) Φ -> Ψ, then Γ U Δ \\(\Vvdash\\) Ψ

10.5.7	(Deduction Theorem) Γ U { Φ } \\(\Vvdash\\) Ψ iff Γ \\(\Vvdash\\) Φ -> Ψ

10.5.8	Γ \\(\Vvdash\\) Φ iff Γ U {-Φ} \\(\Vvdash\\) ‘P&-P’

10.5.9	Γ \\(\Vvdash\\) Φ iff for every sentence Ψ, Γ U { - Φ } \\(\Vvdash\\) Ψ

10.5.10	Γ \\(\Vvdash\\) Φ iff Φ is a consequence of Γ.

