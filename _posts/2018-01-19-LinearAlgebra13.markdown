---

layout: post

title :[Linear Algebra] Triangularization

date : 2018-01-19 13:51:14 +0900

---

(Section 13) Triangularization

(subsection 13.1.) Triangularization

(정의) 이 장에서는 모든 것이 유한차원이라고 가정한다.

(관찰 13.1.1.) W \le V , W’ \le V’ 이고, linear map L : V \to V’ 이 LW \le W’ 을 만족한다고 가정할 때, \bar{L} : V/W \to V’/W’ 을 \bar{L}\bar{v} = \bar{Lv} (v \in V) 로 정의하면, \bar{L} 은 well-defined 된 linear map 이다. (이때, 우리는 L이 \bar{L} 을 naturally induce 한다고 말한다.)

(보조정리 13.1.4.) T \in \mathfrak{LM} 이고, W는 V의 T-invariant subspace 라고 하자. \bar{T} : \bar{V} \to \bar{V} 는 (관찰 13.1.1) 과 같다고 하고, \mathfrak{C} = {v_{1}, …, v_{m}} 은 W의 basis, \mathfrak{B} = {v_{1}, …, v_{n}} 은 V의 basis, 그리고 \bar{\mathfrak{B}} = {\bar{v_{m+1}}, …, \bar{v_{n}}} 는 \bar{V} 의 basis 라고 하자. 그러면, [T]_{\mathfrak{B}}^{\mathfrak{B}} = 	$\left( \begin{array}{c|c}	[T|_{W}]_{\mathfrak{C}}^{\mathfrak{C}} & * \\ \hline 0 & [\bar{T}]_{\bar{\mathfrak{B}}}^{\bar{\mathfrak{B}}}\end{array} \right)$

(Triangularization) (정리 13.1.6.) F = \mathbb{C} 이고 T \in \mathfrak{LM} 이면, [T]_{\mathfrak{B}}^{\mathfrak{B}} 가 upper-triangle matrix 인 V의 기저 \mathfrak{B} 가 존재한다.

(subsection 13.2.) Triangularization 의 결과

(따름정리 13.2.1.) T \in \mathfrak{LM} 일 때, T의 characteristic polynomial \phi_{T}(t) = t^{n} + a_{n-1} t^{n-1} + \cdots + a_{1} t + a_{0} (단, a_{1}, …, a_{n-1} \in F) 가 \mathbb{C}-위에서 \phi_{T}(t) = (t-\lambda_{1})(t-\lambda_{2}) \cdots (t-\lambda_{n}), (단, \lambda_{1}, …, \lambda_{n} \in \mathbb{C}) 로 인수분해되면, det(T) = \lambda_{1}\lambda_{2} \cdots \lambda_{n} = (-1)^{n}a_{0} , tr(T) = \lambda_{1} + \lambda_{2} + \cdots + \lambda_{n} = -a_{n-1} 이다.

(따름정리 13.2.2.) N \in \mathfrak{LM} 이 nilpotent 이면, N의 characteristic polynomial 은 \phi_{N}(t) = t^{n} 이다.

(정의 13.2.5.) T \in \mathfrak{LM} 일 때, (T-I) 가 nilpotent 이면 T를 unipotent operator (matrix) 라고 부른다.

(정의 13.2.9.) T,S \in \mathfrak{LM} 일 때, V 의 하나의 기저 \mathfrak{B} 에 관해 [T]_{\mathfrak{B}}^{\mathfrak{B}} 와 [S]_{\mathfrak{B}}^{\mathfrak{B}} 가 모두 upper-triangular matrix 이면, 우리는 T와 S가 simultaneously triangularizable 하다고 말한다. 여러 개 (무한개 포함) 의 경우도 마찬가지로 정의한다.

(명제 13.2.10.) T,S \in \mathfrak{LM} 이고 TS = ST 이면 – 즉 T 와 S 가 commute 하면 – T와 S는 common eigen-vector 를 갖는다. 즉, [Tv = \lambda v, Sv = \mu v for some \lambda , \mu \in \mathbb{C}] 인 non-zero vector v \in V 가 존재한다.

(명제 13.2.11.) T,S \in \mathfrak{LM} 이고, TS = ST 이면, T,S 는 simultaneously triangularizable 하다.

