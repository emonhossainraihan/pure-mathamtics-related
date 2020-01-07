---

layout: post

title : (Linear Algebra) Hermitian form

date : 2018-01-19 13:51:16 +0900

---

(Section 15) Hermitian form

(subsection 15.1.) Hermitial form

(정의 15.1.1.) V를 \mathbb{C}-vector space 라고 하자. 이 때, 함수 H : V \times V \to \mathbb{C} 가 , 모든 v,u,w \in V , c \in \mathbb{C} 에 대해, 다음 조건

H(u+v, w) = H(u,w) + H(v,w)

H(cv, w) = cH(v,w) 

H(v,w) = \bar{H(w,v)}

를 만족하면, H를 V의 Hermitian form 이라고 부르고, (V,H) 를 Hermitian space 라고 부른다.

(정의) V가 유한차원 \mathbb{C}-벡터공간일 때, \mathfrak{Ker}(V) = {H : V \times V \to \mathbb{C} | H 는 Hermitian form} 이라고 표기하자.

(정의) (i,j)-성분이 H(v_{i}, v_{j}) 인 (n \times n)-행렬 [H]_{\mathfrak{B}} = (H(v_{i},v_{j})) 를 (기저 \mathfrak{B} 에 관한) H의 행렬이라고 부른다

(정리 15.1.6.) 함수 \Omega_{\mathfrak{B}} : \mathfrak{Ker}(V) \to {J \in \mathfrak{M}_{n,n} (\mathbb{C}) | J 는 self-adjoint} 를 \Omega_{\mathfrak{B}}(H) = [H]_{\mathfrak{B}} (H \in \mathfrak{Ker}(V)) 로 정의하면 \Omega_{\mathfrak{B}} 는 bijection 이다.

(명제 15.1.11.) J = [H]_{\mathfrak{B}} 로 표기하면(따라서, J 는 self-adjoint) {[L]_{\mathfrak{B}}^{\mathfrak{B}} \in GL_{n}(\mathbb{C}) | L \in U(V,H) } = {A \in GL_{n}(\mathbb{C}) | ^{t}A \cdot J \cdot \bar{A} = J} 이다.

(정의 15.1.12.) J \in \mathfrak{M}_{n,n}(\mathbb{C}) 가 self-adjoint 일 때, U_{n}^{J}(\mathbb{C}) = {A \in GL_{n}(\mathbb{C}) | ^{t}A \cdot J \cdot \bar{A} = J} 로 표기하고, J 에 대응하는 unitary group 이라고 부른다.

(subsection 15.2.) Non-degenerate Hermitian form

(정의 15.2.1.) v,w \in V 일 때, H(v,w) = 0 이면, v \perp w 로 표기하고 v 와 w는 서로 수직이라고 말한다. 그리고, S,T \subseteq V 일 때, [H(v,w) = 0 for all v \in S, w \in T] 이면, S \perp T 로 표기하고 S와 T는 서로 수직이라고 말한다. 또, S^{\perp} = {v \in V | v \perp w for all w \in S} 로 표기한다.

(정의 15.2.2.) [H]_{\mathfrak{B}} 가 대각행렬이면, \mathfrak{B} 를 V의 orthogonal basis 라고 부른다. 또, [H]_{\mathfrak{B}} = I 이면, \mathfrak{B} 를 V의 orthonormal basis 라고 부른다.

(정의 15.2.4.) V^{\perp} = 0 일 때, 우리는 H를 non-degenerate Hermitian form 이라고 부른다.

(명제 15.2.5.) H가 non-degenerate 이기 위한 필요충분조건은 det([H]_{\mathfrak{B}}) \neq 0 인 것이다.

(정리 15.2.6.) H가 non-degenerate 일 때, W \le V 이면 dim W^{\perp} = dim V – dim W 가 성립한다.

(관찰 15.2.7.) [H(v,v) = 0 for all v \in V] 이면, H = 0 이다.

(정리 15.2.9.) 모든 non-zero Hermitian space (V,H) 는 orthogonal basis 를 갖는다.

(subsection 15.3.) H-Identification 과 Adjoint operator

(정의) 함수 \phi^{V} = \phi_{H}^{V} : V \to V^{*} 를 (\phi^{V} (v)) (w) = H(w,v) (v,w \in V ) 로 정의하자.

(정리 15.3.3.) 함수 \phi^{V} = \phi_{H}^{V} : V \to V^{*} 에 대해 H가 non-degenerate Hermitian form 이면, \phi^{V} 는 bijection이다. 특별히, V^{*} 의 모든 원소는 \phi^{V}(v) 의 꼴로 쓸 수 있다. (단, v \in V)

(관찰 15.3.4.) W \le V 이면, dim W = dim \phi_{H}^{V}(W) 이다.

(표기법 15.3.5.) (정리 15.3.3.) 의 bijection \phi_{H}^{V} 는 기저의 선택과 무관한 natural bijection 이다. 따라서, B-identification 과 유사하게 \phi_{H}^{V} 를 통하여 V 와 V^{*} 를 identify 하고, V = V^{*} 로 표기법을 쓴다. 이를 우리는 H-identification 이라고 부른다. 그리고 혼동의 가능성이 없다면 \phi_{H}^{V}(v) = \phi_{v} (v \in V) 라고 쓰기도 한다.

(정리 15.3.9.) W \le V 라고 하자. 그러면, H-identification 의 관점에서는 W^{\perp} = W^{perp} 이다. 특별히, dim W^{\perp} = dim V – dim W 이다.

(정의 15.3.10.) L \in \mathfrak{L}(V,W) 이라고 하자. 이 때, L의 (H와 K에 관한) adjoint map L^{\star} \in \mathfrak{L}(W,V) 는 – H-identification 과 K-identification 의 관점에서 – L^{\star} = L^{*} 로 정의된다. 즉, L^{\star} : W \to V 는 다음 사각형 diagram

\begin{tikzpicture} \matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] { W & V\\ W^{*} \times V^{*} & F \\}; \path[-stealth] (m-1-1) edge node [left] {$ \phi_{K}^{W} $} node [right] {$=$} (m-2-1)  edge node [above] {$L^{\star}$} (m-1-2) (m-1-2) edge node [right] {$ \phi_{H}^{V} $} node [left] {$=$} (m-2-2) (m-2-1) edge node [below] {$L^{*}$} (m-2-2);\end{tikzpicture}

 을 commutative diagram 으로 만들어주는 유일한 linear map이다. 이를 식으로 표현한다면, L^{*} = (\phi_{H}^{V})^{-1} \bullet L^{*} \bullet \phi_{K}^{W} 가 된다.

(명제 15.3.12.) L \in \mathfrak{L}(V,W) 이면, L^{*} 는 다음 조건 K(Lv, w) = H(v, L^{*}w), (v \in V , w \in W) 를 만족하는 유일한 linear map 이다. (이 조건은 K(w,Lv) = H(L^{*}w, v) (v \in V, w \in W) 와 동치이다.)

(명제 15.3.13.) L \in \mathfrak{L}(V,W) 일 때, J_{\mathfrak{B}} = [H]_{\mathfrak{B}} , J_{\mathfrak{C}} = [K]_{\mathfrak{C}} 로 표기하면, [L^{*}]_{\mathfrak{B}}^{\mathfrak{C}} = \bar{J_{\mathfrak{B}}}^{-1} \cdot ([L]_{\mathfrak{B}}^{\mathfrak{C}})^{*} \cdot \bar{J_{\mathfrak{C}} 이다.

특별히, L \in \mathfrak{L}(V,V) 일 때, J = [B]_{\mathfrak{B}}로 표기하면, [L^{*}]_{\mathfrak{B}}^{\mathfrak{B}} = \bar{J}^{-1} \cdot ([L]_{\mathfrak{B}}^{\mathfrak{B}})^{*} \cdot \bar{J}

(명제 15.3.14.) U(V,H) = { L \in GL(V) | L^{*} \bullet L = I} 

(관찰 15.3.16.) L,M \in \mathfrak{L}(V,W) 이고 c \in \mathbb{C} 이면, 다음이 성립한다.

(L + M)^{*} = L^{*} + M^{*}.

(cL)^{*} = \bar{c} \cdot L^{*}.

(subsection 15.4.) 왜 Non-degenerate 인 경우만?

(관찰 15.4.1.) L \in U(V,H) 이면, V^{\perp} 는 V의 L-invariant subspace 이다. 다시 말해, L(V^{\perp}) = V^{\perp} 이고, 따라서 L|_{V^{\perp}} \in GL(V^{\perp}) 이다.

(관찰 15.4.2.) \bar{H} 는 well-defined 된 \bar{V} 의 Hermitian form 이다.

(관찰 15.4.3.) \bar{H} 는 non-degenerate 이고, [\bar{H}]_{\bar{\mathfrak{B}} = [H|_{W \times W} ]_{\mathfrak{D}} 이다.

(명제 15.4.5.) 함수 \Lambda : U(V,H) \to GL(V^{\perp}) \times \mathfrak{M}_{m,n-m}(\mathbb{C}) \times U(\bar{V}, \bar{H}) 를 \Lambda(L) = (L|_{V^{\perp}} , [L]_{\mathfrak{C}}^{\mathfrak{D}} , \bar{L}) , (L \in U(V,H)) 로 정의하면, \Lambda 는 bijection 이다.

