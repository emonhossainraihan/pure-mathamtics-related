---

layout: post

title :[Linear Algebra] Topology Introduction

date : 2018-01-19 13:51:18 +0900

---

(Section 17) Topology 맛보기

(정의 17.1.8.) X \subseteq \mathbb{R}^{r} , Y \subseteq \mathbb{R}^{s} 일 때, 함수 f : X \to Y 가 다음 조건

f 는 bijection.

f 는 continuous 이고, 그의 역함수 f^{-1} 도 continuous. 

를 만족하면 ,f 를 같은 생김새 함수라고 부르기로 한다. 이 때 X와 Y는 서로 같은 생김새라고 말한다.

(관찰 17.1.17)H 가 matrix group G \le GL_{n}(F) 의 subgroup 일 때, g \in G 이면, H 와 left coset g는 같은 생김새이다.

(정의 17.1.18) ([F,F’= \mathbb{R} or \mathbb{C}] 로 놓자. 즉, F \new F’ 일 수도 있다는 뜻.) G \le GL_{n}(F) \subset \mathbb{R}^{N} , H \le GL_{m}(F’) \subset \mathbb{R}^{M} 이 matrix group 일 때, 함수 \phi : G \to H 가 다음 조건 

\phi 는 group isomorphism.

\phi 는 같은 생김새 함수.

를 만족하면, \phi 를 matrix group isomorphism 이라고 부르기로 한다. 이 때, G와 H는 서로 matrix group 으로서 isomorphic 하다고 말하고, \begin{tikzpicture}\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] {G &H \\}; \path[-stealth] (m-1-1) edge node [above] {$\approx$} node [below]{$matrix gp$} (m-1-2);\end{tikzpicture} 으로 표기하자.

(관찰 17.1.21.) H가 matrix group G \le GL_{n}(F) 의 subgroup 일 때, g \in G 이면 , \begin{tikzpicture}\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] {H &gHg^{-1} \\}; \path[-stealth] (m-1-1) edge node [above] {$\approx$} node [below]{$matrix gp$} (m-1-2);\end{tikzpicture}  이다.

(subsection 17.2.) Compactness 와 Connectedness

(명제 17.2.1.) X \subseteq \mathbb{R}^{N}, Y \subseteq \mathbb{R}^{M} 이고 f : X \to Y가 연속함수이면, 다음이 성립한다.

X가 compact 이면, f(X) 도 compact.

X 가 connected 이면, f(X) 도 connected.

(명제 17.2.9.) X_{i} \subseteq \mathbb{R}^{N_{i}} 일 때, X_{1} \times \cdot \times X_{r} 을 \mathbb{R}^{N_{1} + \cdot + N_{r}} 의 subset으로 생각하자.

모든 X_{i} 가 compact 이면 X_{1} \times \cdot \times X_{r} 도 compact.

모든 X_{i} 가 connected이면 X_{1} \times \cdot \times X_{r} 도 connected.

(정의 17.2.10) \mathbb{R}^{N} 의 subset T가 S^{1} \times \cdots \times S^{1} 과 같은 생김새이면, T를 torus 라고 부른다. Torus 는 compact connected group 이다.

(Spectral Theorem 의 따름정리) (따름정리 17.2.12.) U(n) 과 SU(n), 그리고 SO(n) 은 connected group 이다.

(관찰 17.2.13.) SO(n) 은 O(n) 의 connected component 이다.

O(n) 의 coset decomposition O(n) = SO(n) \mathfrak{U} (O(n) – SO(n)) 은 동시에 O(n) 의 [connected component decomposition] 이다.

(관찰 17.2.14.) SO^{\bullet}(1,1) 은 O(1,1) 의 connected component 이다.

[coset decomposition of O(1,1) modulo SO^{\bullet} (1,1)] 은 동시에 O(1,1) 의 [connected component decomposition] 이다.

