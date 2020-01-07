---

layout: post

title : (Elementary Logic)  Logic Preliminaries

date : 2018-01-19 13:52:05 +0900

---

2	Further preliminaries

2.1	Use and mention

2.1.1	Use : name (identifier)

2.1.2	Mention : use the name for reference (object which identifier indicates)

2.2	Sense and denotation

2.2.1	Sense (an expression) : meaning

2.2.2	Denotation (an expression) : objects which it refers

2.2.3	Condition of sense and denotation

2.2.3.1	The denotation (a complex expression) is a function of the denotations of its parts

2.2.3.2	The sense (a complex expression) is a function of the senses of its parts

2.2.4	Ordinary vs Oblique sense/denotation

2.2.4.1	Oblique denotation = Ordinary sense

2.2.4.2	Direct occurrence (an occurrence of a name or description in a expression) : in the context it has ordinary sense

2.3	Variables : expression of generalization, must specify substituents

2.3.1	Substituents : a set of values which could substitute a variable

2.3.2	Values : names

2.4	Sentence forms 

2.4.1	Replacement of a direct occurrence of a sentence with the expression with same ordinary denotation does not change its truth value

2.4.2	Replacement of an indirect occurrence of a sentence with the expression with same ordinary denotation can change its truth value

2.4.3	Sentence form : it is an expression that is a sentence or is obtainable from a sentence by replacing some or all direct occurrences of names by variables

2.4.4	Quantifier : often asserted in sentence forms

2.4.4.1	Universal quantifier : For every x, ..

2.4.4.2	Existential quantifier : There is an x such that …

2.4.5	Variables

2.4.5.1	Free occurrences : needs additional quantifiers or replacements to obtain a sentence

2.4.5.2	Bound : already has those

2.5	Description forms 

2.5.1	Replacement of a direct occurrence of a description with the expression with same ordinary denotation does not change its truth value

2.6	Set  ~ Class

2.6.1	Elements : objects constituting a set ~ members

2.6.1.1	Sets having same members are identical

2.6.2	Empty set : no members

2.6.3	Universal set : set of all objects satisfying (x is identical with x)

2.6.4	원소나열법 : notation for any finite number of occurrences of variables, names, or descriptions

2.6.5	A subset of B : every element of a set A is also an element of a set B ~ included in

2.6.5.1	 Φ⊂A

2.6.5.2	A⊂A

2.6.5.3	A⊂(Universal set)

2.6.5.4	If A⊂B and B⊂A, then A = B

2.6.5.5	If A⊂B and B⊂C, then A⊂C 

2.6.6	The Union of A and B : a set of all members belonging to A or to B

2.6.7	The Intersection of A and B : a set of all members belonging to A and to B

2.6.8	The Complement of A : a set of all members not belonging to A

2.6.9	Russell’s Antinomy : K = {x | x is not an element of x} K ∈K or K not∈ K ?

2.6.9.1	Give up Assumption that all sets can themselves be members of sets

2.6.10	 Relation : any set of ordered n-tuples of objects is an n-ary relation

2.6.10.1	 Binary Relation : x R y = <x,y> ∈ R

2.6.10.2	 Domain : a set of all objects x s.t. for some y , x R y

2.6.10.3	 Converse domain : a set of all objects y s.t. for some x, x R y

2.6.10.4	 Field (binary relation) : (Domain) U (Converse domain)

2.6.10.5	 Converse (binary relation R) : for all objects x, y , x R y iff y S x

2.6.10.6	 Function (a binary relation R) : for all objects x, y, z , if x R y and x R z , then y = z

2.6.10.7	 1-1 relation (binary relation R) : R and its converse are both function

2.6.10.8	 N-ary operation (n+1-ary relation R) : with respect to set D, for each n-tuple <x1, x2, … , xn> of objects in D there uniquely exists an object y in D s.t. <x1,x2,..,xn,y> ∈ R

2.7	Object-language and Metalanguage

2.7.1	Explain one language by using another, then former is Object-language and latter is Metalanguage (ex. artificial language explained by English)

2.7.2	Metalinguistic variables : variables of the metalanguage, Greek letters

