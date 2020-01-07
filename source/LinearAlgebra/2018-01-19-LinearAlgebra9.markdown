---

layout: post

title : (Linear Algebra) Rigid Motion

date : 2018-01-19 13:51:11 +0900

---

(Section 9) \mathbb{R}^{n} 의 Rigid Motion

(subsection 9.1) \mathbb{R}^{n} -공간의 Dot product 와 Euclidean norm

(정의 9.1.1) X = ^{t}(a_{1} , …, a_{n}) , Y = ^{t}(b_{1}, …, b_{n}) \in \mathbb{R}^{n} 일 때, \langle X , Y \rangel = ^{t} X \cdot Y = \sum_{i = 1}^{n} a_{i}b_{i} 로 정의하고 이를 \mathbb{R}^{n} 의 dot product 라고 부른다. 그리고 dot product 가 주어진 \mathbb{R}^{n}-공간을 Euclidean space 라고 부른다.

(정의 9.1.4) X \in \mathbb{R}^{n} 일 때, \Vert X \Vert = \sqrt{\langle X , X \rangle} 로 표기하고, \Vert X \Vert 를 X의 (Euclidean) norm 이라고 부른다. Norm 은 vector 의 길이(크기)로 해석한다.

(정의 9.1.9.) X,Y \in \mathbb{R}^{n} 일 때, \langle X, Y \rangle = 0 이면, X \perp Y 로 표기하고 X 와 Y는 서로 수직 (perpendicular, 또는 orthogonal) 이라고 말한다.

 S, T \subseteq \mathbb{R}^{n} 일 때, \[\langle X , Y \rangle = 0 for all X \in S , Y \in T ] 이면, S \perp T 로 표기하고 S와 T는 서로 수직이라고 말한다.

(정의 9.1.11) \mathbb{R}^{n} 의 non-zero vector 들 X_{1}, …, X_{m} 이 mutually perpendicular 이면 – 즉 , [X_{i} \perp X_{j} for all 1 \le i \neq j \le m] 이면 – {X_{1}, …, X_{m}} 을 \mathbb{R}^{n} 의 orthogonal subset 이라고 부른다. 이 때, [\Vert X_{k} \Vert = 1 for all 1 \le k \le m] 의 조건도 만족하면, {X_{1}, …, X_{m}} 을 \mathbb{R}^{n} 의 orthonormal subset 이라고 부른다.

\mathbb{R}^{n} 의 basis \mathfrak{B} 가 orthogonal subset 이면, \mathfrak{B} 를 \mathbb{R}^{n} 의 orthogonal basis 라고 부르고, orthonormal subset 이면 \mathfrak{B} 를 \mathbb{R}^{n} 의 orthonormal basis 라고 부른다.

(정의 9.1.14) S \subseteq \mathbb{R}^{n} 일 때, S^{\perp} = {X \in \mathbb{R}^{n} | X \perp Y for all Y \in S } 로 표기하고, “S perp” 로 읽는다. 특히 W \le \mathbb{R}^{n} 일 때에는 W^{\perp} 를 W의 orthogonal complement 라고 부른다.

(관찰 9.1.15) S \subseteq \mathbb{R}^{n} , W \le \mathbb{R}^{n} 이고 \mathfrak{C} 가 W의 basis이면, 다음이 성립한다.

S^{\perp} 는 \mathbb{R}^{n} 의 subspace.

S^{\perp} = \langle S \rangle^{\perp}.

W^{\perp} = \mathfrak{C}^{\perp}.

(subsection 9.2.) \mathbb{R}^{n} -공간의 Rigid Motion

(정의 9.2.1.) 함수 M : \mathbb{R}^{n} \to \mathbb{R}^{n} 이 조건 \Vert M(X) – M(Y) \Vert = \Vert X – Y \Vert (X,Y \in \mathbb{R}^{n}) 을 만족하면 M을 \mathbb{R}^{n} 의 rigid motion 또는 isometry 라고 부른다.

(관찰 9.2.5) 함수 M : \mathbb{R}^{n} \to \mathbb{R}^{n} 이 \mathbb{R}^{n} 의 rigid motion이면, 

M은 injective 이다.

M은 연속함수이다.

(관찰 9.2.8.) L(0) = 0 인 \mathbb{R}^{n} 의 rigid motion L 은 다음 성질을 갖는다.

\Vert L(X) \Vert = \Vert X \Vert for all X \in \mathbb{R}^{n}.

\langle L(X), L(X) \rangle = \langle X , X \rangle for all X \in \mathbb{R}^{n}.

\langle L(X), L(Y) \rangle = \langle X, Y \rangle for all X , Y \in \mathbb{R}^{n}.

\mathfrak{B} 가 \mathbb{R}^{n} 의 orthonormal basis 이면, L(\mathfrak{B}) 도 \mathbb{R}^{n} 의 orthonormal basis.

(관찰 9.2.9) A \in \mathfrak{M}_{n,n}(\mathbb{R}) 의 column 들 {[A]^{1}, …, [A]^{n}} 이 \mathbb{R}^{n} 의 orthonormal basis 이면, linear map L_{A} 는 rigid motion 이다.

(관찰 9.2.10) L(0) = 0 인 \mathbb{R}^{n} 의 rigid motion L 이 \mathbb{R}^{n} 의 orthonormal basis \mathfrak{B} = {X_{i}} 를 고정하면 – 즉 , [L(X_{j}) = X_{j} for all j = 1, …, n ] 이면, - L은 항등사상이다.

(정리 9.2.11) L(0) = 0 인 \mathbb{R}^{n} 의 rigid motion L 은 linear map 이다.

따라서, \mathbb{R}^{n} 의 rigid motion M 은 translation 과 linear rigid motion 의 합성으로 쓸 수 있다.

(따름정리 9.2.12) \mathbb{R}^{n} 의 rigid motion 은 항상 bijection 이다.

(정의 9.2.13) \mathbb{R}^{n} 의 linear rigid motion 을 (real) orthogonal operator 라고 부른다. 또, L 이 \mathbb{R}^{n} 의 orthogonal operator 이고 L = L_{A} 일 때, real (n \times n)-matrix A 를 (real) orthogonal matrix 라고 부른다.

(subsetion 9.3.) Orthogonal operator / Matrix

(정의 9.3.1.) \mathbb{R}^{n} 의 orthogonal operator 전체의 집합을 [orthogonal group on \mathbb{R}^{n}] 이라고 부르고, \mathbf{O}(\mathbb{R}^{n}) 이라고 부른다. 즉, \mathbf{O}(\mathbb{R}^{n}) = {L \in \mathfrak{L} (\mathbb{R}^{n}, \mathbb{R}^{n}) | \Vert L(X) – L(Y) \Vert = \Vert X – Y \Vert for all X, Y \in \mathbb{R}^{n}} . 

또, real ( n \times n )-orthogonal matrix 전체의 집합을 (real) orthogonal group 이라고 부르고 \mathbf{O}(n) 으로 표기한다. 즉, \mathbf{O}(n) = {A \in \mathfrak{M}_{n,n} (\mathbb{R}) | \Vert AX – AY \Vert = \Vert X – Y \Vert for all X, Y \in \mathbb{R}^{n}} 이다.

(따름정리 9.3.2.) M : \mathbb{R}^{n} \in \mathbb{R}^{n} 이 rigid motion 이면, M(X) = AX + B (X \in \mathbb{R}^{n}) 인 A \in \mathbf{O}(n) 과 B \in \mathbb{R}^{n}이 유일하게 존재한다.

(관찰 9.3.3.) L:\mathbb{R}^{n} \to \mathbb{R}^{n} 이 linear 일 때, 다음 조건들은 동치이다.

 \Vert LX – LY \Vert = \Vert X – Y \Vert for all X, Y \in \mathbb{R}^{n} . (즉, L \in \mathbf{O}(\mathbb{R}^{n}).) 

\Vert LX \Vert = \Vert X \Vert for all X \in \mathbb{R}^{n}.

\langle LX, LX \rangle = \langle X, X \rangle for all X \in \mathbb{R}^{n}

\langle LX, LY \rangle = \langle X, Y \rangle for all X, Y \in \mathbb{R}^{n}.

\mathfrak{B} 가 \mathbb{R}^{n} 의 orthonormal basis 이면, L(\mathfrak{B}) 도 \mathbb{R}^{n} 의 orthonormal basis 이다.

(관찰 9.3.5.) A \in \mathfrak{M}_{n,n} (\mathbb{R}) 일 때, 다음 조건들은 동치이다.

\Vert AX – AY \Vert = \Vert X – Y \Vert for all X, Y \in \mathbb{R}^{n} . (즉, A \in \mathbf{O}(n).) 

\Vert AX \Vert = \Vert X \Vert for all X \in \mathbb{R}^{n}.

\langle AX, AX \rangle = \langle X, X \rangle for all X \in \mathbb{R}^{n}

\langle AX, AY \rangle = \langle X, Y \rangle for all X, Y \in \mathbb{R}^{n}.

A의 column 들의 집합 {[A]^{1}, …, [A]^{n}} 은 \mathbb{R}^{n} 의 orthonormal basis.

^{t}A \cdot A = I = A \cdot ^{t}A . 즉, A^{-1} = ^{t}A.

^{t}A  \in \mathbf{O}(n).

A의 row들의 집합 {[A]_{1}, …, [A]_{n}} 은 \mathfrak{M}_{1,n}(\mathbb{R}) 의 orthonormal basis.

(정의 9.3.8) Special orthogonal group \mathbf{SO}(n) 을 \mathbf{SO}(n) = {A \in \mathbf{O}(n) | det(A) = 1} 로 정의한다. 이제, \mathbf{SO}(\mathbb{R}^{n}) = {L \in \mathbf{O}(\mathbb{R}^{n}) |det(L) = 1} 로 표기한다.

기하학에서 A \in \mathbf{SO}(n) 이면 L_{A} 를 \mathbb{R}^{n} 의 orientation preserving orthogonal operator, A \in \mathbf{O}(n) - \mathbf{SO}(n) 이면 L_{A} 를 \mathbb{R}^{n} 의 orientation reversing orthogonal operator 라고 부른다.

(subsection 9.4.) Reflection

(정의 9.4.2.) 0 \neq Y \in \mathbb{R}^{n} 일 때, 함수 S_{Y} : \mathbb{R}^{n} \to \mathbb{R}^{n} 을 S_{Y} (X) = X - \frac{2 \langle X , Y \rangle}{\langle Y, Y \rangle} Y (X \in \mathbb{R}^{n}) 으로 정의하고, S_{Y} 를 Y에 관한 reflection 또는 symmetry 라고 부른다.

(subsection 9.5.) \mathbf{O}(2) 와 \mathbf{SO}(2)

(정리 9.5.2.) \mathbf{SO}(2) 의 원소는 2-dimensional rotation 뿐이다. 즉, \mathbf{SO}(2) = {\begin{pmatrix}cos \theta & -sin \theta \\ sin \theta & cos \theta \end{pmatrix} | 0 \le \theta < 2\pi} = {\begin{pmatrix} x & -y \\ y & x \end{pmatrix} |x,y \in \mathbb{R} , x^{2} + y^{2} = 1}

(따름정리 9.5.3.) \mathbf{O}(2) 의 구조는 다음과 같다. 즉, \mathbf{O}(2) = \mathbf{SO}(2) \mathfrak{U} {\begin{pmatrix} x & -y \\ y & x \end{pmatrix} |x,y \in \mathbb{R} , x^{2} + y^{2} = 1}

(관찰 9.5.6.) \theta \in \mathbb{R} 이면, S_{\theta} = S_{^{t}(-sin \frac{\theta}{2} , cos \frac{\theta}{2} } 이 성립한다.

따라서, \mathbb{R}^{2} 의 모든 reflection 은 S_{\theta} 의 꼴이다.

(따름정리 9.5.7.) 

\mathbb{R}^{2} 의 orthogonal operator L 은 rotation 이거나 reflection 둘 중 하나이다. 즉, det(L) = 1 이면 L 은 rotation 이고, det(L) = -1 이면 L 은 reflection 이다.

따라서, \mathbb{R}^{2} 의 rotation \mathbb{R} 과 reflection S 의 합성 R \bullet S 와 S \bullet R 은 언제나 \mathbb{R}^{2} 의 reflection 이다.

역으로, \mathbb{R}^{2} 의 reflection S를 하나 고정하면, \mathbb{R}^{2} 의 모든 reflection 은 [S \bullet R for some rotation R] 의 꼴로 유일하게 쓸 수 있다.

(관찰 9.5.8.) S가 \mathbb{R}^{2} 의 reflection 이고 \theta \in \mathbb{R} 이면, S^{-1} \bullet R_{\theta} \bullet S = (R_{\theta})^{-1} , 즉 R_{\theta} \bullet S = S \bullet R_{-\theta} 가 성립한다.

(subsection 9.6.) \mathbf{SO}(3) 와 \mathbf{SO}(n) 

(정의 9.6.1.) Z \in \mathbb{R}^{3} 가 unit vector 일 때, \mathfrak{B} = {Z,X,Y} 가 \mathbb{R}^{3} 의 rotation basis 인 X,Y 를 찾자. 그리고, det(Z,X,Y) = det(X,Y,Z) = 1 이 되도록 X,Y 의 순서를 정하자. 이 때, 원점을 중심으로 하는 \mathbb{R}^{3} 의 rotation R_{Z,\theta} : \mathbb{R}^{3} \to \mathbb{R}^{3} 를

[R_{Z,\theta}]_{\mathfrak{B}}^{\mathfrak{B}} = \begin{pmatrix} 1 & 0 & 0 \\ 0 & cos \theta & -sin \theta \\ 0 & sin \theta & cos \theta \end{pmatrix} 

라고 정의하자. (이 때, Z를 회전축, \langle X \rangle \oplus \langle Y \rangle 을 회전판, \theta 를 회전각 이라고 부르면 자연스럽다.)

(정리 9.6.3.) \mathbf{SO}(\mathbb{R}^{3}) 의 원소는 모두 \mathbb{R}^{3} 의 rotation 이다.

(따름정리 9.6.4.) \mathbb{R}^{3} 의 두 rotation 의 합성도 rotation 이다.

(정의 9.6.6.) 임의의 n 에 대하여, \mathbf{SO}(\mathbb{R}^{n}) 의 원소를 – 혹은, \mathbf{SO} (n)의 원소를 - \mathbb{R}^{n} 의 rotation 이라고 정의한다.

