---

layout: post

title : Quotient

date : 2018-01-19 13:51:13 +0900

---

(Section 12) Quotient

(subsection 12.1) Equivalence class 와 Partition

(정의 12.1.1.) 집합 X가 있을 때, X \times X 의 subset R이 다음 조건을 만족하면, R 을 X-위의 equivalence relation 이라고 부른다. 또, (x,y) \in R 이면, x~_{R} y, 혹은 간단히 x ~ y 로 표기한다.

(x,x) \in R for all x \in X. (Reflexivity)

(x,y) \in R 이면, (y,x) \in R (Symmetry)

(x,y) \in R 이고 (y,z) \in R 이면 (x,z) \in R. (Transitivity)

(정의 12.1.2) ~ 이 집합 X-위의 equivalence relation 이고 x \in X 일 때, [x] = { y \in X | x ~ y} 로 표기하고, [x] 를 x의 (x를 대표로 갖는) equivalence class 라고 부른다. 또, X/~ = {[x] | x \in X} 로 표기하고, X/~ 를 the set of equivalence classes in X 라고 부른다.

(정의 12.1.5.) ~ 이 집합 X-위의 equivalence relation 일 때, X 의 subset \mathcal{C} 가 다음 조건을 만족하면, \mathcal{C} 를 a complete set of representatives 라고 부른다.

z \in X 이면, z ~ x for some x \in \mathcal{C}.

x,y \in \mathcal{C} 이면, x \nsim y.

이 때 X = \mathfrak{U}_{x \in \mathcal{C}} [x] 이다. 이를 equivalence class decomposition 이라고 부른다.

(정의 12.1.6.) X가 집합이고 A가 index set 일 때, X의 non-empty subset 들 {X_{\alpha} | \alpha \in A} 가 다음 조건

\bigcul_{\alpha \in A} X_{\alpha} = X.

X_{\alpha} \cap X_{\beta} = \empty if \alpha \neq \beta.

을 만족하면, {X_{\alpha} | \alpha \in A} 를 X-의 partition 이라고 부른다. 그리고, 각각의 X_{\alpha} 를 part 라고 부른다.

(관찰 12.1.7.) 집합 X위에 equivalence relation 이 주어졌다는 말과 partition 이 주어졌다는 말은 같은 말이다.

(표기법 12.1.12) H \le G 이고 g \in G 일 때, 다음 표기법 g^{-1} H g = {g^{-1} hg | h \in H} , gHg^{-1} = {ghg^{-1} | h \in H} 를 사용한다.

(subsection 12.2.) Coset

(정의 12.2.1.) H \le G 이고 x \in G 일 때, xH = {xh | h \in H} 로 표기하고 (G의 연산이, 예를들어 덧셈일 때에는 x + H 로 표기) xH 를 [x를 대표로 갖는 left coset modulo H] 라고 부른다. 마찬가지로, Hx = {hx | h \in H} 로 표기하고, Hx 를 [x를 대표로 갖는 right coset modulo H] 라고 부른다.

(관찰 12.2.2.) H \le G 이고 x,y \in G 일 때, 

x \in xH 이고, 따라서 G = \bigcup_{x \in G} xH.

xH = yH iff y^{-1}x \in H.

xH \cap yH = \empty if xH \neq yH.

(표기법 12.2.4.) H \le G 이고 x,y \in G 일 때, 다음 표기법 x \equiv y (mod H) \iff xH = yH \iff x ~_{H} y 와 \bar{x} = [x] = xH 를 사용한다. coset들 전체의 집합 – 즉 equivalence class 전체의 집합- 을 G/H = \frac{G}{H} = {xH | x \in G} = G/~_{H} 로 표기하고, G/H 를 [coset space of G modulo H] 라고 부른다. 따라서 {x_{i} | i \in I} 를 a complete set of representatives 라고 하면, G/H = {\bar{x_{i}} | i \in I} 가 된다. 이 때, 서로 다른 coset 들 전체의 집합은 G의 partition 이므로, G = \mathfrak{U}_{i \in I} x_{i}H 로 쓸 수 있고, 이를 [coset decomposition of G modulo H] 라고 부른다. 

(관찰 12.2.11.) H \le G 이고 x,y \in G 이면, |xH| = |yH| = |H| 이다.

(Lagrange’s Theorem) (관찰 12.2.12) G가 finite group 이고 H \le G 이면, |H| 는 |G| 의 약수이고, |G/H| = \frac{|G|}{|H|} 이다.

(표기법 12.2.13.) H \le G 일 때, |G/H| < \infty 이면, [G : H] = |G/H| 로 표기하고, [G:H] 를 [index of H in G]라고 부른다.

(관찰 12.2.16.) G가 finite group 일 떄 x \in G 이면, |x| \mid |G| 이다. 즉 x의 order 는 G의 order 를 나눈다.

(명제 12.2.17.) p가 prime 이고 |G| = p 이면, G 는 cyclic 이다. 즉, G \approx \mu_{p} 이다.

(Cauchy’s Theorem) (정리 12.2.22) p 가 prime 이고 p \mid |G| 이면, |x| = p 인 x \in G 가 존재한다.

(subsection 12.3.) Normal Subgroup 과 Quotient Group

(정의 12.3.2.) H \le G 일 때, 다음 조건 g^{-1}hg \in G (for all g \in G, h \in H) 를 만족하면, H 를 G의 normal subgroup 이라고 부르고, H \trianglelefteq G 로 표기한다.

(관찰 12.3.3.) H \le G 일 때, coset space G/H 의 binary operation \bar{x} \cdot \bar{y} = \bar{xy} (x,y \in G) 가 well-defined 되어있을 필요충분조건은 H \trianglelefteq G 로 표기한다.

(명제 12.3.4.) N \trianglelefteq G 일 때, coset space G/N 의 binary operation 을 bar{x} \cdot \bar{y} = \bar{xy} (x,y \in G) 라 정의하면, G/N 은 group 이 된다. 우리는 G/N 을 [quotient group of G modulo N] 이라고 부른다.

(관찰 12.3.6.) H \le G 일 때, 다음 조건은 동치이다.

H \trianglelefteq G.

g^{-1}Hg \le H for all g \in G.

g^{-1}Hg = H for all g \in G.

(관찰 12.3.10.) H \le G 이고 [G:H] = 2이면, H 는 G의 normal subgroup 이다.

(관찰 12.3.11.) \phi : G \to G’ 이 group homomorphism 이면, ker \phi \trianglelefteq G (그러나, 반드시 im \phi \trianglelefteq G’일 필요는 없다.

(정의 12.3.12.) N \trianglelefteq G 일 때, \pi : G \to G/N 을 \pi(x) = \bar{x} (x \in G) 라고 정의하고, \pi 를 natural projection 이라고 부른다.

(관찰 12.3.14.) Cyclic group 의 quotient group 은 cyclic 이다.

(표기법 12.3.16.) 0 < n \in \mathbb{Z} 일 때, \mathbb{Z}_{n} = \mathbb{Z}/n\mathbb{Z} 로 표기한다. 이 때, 연산은 \bar{a} + \bar{b} = \bar{a+b} 로 표기한다. (단, a,b \in \mathbb{Z}).

(관찰 12.3.17.) \mathbb{Z}_{n} 은 cyclic group 이다. 따라서 \mathbb{Z}_{n} \approx \mu_{n} 이다.

(정의 12.3.20.) G가 group 일 때, Z(G) = { z \in G | zg = gz for all g \in G} 로 표기하고, Z(G) 를 G의 center 라고 부른다.

(정의 12.3.24.) Projective general linear group PGL_{n}(F) 와 projective special linear group PSL_{n}(F) 를 각각 PGL_{n}(F) = GL_{n}(F) / Z(GL_{n}(F)) , PSL_{n}(F) = SL_{n}(F) / Z(SL_{n}(F)) 로 정의한다. PSO, PSU 등도 유사하게 정의할 수 있다.

(subsection 12.4.) Quotient space

(명제 12.4.1.) W \le V 일 때, coset space V/W 의 연산을 \bar{u} + \bar{v} = \bar{u+v} , c\bar{v} = \bar{cv} (u,v \in V, c \in F) 로 정의하면, V /W 는 vector space 가 된다. 우리는 V/W 를 [quotient space of V modulo W] 라고 부른다.

(정리 12.4.6.) V 가 f.d.v.s.이면 dim(V/W) = dim V = dim W 이다.

(subsection 12.5.) Isomorphism Theorem

(관차 12.5.1.) \phi : G \to H 가 group homomorphism 일 때, \phi (g) = h \in im \phi 이면, \phi^{-1}(h) = g \cdot ker \phi = \bar{g} 이다. (여기에서, (g \cdot ker \phi) 는 [G/ker \phi 의 coset] 을 뜻한다.)

(Group 의 First Isomorphism Theorem) (정리 12.5.2.) \phi : G \to H 가 group homomorphism 일 때, 함수 \bar{\phi} : G / ker \phi \to \im \phi 를 \bar{\phi} (\bar{g}) = \phi(g) , (g \in G) 로 정의하면, \bar{\phi} 는 well-defined 된 group isomorphism 이다. 즉, \begin{tikzpicture}\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] {G/ker \phi &im \phi \\}; \path[-stealth] (m-1-1) edge node [above] {$\bar{\phi}$} node [below]{$\approx$} (m-1-2);\end{tikzpicture} 이다.

(벡터공간의 First Isomorphism Theorem) (정리 12.5.11.) L : V \to W 가 linear map 일 때, 함수 \bar{L} : V/ker L \to im L 을 \bar{L} (\bar{v}) = L(v) (v \in V) 로 정의하면, \bar{L} 은 well-defined 된 vector space isomorphism 이다. 즉, \begin{tikzpicture}\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] {V/ker L &im L \\}; \path[-stealth] (m-1-1) edge node [above] {$\bar{\phi}$} node [below]{$\approx$} (m-1-2);\end{tikzpicture} 이다.

(관찰 12.5.14.) H \trianglelefteq G 이고 K \le G 이면, HK \le G 이다.

(Group 의 Second Isomorphism Theorem) H \trianglelefteq G 이고 G \le G 일 때, 함수 \bar{\jmath} : \frac{K}{H \cap K } \to \frac{HK}{H} 를 \bar{\jmath} (\bar{k}) = \bar{k} , (k \in K) 로 정의하면, \bar{\jmath} 는 well-defined 된 group isomorphism 이다. 따라서, \begin{tikzpicture}\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] {\frac{K}{H\capK} &\frac{HK}{H} \\}; \path[-stealth] (m-1-1) edge node [above] {$\bar{\jmath}$} node [below]{$\approx$} (m-1-2);\end{tikzpicture} 이다.

(벡터공간의 Second Isomorphism Theorem) U, W \le V  일 때, 함수 \bar{\jmath} : \frac{W}{U \cap W } \to \frac{U + W}{W} 를 \bar{\jmath} (\bar{w}) = \bar{w} , (w \in W) 로 정의하면, \bar{\jmath} 는 well-defined 된 group isomorphism 이다. 따라서, \begin{tikzpicture}\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] {\frac{W}{U\capW} &\frac{U+W}{U} \\}; \path[-stealth] (m-1-1) edge node [above] {$\bar{\jmath}$} node [below]{$\approx$} (m-1-2);\end{tikzpicture} 이다.

(따름정리 12.5.18.) V 가 f.d.v.s. 일 때, U,W \le V 이면, dim(U+W) = dim U + dim W – dim(U \cap W) 이다.

