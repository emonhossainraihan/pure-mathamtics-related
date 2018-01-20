---

layout: post

title :[Linear Algebra] Inner Product Space

date : 2018-01-19 13:51:11 +0900

---

(Section 10) 내적공간

(subsection 10.1) Inner product space

(정의 10.1.1) X = ^{t}(a_{1}, …, a_{n}) , Y = ^{t}(b_{1}, …, b_{n}) \in \mathbb{C}^{n} 일 때, \langle X , Y \rangle = ^{t} X \cdot \bar{Y} = \sum_{i =1}^{n} a_{i} \bar{b_{i}} 로 정의하고 이를 \mathbb{C}^{n} 의 (Hermitian) dot product 라고 부른다.

(정의 10.1.4) (F = \mathbb{R} 혹은 F = \mathbb{C} 일 때, ) F^{n} \times F^{n} 에서 F로 가는 함수 (X,Y) \mapsto \langle X, Y \rangle 가, 모든 X,Y,Z \in F^{n}, c \in F 에 대해, 다음 조건

\langle X + Y , Z \rangle = \langle X, Z \rangle + \langle Y , Z \rangle 

\langle cX , Y \rangle = c \langle X , Y \rangle 

\langle X, Y \rangle = \bar{\langle Y , X \rangle}

X \neq 0 이면, (\langle X, X \rangle \in \mathbb{R} 이고) \langle X, X \rangle > 0

을 만족하면 , \langle , \rangle 을 F^{n} 의 inner product 라고 부른다. (특별히, F = \mathbb{C}인 경우에는 Hermitian inner product 라고 부르기도 한다.)

(관찰 10.1.5) \langle , \rangle 가 F^{n} 의 inner product 라면 다음이 성립한다. 

\langle X, Y + Z \rangle = \langle X , Y \rangle + \langle X , Z \rangle

\langle X , cY \rangle = \bar{c} \langle X, Y \rangle

(정의 10.1.6) (F = \mathbb{R} 혹은 F = \mathbb{C} 일 때, ) V를 F-vector space 라고 하자. (V가무한차원인 경우도 허용한다.) 이 때, 함수 \langle, \rangle : V \times V \to F 가, 모든 u,v,w \in V, c \in F 에 대해, 다음 조건

\langle u + v , w \rangle = \langle u, w \rangle + \langle v , w \rangle 

\langle cv , w \rangle = c \langle v , w \rangle 

\langle v, w \rangle = \bar{\langle w , v \rangle}

v \neq 0 이면, (\langle v, v \rangle \in \mathbb{R} 이고) \langle v, v \rangle > 0

을 만족하면 , \langle , \rangle 을 V 의 inner product 라고 부르고, inner product 가 주어진 V를inner product space (내적공간) 라고 부른다. (특별히, F = \mathbb{C} 인 경우에는 Hermitialn inner product 라고 부르기도 한다.)

(subsection 10.2) Inner product space 의 성질

(정의 10.2.2) v \in V 일 때, \Vert v \Vert = \sqrt{\langle v, v \rangle} 로 표기하고, \Vert v \Vert 를 v의 norm 이라고 부른다. Norm은 vector 의 길이(크기)로 이해한다.

(정의 10.2.5) v, w \in V 일 때, \langle v, w \rangle = 0 이면, v \perp w로 표기하고 v와 w는 서로 수직(perpendicular 또는 orthogonal) 이라고 말한다. (\langle v, w \rangle = 0 이면, \langle w ,v \rangle = 0 이다.)

S,T \subseteq V 일 때, [\langle v,w \rangle = 0 for all v \in S, w \in T ] 이면, S \perp T 로 표기하고 S 와 T는 서로 수직이라고 말한다.

(관찰 10.2.8) v,w \in V 이면, 다음이 성립한다.

(Cauchy-Schwarz Inequality) | \langle v, w \rangle | \le \Vert v \Vert \cdot \Vert w \Vert (등호가 성립할 필요충분조건은 {v,w} 가 일차종속인 것이다.)

(Triangle inequality) \Vert v + w \Vert \le \Vert v \Vert + \Vert w \Vert

(정의 10.2.10) V의 non-zero vector 들 {v_{i} | i \in I} 가 mutually perpendicular 이면 – 즉 [v_{i} \perp v_{j} for all i \neq j \in I] 이면 – {v_{i} | i \in I} 를 V의 orthogonal subset 이라고 부른다. 이 때, v_{i} 들이 모두 unit vector 이면, 이번에도 {v_{i} | i \in I } 를 V의 orthonormal subset 이라고 부른다.

V의 basis \mathfrak{B} 가 orthogonal subset 이면, \mathfrak{B} 를 V의 orthogonal basis 라고 부르고, orthonormals subset 이면 \mathfrak{B} 를 V의 orthonormal basis 라고 부른다.

(정의 10.2.14) S \subseteq V 일 때, S^{\perp} = {v \in V | v \perp w for all w \in S} 로 표기한다. 특히, W \le V 일 때에는 W^{\perp} 를 W의 orthogonal complement 라고 부른다.

(subsection 10.3) Gram-Schmidt Orthogonalization

(Gram-Schmidt Orthogonalization) (정리 10.3.1) V가 inner product space 이고 {v_{1}, …, v_{r}} 가 V의 linearly independent subset 이라고 하자.

w_{1} = v_{1} 으로, 그리고 2 \le i \le r 일 때에는 w_{i} = v_{i} - \frac{\langle v_{i}, w_{i-1} \rangle}{\langle w_{i-1} , w_{i-1} \rangle} w_{i-1} - \cdots - \frac{\langle v_{i}, w_{2} \rangle}{\langle w_{2}, w_{2} \rangle} w_{2} - \frac{\langle v_{i}, w_{1} \rangle}{ \langle w_{1}, w_{1} \rangle} w_{1} 으로 inductively 정의하면, \langle v_{1}, …, v_{r} \rangle = \langle w_{1}, …, w_{r} \rangle 이고, {w_{1}, …, w_{r}} 은 V의 orthogonal subset 이 된다.

따라서, {\frac{1}{\Vert w_{1} \Vert} w_{1} , …, \frac{1}{\Vert w_{r} \Vert} w_{r}} 은 V의 orthonormal subset 이 된다.

특별히, r = dim V 이면 , {\frac{1}{\Vert w_{1} \Vert} w_{1} , …, \frac{1}{\Vert w_{r} \Vert} w_{r}} 은 V의 orthonormal basis 가 된다.

(따름정리 10.3.4.) V가 유한차원 inner product space 이고 W \le V 라고 하자.

W 자신 inner product space 이므로, W도 orthonormal basis 를 갖는다.

따라서, V = W \oplus W^{\perp} 이고, 특별히 dim V = dim W + dim W^{\perp} 이다.

(따름정리 10.3.7) A \in \mathfrak{M}_{m,n}(\mathbb{R}) 의 row space \langle ^{t}[A]_{1}, …, ^{t}[A]_{m} \rangle 은 연립방정식 AX = 0 의 solution space 의 orthogonal complement 이다. 즉, ker (L_{A}) = {X \in \mathbb{R}^{n} | AX = 0} = \langle ^{t}[A]_{1}, …, ^{t}[A]_{m} \rangle^{\perp} 이다. 따라서, (따름정리 10.3.4.)에 의해 dim ker(L_{A}) = n – [row rank of A] 이다.

(subsection 10.4.) Standard Basis 대 Orthonormal Basis

(관찰 10.4.1.) \mathfrak{B} = {v_{1}, …, v_{n}} 이 inner product space V 의 orthogonal basis 이면, 다음이 성립한다.

v \in V 이면, v = \sum_{i = 1}^{n} \frac{\langle v,v_{i} \rangle}{\langle v_{i}, v_{i} \rangle} v_{i} (즉, [v]_{\mathfrak{B}} 의 i-번째 좌표는 \frac{\langle v, v_{i} \rangle}{\langle v_{i}, v_{i} \rangle}). 

그리고, \mathfrak{B} = {v_{1}, …, v_{n}} 이 inner product space V 의 orthonormal basis 이면, 다음이 성립한다.

v \in V 이면, v = \sum_{i = 1}^{n} \langle v,v_{i} \ranglev_{i} (즉, [v]_{\mathfrak{B}} 의 i-번째 좌표는 \langle v, v_{i} \rangle).

v,w \in V 이면, \langle v, w \rangle = ^{t} [v]_{\mathfrak{B}} \cdot \bar{[w]_{\mathfrak{B}}}.

(정의 10.4.2.) \mathfrak{B} = {v_{i} | i \in I} 가 inner product space V 의 orthonormal subset 이라고 하자. v \in V 일 때, \langle v, v_{i} \rangle 을 \mathfrak{B} 에 관한 v의 i-th Fourier coefficient 라고 부른다. 그리고, 이를 \mathfrak{B} 에 관한 v 의 i-번째 좌표로 생각한다.( 한편, \mathfrak{B} 가 V의 orthogonal subset 일 때에는 \frac{\langle v, v_{i}\rangle}{\langle v_{i}, v_{i} \rangle} 을 \mathfrak{B} 에 관한 v의 i-th Fourier coefficient 라고 부른다.)

(관찰 10.4.3.) W가 inner product space V의 finite dimensional subspace 이고, {v_{1}, …, v_{m}} 을 W의 orthonormal basis 라고 하자. v \in V 이면, v = w + w’ 인 w \in W 와 w’ \in W^{\perp} 가 유일하게 존재하고, w = \langle v, v_{1} \rangle v_{1} + \cdots + \langle v, v_{m} \rangle v_{m} 으로 주어진다.

(Closest Vector Problem) (관찰 10.4.4) 위 (관찰 10.4.3) 의 w는 v에 가장 가까운 W의 vector 이다.

(Bessel’s Inequality) (관찰 10.4.7) \mathfrak{B} = {v_{1}, …, v_{n}} 이 inner product space V 의 orthonormal subset 이면, 모든 v \in V 는 다음 부등식 \sum_{i = 1}^{n} |\langle v, v_{i} \rangle |^{2} \le \Vert v \Vert^{2} 을 만족한다.

(subsection 10.5) Inner product space 의 isomorphism

(정의 10.5.3) V 와 V’ 이 F-위의 inner product space 이고, 다음 조건 \langle \phi(v) , \phi(w) \rangle = \langle v, w \rangle , (v,w \in V) 을 만족하는 vector space isomorphism \phi : V \to V’ 이 존재하면, 우리는 V와 V’ 이 inner product space 로서 isomorphic 하다고 말하고, \phi 를 inner product space isomorphism 이라고 부른다.

(Classification of finite dimensional inner product space) (정리 10.5.5) V 와 W가 F-위의 유한차원 inner product space 일 때, 다음은 동치이다.

V와 W는 inner produce space 로서 isomorphic.

dim V = dim W.

(정리 10.5.6.) V가 \mathbb{R} -위의 유한차원 inner product space 일 때,

L(0) = 0 인 V의 rigid motion L 은 linear map 이다.

따라서, V 의 rigid motion M 은 translation 과 linear rigid motion 의 합성으로 쓸 수 있다.

V의 rigid motion 은 항상 bijection 이다.

(section 10.6) Orthogonal Group 과 Unitary Group

(정의 10.6.1) (F = \mathbb{R}) 인 경우) V가 inner product \langle , \rangle 가 주어진 \mathbb{R}-위 의 inner product space일 때, \mathbf{O}(V) = \mathbf{O}(V, \langle, \rangle ) = {L \in \mathfrak{L}(V,V) | \Vert Lv – Lw \Vert = \Vert v – w \Vert for all v, w \in V} 로 표기하고 [orthogonal group on V with respect to \langle , \rangle ] 라고 부른다. 또, \mathbf{O}(V) 의 원소를 orthogonal operator 라고 부른다.

(F = \mathbb{C}) 인 경우) V가 inner product \langle , \rangle 가 주어진 \mathbb{C}-위 의 inner product space일 때, \mathbf{U}(V) = \mathbf{U}(V, \langle, \rangle ) = {L \in \mathfrak{L}(V,V) | \Vert Lv – Lw \Vert = \Vert v – w \Vert for all v, w \in V} 로 표기하고 [unitary group on V with respect to \langle , \rangle ] 라고 부른다. 또, \mathbf{U}(V) 의 원소를 unitary operator 라고 부른다.

(정의 10.6.2.) \mathbb{C}^{n} 에 (Hermitian ) dot product 가 주어졌을 때, \mathbf{U}(n) = {A \in \mathfrak{M}_{n,n}(\mathbb{C}) | L_{A} \in \mathbf{U} (\mathbb{C}^{n} , dot product )} = {[L]_{\mathcal{E}}^{\mathcal{E}} \in \mathfrak{M}_{n,n}(\mathbb{C}) | L \in \mathbf{U} (\mathbb{C}^{n} , dot product )} 로 표기하고, 이를 (complex) unitary group 이라고 부른다. 그리고, \mathbf{U}(n) 의 원소를 (complex) unitary matrix 라고 부른다.

(정의 10.6.3.) V가 inner product \langle , \rangle 가 주어져 있는 F-위의 n-dimensional inner product space 이고, \mathfrak{B} 를 V의 orthonormal basis 라고 하자.

F = \mathbb{R} 이면, \mathbf{O}_{n} (\mathbb{R} , \langle, \rangle ) = {[L]_{\mathfrak{B}}^{\mathfrak{B}} \in \mathfrak{M}_{n,n}(\mathbb{R}) | L \in \mathbf{O} (V, \langle, \rangle ) } 로 표기하고, 이를 V와 \langle, \rangle 로부터 얻어진 orthogonal group 이라고 부른다.

F = \mathbb(C) 이면, \mathbf{U}_{n} (\mathbb{C} , \langle, \rangle ) = {[L]_{\mathfrak{B}}^{\mathfrak{B}} \in \mathfrak{M}_{n,n}(\mathbb{C}) | L \in \mathbf{U} (V, \langle, \rangle ) } 로 표기하고, 이를 V와 \langle, \rangle 로부터 얻어진 unitary group 이라고 부른다.

(명제 10.6.4) 위 (정의 10.6.3) 은 – 즉, \mathbf{O}_{n} (\mathbb{R} , \langle, \rangle ) 및 \mathbf{U}_{n} (\mathbb{C} , \langle, \rangle) 의 정의는 V의 orthonormal basis 의 선택과는 무관하다.

(따름명제 10.6.5.) 

\mathfrak{B} 가 [dot product 가 주어진 Euclidean space \mathbb{R}^{n}] 의 임의의 orthonormal basis 이면, \mathbf{O}(n) = {[L]_{\mathfrak{B}}^{\mathfrak{B}} \in \mathfrak{M}_{n,n}(\mathbb{R}) | L \in \mathbf{O}(\mathbb{R}^{n})} 이다. (단, \mathbf{O}(\mathbb{R}^{n}) = \mathbf{O}(\mathbb{R}^{n}, dot product) .)

\mathfrak{B} 가 [(Hermitian) dot product 가 주어진 \mathbb{C}^{n}] 의 임의의 orthonormal basis 이면, \mathbf{U}(n) = {[L]_{\mathfrak{B}}^{\mathfrak{B}} \in \mathfrak{M}_{n,n}(\mathbb{C}) | L \in \mathbf{U}(\mathbb{C}^{n})} 이다. (단, \mathbf{U}(\mathbb{C}^{n}) = \mathbf{U}(\mathbb{C}^{n}, dot product) .)

(관찰 10.6.6.) V가 inner product \langle , \rangle 가 주어진 n-dimensional inner product space 이고, L \in \mathfrak{L} (V,V) 일 때, 다음 조건들은 동치이다.

 \Vert Lv – Lw \Vert = \Vert v – w \Vert for all v, w \in V.

\Vert Lv \Vert = \Vert v \Vert for all v \in V.

\langle Lv, Lv \rangle = \langle v, v \rangle for all v \in V.

\langle Lv, Lw \rangle = \langle v, w \rangle for all v, w \in V.

\mathfrak{B} 가 V의 orthonormal basis 이면, L(\mathfrak{B}) 도 V의 orthonormal basis.

(정의 10.6.9) A \in \mathfrak{M}_{m,n}(\mathbb{C}) 일 때,A^{*} = \bar{^{t}A} = ^{t}\bar{A} 로 표기하고, A^{*} 를 A의 adjoint matrix 라고 부른다. (A \in \mathfrak{M}_{n,n}(\mathbb{R}) 일 때에는, 물론 A^{*} = ^{t} A로 이해한다.)

(정의 10.6.13.) 다음 표기법 \mathbf{SU} (n) = {A \in \mathbf{U}(n) | det(A) = 1} 이다. \mathbf{SU} (n) 을 special unitary group 이라고 부른다.

(subsection 10.7.) Adjoint Matrix 와 그 응용

(관찰 10.7.1.) F^{n} 과 F^{m} 에 각각 dot product \langle , \rangle 가 주어져 있다고 하자. 이 때, A \in \mathfrak{M}_{n,n} (F) 이면, \langle AX, Y \rangle = \langle X, A^{*} Y \rangle , \langle Y , AX \rangle = \langle A^{*} Y , X \rangle , (X \in F^{n}, Y \in F^{m}) 이 성립한다.

(정의) AX = B 가 solution 을 갖지 않는 경우에 \Vert AX_{0} – B \Vert 가 최소인 X_{0} 을 구하는 문제를 최소자승법 (Least Squares Approximation – LSA) 라고 한다.

(명제 10.7.3.) A \in \mathfrak{M}_{m,n} (F) 이고 B \in F^{m} 일 때,

LSA-문제의 solution – 즉, [\Vert AX_{0} – B \Vert \le \Vert AX – B \Vert for all X in F^{n} ] 인 X_{0} \in F^{n} 은 항상 존재한다.

만약 L_{A} 가 injective 이면, LSA-문제의 solution X_{0} 는 유일하게 결정된다.

(명제 10.7.4.) A \in \mathfrak{M}_{m,n}(F) 이고 B \in F^{m} 일 때, 다음은 동치이다.

 X_{0} 는 LSA-문제의 solution (즉, \Vert AX_{0} – B \Vert \le \Vert AX – B \Vert for all X \in F^{n} )

(A^{*} A ) X_{0}  = A^{*} B.

(명제 10.7.5) A \in \mathfrak{M}_{m,n} (F) 이고 B \in F^{m} 이라고 하자. 만약, m \ge n 이고 rk(A) = n 이면 (즉 A가 full rank 를 가지면), LSA-문제의 solution X_{0} 은 존재하고 하나뿐이다.

(관찰 10.7.9.) A \in \mathfrak{M}_{m,n}(F) 이면, rk(A^{*} A) = rk(A) 이다. (따라서, A가 full rank 를 가지면, (A^{*}A) 는 가역행렬이다.)

(관찰 10.7.11) A \in \mathfrak{M}_{m,n}(F) 이면, 다음이 성립한다.

im(A^{*}) = (ker A)^{\perp} . 즉, ker A = (im(A^{*})^{\perp}

im(A) = (ker(A^{*}))^{\perp}. 즉, ker(A^{*}) = (im A)^{\perp}

(정의) Minimal solution problem 은 AX = B가 solution 을 가질 때, 크기가 가장 작은 solution 을 구하는 것이다.

(명제 10.7.12.) A \in \mathfrak{M}_{m,n} (F) 이고 B \in F^{m} 일 때, AX = B 가 solution 을 갖는다고 가정하자. 그러면

AX = B 의 minimal solution – 즉 , AX_{0} = B 이고 [X \in F^{n} 이 AX = B 를 만족하면 \Vert X_{0} \Vert \le \Vert X \vert ] 인 X_{0} \in F^{n} 이 유일하게 존재한다.

{X_{0}} = [AX = B 의 해집합] \cap im(A^{*}) .

