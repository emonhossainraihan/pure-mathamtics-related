---
layout: post
title : (Linear Algebra) Linear Mapping 선형 사상
date : 2018-01-19 13:51:06 +0900
---
(Section 4) 선형사상

(subsection 4.1) Linear map

(정의 4.1.1) V,W 가 F-위의 벡터공간일 때, 함수 \\(L : V \to W\\) 가 다음 조건을 만족하면 L을 linear map (선형사상, linear mapping, linear transformation from V into W) 라고 부른다. 

\\(L(v_{1} + v_{2}) = L(v_{1}) + L(v_{2}) (v_{1}, v_{2} \in V)\\)

\\(L(av) = aL(v) ( v \in V , a \in F)\\)

(관찰 4.1.2) \\(L : V \to W\\) 가 linear map 일 때,

\\( L(0) = 0\\)

\\(v \in V\\) 이면, \\(L(-v) = -L(v)\\)

\\(u,v \in V\\) 이면, \\(L(u-v) = L(u) – L(v)\\)

(정의 4.1.3) \\(L : V \to W\\) 가 linear map일 때,

L 이 injective (단사) 이면, L을 monomorphism 이라 부른다.

L 이 surjective (전사) 이면, L 을 epimorphism 이라고 부른다.

L 이 bijective (전단사) 이면, L을 isomorphism 이라고 부른다.

V = W 이면, L 을 endomorphism, 혹은 Linear operator, 혹은 간단히 operator 라 부른다.

Bijective endomorphism 은 automorphism 이라고 부른다.

(관찰 4.1.4) \\(L : V \to W\\) 가 linear map 일 때, 다음 조건은 동치이다.

L 은 isomorphism.

[\\(M \bullet L = I_{V}\\) 이고\\( L \bullet M = I_{W}\\) ] 인 linear map\\(M : W \to V\\) 가 존재.

(정의 4.1.5)\\( L : V \to W\\) 가 linear map 일 때,

\\(ker L = L^{-1} (0) = {v \in V | L(v) = 0}\\) 을 L 의 kernel 이라고 부른다.

\\(im L = L(V) = {L(v) | v \in V}\\) 를 L의 image 라고 부른다.

(관찰 4.1.6) \\(L : V \to W\\) 가 linear map 이면, \\(ker L \le V , im L \le W\\) 이다.

(관찰 4.1.8) \\(L : V \to W\\) 가 linear map 일 때, 다음 조건은 동치이다.

L 은 monomorphism 이다.

\\(u,v, \in V\\) 이고 \\(Lu = Lv\\) 이면, \\(u = v \\)이다.

 \\(v \in V\\) 이고\\(Lv = L0\\) 이면, \\(v = 0\\) 이다.

 \\(ker L = 0\\) 이다.

(관찰 4.1.9)\\( L : V \to W\\) 가 linear 이고, \\(S \subseteq V\\) 이면,\\( L\langle S \rangle = \langle LS \rangle\\) 이다.

(관찰 4.1.12) \\(L : V \to W\\) 가 linear map 일 때, 다음 조건은 동치이다.

 L 은 isomorphism 이다.

 L 은 basis 를 basis 로 옮긴다.

(표기법 4.1.13) \\(U \le V\\) 이고 \\(v \in V\\) 일 때, \\(v + U = {v + u | u \in U}\\) 의 notation 을 쓴다.

(subsection 4.2) Linear map 의 보기

(관찰 4.2.7) 두 선형사상의 합성은 다시 선형사상이다. 즉, \\(M : U \to V\\) 와 \\(L : V \to W\\) 가 linear 이면, \\(L \bullet M : U \to W\\) 도 linear 이다.

(정의 4.2.10) \\(A \in \mathfrak{M}_{m,n} (F)\\) 일 때, \\(L_{A} : F^{n} \to F^{m}\\) 을 \\(L_{A}(X) = AX (X \in F^{n})\\) 으로 정의하면, \\(L_{A}\\) 가 linear map 인 것은 자명하다. \\(L_{A}\\) 를 matrix A 에 대응하는 linear map 이라 부른다.

(subsection 4.3) Dimension Theorem

(Dimension Theorem) (정리 4.3.1) V, W 가 f.d.v.s 이고, \\(L : V \to W\\) 가 linear map 이면, dim V = dim ker L + dim im L 이다.

(따름정리 4.3.2) V,W 가 f.d.v.s. 이고 \\(dim V = dim W\\) 일 때, \\(L : V \to W\\) 가 linear map 이면 다음 세 조건은 동치이다.

L 은 isomorphism. (즉, L은 bijection)

L 은 monomorphism (즉, L 은 injection)

L 은 epimorphism (즉, L 은 surjection)

(Pigeonhole Principle) (정리 4.3.4) X,Y 가 (non-empty) finite set 이고 \\(|X| = |Y|\\) 일 때, \\(f : X \to Y\\) 가 함수이면 다음 세 조건은 동치이다.

f는 bijection.

f 는 injection.

f 는 surjection.

(따름정리 4.3.6) V,W 가 f.d.v.s. 이고 \\(L : V \to W\\) 가 linear map 일 때,

 L 이 monomorphism 이면, \\(dim V \le dim W\\).

L 이 epimorphism 이면, \\(dim V \ge dim W\\).

(subsection 4.4) Rank Theorem

(정의 4.4.1) \\(A \in \mathfrak{M}_{m,n} (F)\\) 일 때, A 의 i-번째 row 는 \\(\left[ A \right]_{i}\\) 로 표기하고, A의 j-번째 column 은 \\(\left[ A \right]^{j}\\) 로 표기한다. \\(\mathfrak{M}_{1,n}(F)\\) 의 부분공간 \\(\langle \left[ A\right]_{1}, …, \left[ A \right]_{m} \rangle\\) 을 A의 rowspace 라 부른다. A 의 row space 의 dimension 은 A 의 row rank 라 부른다. 마찬가지로, A의 column space 는 \\(F^{m}\\) 의 부분공간 \\(\langle \left[ A \right]^{1} , …, \left[ A \right]^{n} \rangle\\) 이고, 그 dimension 은 A의 column rank 라고 부른다.

(관찰 4.4.3) 행렬 A에 elementary row operation 을 수행해도 A의 row space 는 변화하지 않는다. 따라서, [A 로부터 얻어지는 row-reduced echelon form 의 row space] 와 [A 의 row space ] 는 같다.

(Rank Theorem) (정리 4.4.4) \\(A \in \mathfrak{M}_{m,n} (F)\\) 이면, [row rank of A] = [column rank of A] 이다.

(정의 4.4.5) \\(A \in \mathfrak{M}_{m,n}(F)\\) 일 때, A의 row rank (혹은 column rank) 를 간단히 A의 rank 라 부르고 rk(A) 로 표기한다.

(따름정리 4.4.6) \\(A \in \mathfrak{M}_{m,n} (F)\\) 일 때, homogeneous linear equation (*) AX = 0 의 solution space 의 dimension 은 n – rk(A) 이다.

(따름정리 4.4.7) 행렬 A에 elementary row operation 을 수행해도 (A의 column space 는 변화하지만) A의 column rank 는 변화하지 않는다.

(subsection 4.5) Linear extension theorem

(관찰 4.5.1) \\(\mathfrak{B} = {v_{1}, …, v_{n}}\\) 이 V의 basis 이고 \\(L, M : V \to W\\) 가 linear 일 때, [\\(L(v_{i}) = M(v_{i})\\) for all i] 이면, \\(L = M\\) 이다. 즉, 선형사상은 기저에서의 값이 결정한다.

(Linear extension theorem) (정리 4.5.3) \\(\mathfrak{B}\\) 가 V의 basis 이고\\( f : \mathfrak{B} \to W\\) 가 함수이면, \\(L|_{\mathfrak{B}} = f\\) 인 linear map\\( L : V \to W\\) 가 유일하게 존재한다.

(Classification of Vector Spaces) (따름정리 4.5.10) V,W 가 F-vector space 일 때, 다음은 동치이다.

\\(V \approx W\\)

\\(dim V = dim W\\)

(Classification of f.d.v.s) (따름정리 4.5.11) f.d.v.s. V 의 dimension 이 n 이면, \\(V \approx F^{n}\\) 이다.
