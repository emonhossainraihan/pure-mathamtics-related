---
layout: post
title : Characteristic polynomial and Diagonalization 특성다항식과 대각화
date : 2018-01-19 13:51:09 +0900
---
(section 7) 특성다항식과 대각화

(subsection 7.1) Eigen-vector 와 Eigen-value

(정의 7.1.1)\\(A \in \mathfrak{M}_{n,n}(F)\\) 일 때, \\(AX = \lambda X\\) 인 \\(\lambda \in F\\) 와 \\(0 \neq X \in F^{n}\\) 이 존재하면, 우리는 X를 eigen-value \\(\lambda\\) 를 갖는 (\\(\lambda\\) 에 대응하는) A의 eigenvector라 부른다. 마찬가지로, \\(L \in \mathfrak{L}(V,V)\\) 이고, \\(Lv = \lambda v\\) 인 \\(\lambda \in F\\) 와 \\(0 \neq v \in V\\) 가 존재할 때, 우리는 v 를 eigen-value \\(\lambda\\) 를 갖는 L의 eigen-vector 라 부른다.

(표기법 7.1.2) 앞으로 [\\(T \in \mathfrak{L}\mathfrak{M}\\)] 이라고 하면, 항상 [\\(T \in \mathfrak{L}(V,V)\\) 또는 \\(T \in \mathfrak{M}_{n,n}(F)\\)] 를 뜻하기로 약속한다. 이 때, \\(dim V = n\\) 이고, vector들은 u,v,w 등으로 표기하며, \\(I_{V} = I_{n} = I\\) 는 혼동하기로 한다. 물론 T가 행렬이면 \\(V = F^{n}\\) 으로 이해하고, \\(T = L_{T} \\)로 혼동한다. (따라서, \\(A \in \mathfrak{M}_{n,n}(F)\\)) 일 때, \\(ker A = ker L_{A}\\) 의 표기법도 가능.) 또, 혹시 모르니, \\(V \neq 0\\) 이라고 가정.

(재정의 7.1.3) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(Tv = \lambda v\\) 인 \\(\lambda \in F\\) 와 \\(0 \neq v \in V \\)가 존재하면, 우리는 v를 eigen-value \\(\lambda\\) 를 갖는 T의 eigen-vector 라고 부른다. 

(정의 7.1.7) \\(L \in \mathfrak{L} (V,V)\\) 일 때, V의 임의의 기저 \\(\mathfrak{B}\\) 를 골라 \\(det(L) = det(\left[L\right]_{\mathfrak{B}}^{\mathfrak{B}})\\) 로 정의하자.

(관찰 7.1.8) (정의 7.1.7) 의 \\(det(L)\\) 은 well-defined 되어있다.

(정의 7.1.9) \\(T \in \mathfrak{L} \mathfrak{M}\\) 이고, [T 혹은 \\(\left[T\right]_{\mathfrak{B}}^{\mathfrak{B}} \\)의 좌표] 를 \\(a_{ij}\\) 로 표기할 때, T 의 characteristic polynomial (특성다항식) \\(\phi_{T}(t) \in F\left[t\right]\\) 를 \\(\phi_{T}(t) = det(tI – T) = \begin{vmatrix} t-a_{11} & -a_{12} & -a_{13} & \cdots & -a_{1n} 



 -a_{21} & t-a_{22} & -a_{23} & \cdots & -a_{2n} 



 \vdots & \vdots & \vdots & \ddots & \vdots 



 -a_{n1} & -a_{n2} & -a_{n3} & \cdots & t-a_{nn} 



 \end{vmatrix}\\)

으로 정의한다. (이 때, \\(tI – T\\) 의 t는 마치 scalar 인 것처럼 생각한다.)

(관찰 7.1.10) Characteristic polynomial 은 similar matrix 의 invariant 이다. 따라서, \\(T \in \mathfrak{L} \mathfrak{M}\\)일 때, \\(\phi_{T}(t)\\) 는 well-defined 된다.

(명제 7.1.11) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(\lambda \in F \\)가 T의 eigen-value 이기 위한 필요충분조건은 \\(\phi_{T}(\lambda) = 0\\) 인 것이다.

(관찰 7.1.12) Trace, rank, determinant, characteristic 및 eigen-value 는 similar matrix 의 invariant 이다.

(정리 7.1.18) 모든 다항식 \\(f(t) \in \mathbb{C}\left[t\right]\\) 는 (\\(\mathbb{C}\\) 에서) 근 (root) 를 갖는다. (즉, 인수정리에 의해, \\(f(t) \in \mathbb{C}\left[t\right]\\) 는 \\(\mathbb{C}\\) 위의 일차식들의 곱으로 인수분해된다.)

(subsection 7.2.) Diagonalization

(정의 7.2.1) \\(A \in \mathfrak{M}_{n,n} (F)\\) 일 때, \\(A ~ D\\) 인 diagonal matrix \\(D \in \mathfrak{M}_{n,n} (F)\\) 가 존재하면, A를 diagonalizable matrix 라 부른다.

(관찰 7.2.2) \\(A \in \mathfrak{M}_{n,n}(F)\\) 일 때, 다음 조건들은 동치이다.

 A는 diagonalizable.

A 의 eigen-vector 들로 이루어진 \\(F^{n}\\) 의 basis 가 존재.

(정의 7.2.3) Linear operator \\(L \in \mathfrak{L}(V,V)\\) 의 (V의 임의의 기저 \\(\mathfrak{B}\\) 에 대한) 행렬 \\(\left[L\right]_{\mathfrak{B}}^{\mathfrak{B}}\\) 가 diagonalizable 이면, L 도 diagonalizable 이라고 말한다.

(관찰 7.2.4) Linear operator \\(L \in \mathfrak{L} (V,V)\\) 가 diagonalizable 이기 위한 필요충분조건은\\( \left[L\right]_{\mathfrak{B}}^{\mathfrak{B}}\\) 가 diagonalizable matrix 인 V의 기저 \\(\mathfrak{B}\\) 가 존재하는 것이다.

(재정의 7.2.5) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(\left[T\right]_{\mathfrak{B}}^{\mathfrak{B}}\\) 가 diagonal matrix 인 V 의 기저 \\(\mathfrak{B}\\) 가 존재하면 – 즉, T의 eigen-vector 들로 이루어진 V의 기저 \\(\mathfrak{B}\\) 가 존재한다면 – T는 diagonalizable 이라 말한다.

(명제 7.2.6) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(\phi_{T}(t)\\) 가 F에서 서로 다른 n-개의 root 를 가지면, T 는 diagonalizable이다. (물론, \\(dim V = n\\))

(보조정리 7.2.7) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(v_{1}, …, v_{k}\\) 가 T의 eigen-vector 라고 하자. 만약, \\(v_{i} 의 eigen-value \lambda_{i}\\) 들이 mutually distinct (즉, \\(\lambda_{i} \neq \lambda_{j} if i \neq j\\)) 이면, \\({v_{1}, …, v_{k}}\\) 는 일차독립이다.

(subsection 7.3.) Caley-Hamilton Theorem

(정의 7.3.2) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(\mathcal{I}_{T} = {f(t) \in F\left[t\right] | f(T) = 0}\\) 라고 정의하자.

(명제 7.3.4) \\(T \in \mathfrak{L} \mathfrak{M}\\) 이면, \\(\mathcal{I}_{T} \neq 0\\) 이다.

(Cayley-Hamilton Theorem) (정리 7.3.5) \\(T \in \mathfrak{L} \mathfrak{M}\\) 이면, \\(\phi_{T}(T) = 0\\) 이다. 즉, \\(\phi_{T}(t) \in \mathcal{I}_{T}\\) 이다.

(subsection 7.4) Minimal Polynomial

(정의 7.4.1) \\(T \in \mathfrak{L} \mathfrak{M}\\) 일 때, \\(\mathcal{I}_{T}\\) 의 non-zero polynomial 중에서 [최소의 degree 를 갖는 monic polynomia] 을 T의 minimal polynomial 이라고 부르고, \\(m_{\tau}(t)\\) 로 표기한다.

(관찰 7.4.2) \\(A, B \in \mathfrak{M}_{n,n}(F)\\) 이고 \\(A ~ B\\) 이면, \\(m_{A}(t) = m_{b}(t)\\) 이다. 즉, minimal polynomial 은 similar matrix 의 invariant 이다.

(정리 7.4.3) \\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때, T의 minimal polynomial 은 존재하고 하나뿐이다.

(따름정리 7.4.4)\\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때, \\(f(t) \in \mathcal{I}_{T}\\) 이면, \\(f(t)\\) 는 \\(m_{T}(t)\\) 의 배수이다. 

특별히 , \\(\phi_{T}(t)\\) 도 \\(m_{T}(t)\\) 의 배수이다.

(subsection 7.5) Direct sum 과 Eigen-space Decomposition

(정의 7.5.1) V가 벡터공간이고 U,W 가 V의 부분공간이라고 하자. 이 때, \\(U \cap W\\) 이면, \\(U + W = U \oplus W \\)로 표기하고, “\\(U+W\\) 는 \\(U,W\\) 의 direct sum이다” 라고 말한다.

(관찰 7.5.2) V가 vector space 이고, U,W 가 V 의 subspace 라고 할 때, 다음 조건은 동치이다.

\\(V = U \oplus W,\\)

\\(V = U + W\\) 이고 \\(U \cap W = 0\\)

이 떄, U 를 W의 direct complement 라고 부른다.

(관찰 7.5.3) V가 vector space 이고, U,W 가 V의 subspace 라고 할 때, 다음은 동치이다.

\\(V = U \oplus W\\)

V 의 모든 vector v 는 \\(u + w\\) (단, \\(u \in U\\), \\(w \in W\\)) 의 꼴로 쓸 수 있고, 그 방법은 하나뿐이다.

\\(V = U + W\\) 이고, V의 zero vector 0 를 \\(u + w\\) (단, \\(u \in U\\), \\(w \in W\\) ) 의 꼴로 쓰는 방법은 하나뿐이다.

(관찰 7.5.4.) V가 f.d.v.s. 이고, \\(U, W \le V\\) 일 때, 다음 조건은 동치이다.

 \\(V = U \oplus W,\\)

\\(dim V = dim U + dim W\\) 이고, \\(U \cap W = 0.\\)

(관찰 7.5.6.) V가 벡터공간이고 \\(\mathfrak{B}_{1}, \mathfrak{B}_{2}\\) 가 각각 V의 subspace \\(W_{1}, W_{2}\\) 의 기저라고 하면, 다음 조건은 동치이다.

 \\(V = W_{1} \oplus W_{2}\\).

\\(\mathfrak{B} = \mathfrak{B}_{1} \mathfrak{U} \mathfrak{B}_{2}\\) 는 V의 basis. (단, \\(\mathfrak{U}\\) 는 disjoint union 을 의미한다.)

(정의 7.5.7) V가 vector space 이고, \\(W_{1}, …, W_{k}\\) 가 V의 subspace 라고 하자. 이 때, \\(W_{1} + \cdots + W_{k}\\) 의 vector v를 \\(w_{1}, + \cdots + w_{k}\\) (단, \\(w_{i} \in W_{i}\\)) 의 꼴로 표현하는 방법이 하나뿐이면, \\(\sum_{i = 1}^{k} W_{i} = W_{1} + \cdots + W_{k} = W_{1} \oplus \cdots \oplus W_{k} = \bigoplus_{i = 1}^{k} W_{i}\\) 로 표기하고, 이런 경우에 “\\(\sum_{i = 1}^{k} W_{i}\\) 는 \\(W_{1}, …, W_{k}\\) 의 direct sum 이다” 라고 말한다. 또, 각각의 \\(W_{1}, …, W_{k}\\) 는 \\(\oplus_{i=1}^{k}\\) 의 direct summand 라고 말한다.

(관찰 7.5.9) V가 vector space 이고 \\(W_{1}, …, W_{k}\\) 가 V의 subspace 라고 할 때, 다음은 동치이다.

\\(V = W_{1} \oplus \cdots \oplus W_{k}\\) .

V 의 모든 vector v 는 \\(w_{1} + \cdots + w_{k}\\) (단, \\(w_{i} \in W_{i}\\)) 의 꼴로 쓸 수 있고, 그 방법은 하나뿐이다.

\\(V = W_{1} + \cdots + W_{k}\\) 이고, V의 zero vector 0 을 \\(w_{1} + \cdots + w_{k}\\) (단, \\(w_{i} \in W_{i}\\)) 의 꼴로 쓰는 방법은 하나 뿐이다.

(관찰 7.5.11) \\(\mathfrak{B}_{i}\\) 가 각각 V의 subspace \\(W_{i}\\) (단, \\(i = 1,…,k\\)) 의 기저라고 할 때, 다음 조건은 동치이다.

\\( V = W_{1} \oplus \cdots \oplus W_{k}\\)

\\(\mathfrak{B} = \mathfrak{B}_{1} \mathfrak{U} \cdots \mathfrak{U} \mathfrak{B}_{k}\\) 는 V의 basis. (이 때, \\(\mathfrak{U}\\) 는 mutually disjoint union 을 의미한다. 즉\\( \mathfrak{B}_{i} \cap \mathfrak{B}_{j} = \empty if i \neq j\\) 인 union 이라는 뜻이다.)

(정의 7.5.15.) \\(T \in \mathfrak{L}\mathfrak{M}\\)이고, \\(\lambda \in F\\) 일 때, \\(V_{\lambda} = V_{T,\lambda} = {v \in V | Tv = \lambda v}\\) 로 표기하고, \\(V_{\lambda} = V_{T,\lambda}\\) 를 \\(\lambda\\) 에 대응하는 T의 eigen-space 라고 부른다.

(관찰 7.5.17) \\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때, 다음은 동치이다.

T는 diagonalizable.

\\(V = V_{\lambda_{1}} \oplus \cdots \oplus V_{\lambda_{k}}\\) 인, T의 (서로 다른) eigen-value \\(\lambda_{1}, …, \lambda_{k}\\) 존재.

(정의 7.5.18) 위 (관찰 7.5.17) 의 \\(V = V_{\lambda_{1}} \oplus \cdots \oplus V_{\lambda_{k}}\\) 를 diagonalizable T 에 관한 (V의) eigen-space decomposition 이라고 부른다.

