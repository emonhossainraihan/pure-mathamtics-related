---
layout: post
title : Determinant 행렬식
date : 2018-01-19 13:51:08 +0900
---
(Section 6) 행렬식

(subsection 6.1) Alternating Multilinear form

(정의 6.1.1) \\(V_{1}, …, V_{k}\\) 가 벡터공간일 때, 함수 \\(\mu : V_{1} \times \cdots \times V_{k} \to F\\) 가 모든 k-개의 좌표에 대하여 linear 일 때, 즉 임의의\\( i = 1,2, …, k\\) 에 대하여 \\(\mu(…, au_{i} + bw_{i}, …) = a\mu(…, u_{i},…) + b\mu(…,w_{i},….) , (u_{i}, w_{i} \in V_{i}, a,b \in F)\\) 일 때, 우리는 \\(\mu\\) 를 k-linear form 이라고 부른다. 특히, \\(k = 2\\) 일 때는 \\(\mu\\) 를 bilinear form 이라고 부른다. 

\\(V_{1} = \cdots = V_{k} = V\\) 인 경우에는 \\(\mu\\) 를 k-linear form on \\(V\\) 라고 부른다.

(정의 6.1.6) V 가 벡터공간이고 \\(\mu : V \times \cdots \times V \to F\\) 가 k-linear form 이라고 하자. 만약 모든 \\(v \in V\\) 에 대하여 \\(\mu (…, v, …, v , …) = 0\\) 이면 – 즉 두 좌표가 같을 때 \\(\mu\\) 의 함수값이 0 이면 – 우리는 \\(\mu\\) 를 alternating k-linear form on V 라고 부른다.

(관찰 6.1.7) \\(\mu : V \times \cdots \times V \to F\\) 를 alternating k-linear form 이라고 하면, 모든 \\(v, w \in V\\) 에 대해 \\(\mu(…, v, …, w, …) = - \mu(…, w, …, v, …)\\) 이다. 즉, 두 좌표의 위치를 교환하면 부호가 바뀐다.

(표기법 6.1.8) 이 장에서는, \\(\mathfrak{M}_{n,n} (F) = F^{n} \times \cdots \times F^{n}\\) (n 번 곱) 의 표기법을 사용한다. 즉, \\(A \in \mathfrak{M}_{n,n} (F)\\) 일 때,\\( A = (\left[A\right]^{1}, …, \left[A\right]^{n})\\) (단, \\(\left[A\right]^{j}\\) 는 A의 j-th column) 으로 표기한다.

(정리 6.1.9) 조건 [\\(det(I_{n}) = det (e_{1}, …, e_{n}) = 1\\)] 을 만족하는 alternating n-linear form det : \\(F^{n} \times \cdots \times F^{n} \to F\\) 는 존재하고, 단 하나뿐이다. \\(det(A) = |A|\\) 의 표기법도 사용한다.

(subsection 6.2) Symmetric Group

(정의 6.2.1) 함수 \\(\sigma : \lbrace1, …, n\rbrace \to \lbrace1, …, n\rbrace\\) 전체의 집합을 \\(T_{n}\\) 으로 표기하고, \\(S_{n} = \lbrace\sigma \in T_{n} | \sigma is_bijection \rbrace\\) 으로 정의한다. \\(S_{n}\\) 은 symmetric group 이라고 부른다. Symmetric group 의 원소는 permutation 이라고 부른다. 우리는 \\(|T_{n}| = n^{n} , |S_{n}| = n!\\) 인 것을 잘 알고 있다.

(표기법 6.2.3) \\(\sigma \in S_{n}\\) 일 때, 우리는 다음의 표기법을 사용한다.

\\(\sigma = \begin{pmatrix} 1 & 2 & \cdots & n 



 \sigma(1) & \sigma(2) & \cdots & \sigma(n) \end{pmatrix}\\)

(Cycle notation)\\(k \le n\\) 이고, \\(i_{1}, i_{2}, …, i_{k} (\le n)\\) 가 서로 다른 k 개의 자연수일 때, \\(\sigma = (i_{1}, i_{2}, …, i_{k}) \in S_{n}\\) 은 다음과 같이 정의된 permutation 을 의미한다.

\\(\begin{cases} \sigma(i_{h}) = i_{h+1} & (h = 1,2, …, k-1) 



 \sigma(i_{k}) = i_{1},&  



 \sigma(j) = j & (j \notin {i_{1}, i_{2}, …, i_{k}}) \end{cases}\\)

\\((i_{1}, i_{2}, …, i_{k})\\) 는 k-cycle 이라고 부른다. 특별히 k = 2 인 경우 \\((i_{1}, i_{2})\\) 를 transposition 이라고 부른다. (1-cycle 은 항등사상)

(관찰 6.2.8) 

\\(\sigma\\) 와 \\(\tau\\) 가 disjoint cycle 이면, \\(\sigma \bullet \tau = \tau \bullet \sigma\\) 이다.

모든 permutation 은 disjoint cycle 들의 합성으로 나타낼 수 있고, 그 방법은 (합성의 순서를 제외하고) 유일하다.

모든 permutation 은 transposition 들의 합성으로 나타낼 수 있다.

(정의 6.2.9) 함수 \\(sgn : S_{n} \to {\mp 1}\\) 을 \\(sgn(\sigma) = (-1)^{r}\\) (단, \\(\sigma\\) 는 r-개 transposition 의 합성) 이라고 정의하자. 우리는 sgn 을 signum 혹은 sign 이라고 읽는다.

(명제 6.2.10) 위 (정의 6.2.9) 의 \\(sgn : S_{n} \to {\mp 1}\\) 은 well-defined 되어있다.

(정의 6.2.11)\\(\sigma \in S_{n}\\) 일 때, \\(sgn(\sigma) = 1\\) 이면 \\(\sigma\\) 를 even permutation 이라고 부르고, \\(sgn(\sigma) = -1\\) 이면 \\(\sigma\\) 를 odd permutation 이라고 부른다. 또, \\(A_{n} = {\sigma \in S_{n} | sgn(\sigma) = 1}\\) 이라고 표시하고, \\(A_{n}\\) 을 alternating group 이라고 부른다.

(정의 6.2.15) \\(\mathfrak{B} = {v_{1}, …. , v_{n}}\\) 이 V의 ordered basis 이고 \\(\sigma \in S_{n}\\) 일 때, V의 새로운 ordered basis \\(\mathfrak{B}_{\sigma} = {v_{\sigma(1)} , v_{\sigma(2)}, …, v_{\sigma(n)}}\\) 을 생각하자. 이때, (\\(n \times n\\))-transition matrix \\(\left[I\right]_{\mathfrak{B}}^{\mathfrak{B}_{\sigma}}\\) 를 \\(\sigma\\) 에 대응하는 permutation matrix 라고 부르고, \\(I_{\sigma} = \left[I\right]_{\mathfrak{B}}^{\mathfrak{B}_{\sigma}}\\) 로 표기한다.

(관찰) \\(\sigma, \tau \in S_{n}\\) 일 때, 다음이 성립한다.

\\(I_{\sigma}\\) 의 j-th column 은 \\(e_{\sigma(j)}\\) . 즉 \\(I_{\sigma} = (e_{\sigma(1)}, …, e_{\sigma(n)}) \\)

\\(A \in \mathfrak{M}_{n,n}(F)\\) 이면, \\(AI_{\sigma} = (\left[A\right]^{\sigma(1)} , …, \left[A\right]^{\sigma(n)})\\) .

\\(I_{\sigma} \cdot I_{\tau} = I_{\sigma \bullet \tau}\\).

\\((I_{\sigma})^{-1} = I_{(\sigma^{-1})} = ^{t}(I_{\sigma}) \\)

\\(I_{\sigma} = I_{\tau}\\) 이면, \\(\sigma = \tau\\)

(정의 6.2.19) \\(\mathfrak{B} = {v_{1}, …, v_{n}}\\) 이 V의 고정된 ordered basis 이고 \\(\sigma \in S_{n}\\) 일 때, Linear extension theorem 을 이용하여 선형사상 \\(P_{\sigma} : V \to V\\) 를 \\(P_{\sigma} (v_{i}) = v_{\sigma(i)}\\) , (i = 1, …, n) 으로 정의하자.

(표기법 6.2.22) \\(\lambda_{i} \in F\\) 일 때, (i,i)-성분이 \\(\lambda_{i}\\) 인 (\\(n \times n\\))-대각행렬 (diagonal matrix) 를 \\(diag(\lambda_{1}, …, \lambda_{n})\\) 으로 표기한다.

(subsection 6.3) Determinant 의 정의 1

(관찰 6.3.1) 만약 \\(D : \mathfrak{M}_{n,n} (F) \to F\\) 가 (정리 6.1.9) 의 조건을 만족한다면, \\(A \in \mathfrak{M}_{n,n}(F)\\)이고 \\(\sigma \in S_{n}\\) 일 때, 다음이 성립한다.

\\(D(\left[A\right]^{\sigma(1)} , …, \left[A\right]^{\sigma(n)} ) = sgn(\sigma) \cdot D(\left[A\right]^{1}, …, \left[A\right]^{n}) = sgn(\sigma) \cdot D(A)\\),

\\(D(e_{\sigma(1)} , … e_{\sigma(n)}) = sgn(\sigma)\\)

(정리 6.3.2. 정리 6.1.9 의 \\(det : \mathfrak{M}_{n,n} (F) \to F\\) 는 \\(det(A) = |A| = det(a_{ij}) = \sum_{\sigma \in S_{n}} sgn(\sigma) \cdot a_{\sigma(1), 1} a_{\sigma(2), 2} \cdots a_{\sigma(n), n}\\) 으로 주어진다.

(따름정리 6.3.7) \\(A \in \mathfrak{M}_{n,n} (F)\\) 이면 \\(det(^{t}A) = det(A)\\) 이다.

(따름정리 6.3.8) \\(det : \mathfrak{M}_{n,n} (F) \to F\\) 를 n-개의 row들에 관한 함수로 보더라도, det 는 \\(det(I) = 1\\)인 유일한 alternating n-linear form 이다.

(subsection 6.4) Determinant 의 성질

(명제 6.4.1) \\(A, B \in \mathfrak{M}_{n,n} (F)\\) 이면, \\(det(AB) = det(A)det(B)\\) 가 성립한다.

(따름정리 6.4.2) A가 invertible이면, 물론 \\(det(A) \neq 0\\) 이고, \\(det(A^{-1}) = \frac{1}{det(A)} = det(A)^{-1}\\) 이다.

(관찰 6.4.5) \\(A \in \mathfrak{M}_{n,n} (F)\\)일 때, 만약 \\({\left[A\right]^{1}, …, \left[A\right]^{n}}\\) 이 linearly dependent 이면, \\(det(A) = 0\\) 이다.

(따름정리 6.4.6) 다음은 동치이다.

 A는 invertible.

\\(det(A) \neq 0\\).

(Gaussian Elimination 과 Determinant) (명제 6.4.11) 행렬식은 다음 성질을 갖는다.

어떤 한 column 에 다른 column 의 상수배를 더해주어도, 행렬식은 변하지 않는다. 즉, \\(i \neq j\\) 이고 \\(c \in F\\) 일 때, i-th column 에 [j-th column 의 c-배] 를 더해주면,  \\(det(…, \left[A\right]^{i} + c\left[A\right]^{j}, …, \left[A\right]^{j}, …) = det(A)\\) 이다.

위 성질에서 ‘column’ 을 ‘row’로 바꾸어도 성질이 성립한다.

(subsection 6.5) Determinant 의 정의 2

(표기법 6.5.1) \\(A = (a_{ij}) \in \mathfrak{M}_{n,n}(F)\\) 일 때, \\(M_{ij}\\) 를 [A에서 i-th row 와 j-th column 을 제거한] (\\((n-1) \times (n-1)\\))-행렬이라 하고, \\(\hat{A}_{ij} = det(M_{ij})\\) 로 표기한다. 우리는 \\(\hat{A}_{ij}\\) 를 A 의 (i,j)-minor 라 부른다.

(정의 6.5.2) j-th column 에 관한 전개(expansion) \\(D^{j} : \mathfrak{M}_{n,n} (F) \to F\\) 를 \\(D^{j}(A) = \sum_{i =1}^{n} (-1)^{i+j} a_{ij}\hat{A}_{ij} , (j = 1,…,n)\\) 로 정의하고, 마찬가지로 i-th row 에 관한 expansion \\(D_{i} :  \mathfrak{M}_{n,n} (F) \to F\\) 를 \\(D_{i}(A) = \sum_{j =1}^{n} (-1)^{i+j} a_{ij}\hat{A}_{ij} , (j = 1,…,n)\\) 로 정의한다.

(정리 6.5.6) (정의 6.5.2) 에서 정의된 2n-개의 함수 \\(D_{i}, D^{j} : \mathfrak{M}_{n,n}(F) \to F\\) 는 모두 alternating n-linear form 이고, \\(I_{n}\\) 에서의 값이 1이다. 따라서, 이 2n-개의 함수가 모두 \\(det : \mathfrak{M}_{n,n}(F) \to F\\) 와 같은 함수이다.

(subsection 6.6) Cramer’s Rule

(Cramer’s Rule) (정리 6.6.1) \\(A \in \mathfrak{M}_{n,n}(F)\\) 일 때, \\(X = ^{t}(x_{1}, …, x_{n}) \in F^{n}\\) 이 연립방정식 \\(AX = B\\) 의 solution이면, \\(det(A)x_{i} = det(\left[A\right]^{1}, …, B, …, \left[A\right]^{n})\\) (i = 1, …, n) 이어야 한다. 이 식에서 \\((\left[A\right]^{1}, …, B, …, \left[A\right]^{n}\\)) 은 A의 i-tho column 을 B로 바꿔치기한 행렬을 뜻한다.

(명제 6.6.4) \\(A = (a_{ij}) \in \mathfrak{M}_{n,n}(F)\\) 가 invertible matrix 이면,\\( A^{-1} = ^{t} (\frac{(-1)^{i+j} \hat{A}_{ij}}{det(A)} ) \\)이다. 즉, \\(A^{-1}\\) 의 (i,j)-좌표는 \\(\frac{(-1)^{i+j} \hat{A}_{ji}}{det(A)}\\) 이다.

(subsection 6.7) Adjoint Matrix

(정의 6.7.1) \\(A \in \mathfrak{M}_{n,n}(F)\\) 일 때, \\(adj(A) = ^{t}((-1)^{i+j} \hat{A}_{ij})\\) (즉 , \\(adj(A)\\) 의 (i,j)-좌표는 \\((-1)^{i+j} \hat{A}_{ji})\\) 라고 표기하고, \\(adj(A)\\) 를 A의 adjoint matrix 라 부른다.

(정리 6.7.2) \\(A \in \mathfrak{M}_{n,n} (F)\\) 이면, \\(A \cdot adj(A) = det(A) \cdot I_{n} = adj(A) \cdot A\\) 이다. (A 가 가역일 필요는 없다.)

(따름정리 6.7.3) \\(A = (a_{ij}) \in \mathfrak{M}_{n,n}(F)\\) 이면, \\(\sum_{k = 1}^{n} (-1)^{k+j} a_{ik} \hat{A}_{jk} = \delta_{ij} \cdot det(A) = \sum_{k=1}^{n} (-1)^{k+j} a_{ki} \hat{A}_{kj}\\)

