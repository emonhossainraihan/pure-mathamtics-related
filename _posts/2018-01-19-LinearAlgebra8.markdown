---
layout: post
title : [Linear Algebra] Decomposition theorem 분해정리
date : 2018-01-19 13:51:10 +0900
---
(Section 8) 분해정리

(subsection 8.1) polynomial

(명제 8.1.4) \\(F\left[t\right]\\) 의 polynomial \\(f_{1}(t), f_{2}(t), … , f_{k}(t)\\) 의 최대공약수를 \\(d(t)\\) 라고 하면, \\(d(t) = g_{1}(t) f_{1}(t) g_{2}(t) f_{2}(t) + \cdots + g_{k}(t) f_{k}(t)\\) 가 성립하는 \\(F\left[t\right]\\) 의 polynomial \\(g_{1}(t), g_{2}(t), … , g_{k}(t)\\) 가 존재한다.

(명제 8.1.5) \\(T \in \mathfrak{L}\mathfrak{M}\\) 의 characteristic polynomial \\(\phi_{T}(t)\\) 와 minimal polynomial \\(m_{T}(t)\\) 의 [F-위의 monic irreducible divisor 의 집합] 은 같다.

(표기법 8.1.10)\\(f(t) \in \mathbb{C} \left[t\right]\\) 가\\( f(t) = \alpha_{n}t^{n} + \alpha_{n-1}t^{n-1} + \cdots + \alpha_{1}t + \alpha_{0}\\) (단, \\(\alpha_{0} , …, \alpha_{n} \in \mathbb{C}\\)) 로 주어졌을 때, \\(\hat{F}(t) \in \mathbb{C} \left[t\right] 를 \hat{f}(t) = \hat{\alpha_{n}} t^{n} + \hat{\alpha_{n-1}} t^{n-1} + \cdots + \hat{\alpha_{1}} t + \hat{\alpha_{0}}\\) 으로 정의한다. 또, \\(A = (\alpha_{ij}) \in \mathfrak{M}_{m,n}(\mathbb{C})\\) 일 때, \\(\hat{A} = (\hat{\alpha_{ij}}) \in \mathfrak{M}_{m,n} (\mathbb{C})\\) 로 정의한다.

(관찰 8.1.14.) \\(A \in \mathfrak{M}_{n,n}(\mathbb{R})\\) 을 real matrix 로 생각하나 complex matrix 로 생각하나 characteristic polynomial 과 minimal polynomial 은 변함이 없다.

(subsection 8.2) T -invariant Subspace

(정의 8.2.1) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이고 \\(W \le V\\) 일 때, \\(T(W) \le W\\) 이면 – 즉  \\(T |_{W} : W \to W\\) 가 의미가 있으면 – 우리는 W를 V의 T-invatiant subspace 라고 부른다. 혹은, W 는 “T-stable” 이다 라고 말한다. (만약, \\(T \in \mathfrak{M}_{n,n}(F)\\) 이면, \\(T = L_{T}, V = F^{n}\\)으로 이해한다.)

(관찰 8.2.9) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이고 \\(f(t) \in F\left[t\right]\\) 라고 하면 다음이 성립한다.

ker T 와 im T 는 T-invariant.

ker f(T) 와 im f(T) 는 T-invariant.

(subsection 8.3) Primary Decomposition Theorem

(표기법 8.3.3) \\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때, \\(\phi_{T}(t) = p_{1}(t)^{e_{1}} p_{2}(t)^{e_{2}} \cdots p_{k}(t)^{e_{k}}, m_{T}(t) = p_{1}(t)^{f_{1}} p_{2}(t)^{f_{2}} \cdots p_{k}(t)^{f_{k}}\\) 로 (F-위에서) 인수분해된다고 하자. 이 때 \\(p_{i}(t)\\) 들은 F[t] 의 relatively prime monic irreducible polynomial 이고 \\(1 \le f_{i} \le e_{i}\\) 이다. 또, \\(W_{i} = ker p_{i}(T)^{e_{i}} , T_{i} = T|_{W_{i}} , (i = 1,…,k)\\) 로 간단히 표기하기로 한다. \\(W_{i}\\) 가 T-invariant subspace 이다.

(Primary Decomposition Theorem) (정리 8.3.4) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이면, \\(V = ker p_{1}(T)^{e_{1}} \oplus ker p_{2} (T)^{e_{2}} \oplus \cdots \oplus ker p_{k}(T)^{e_{k}} = ker p_{1}(T)^{f_{1}} \oplus ker p_{2}(T)^{f_{2}} \oplus \cdots \oplus ker p_{k}(T)^{f_{k}}\\) 로 분해할 수 있다. 그리고 모든 \\(i = 1, …, k\\) 에 대해, 다음이 성립한다.

 \\(W_{i} = ker p_{i}(T)^{e_{i}} = ker p_{i}(T)^{f_{i}}\\).

\\(m_{T_{i}}(t) = p_{i}(t)^{f_{i}}\\) .

\\(\phi_{T_{i}}(t) = p_{i}(t)^{e_{i}}\\) . (따라서, \\(dim W_{i} = e_{i} \cdot deg(p_{i})\\).) 

(보조정리 8.3.5.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때,\\( f(t), g(t) \in F\left[t\right]\\) 는 monic 이고 relatively prime 이라고 하자. 만약 \\(\xi(t) = f(t) g(t) \in \mathcal{I}_{T}\\) 이면, \\(V = ker f(T) \oplus ker g(T)\\) 로 쓸 수 있다. 이때, \\(U = ker f(T), W = ker g(T) \\)로 간단히 표기하면,

\\(\xi(t) = m_{T} (t)\\) 일 때에는, \\(m_{T|v}(t) = f(t)\\) 이고 \\(m_{T|w} (t) = g(t)\\)

\\(\xi(t) = \phi_{T}(t)\\) 일 때에는, \\(\phi_{T|v} (t) = f(t)\\) 이고 \\(\phi_{T|w} (t) = g(t)\\) .

(subsection 8.4.) Diagonalizability

(따름정리 8.4.1.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이 diagonalizable일 필요충분조건은 T의 minimal polynomial \\(m_{T}(t)\\) 가 (F-위에서) 일차식들로 인수분해되고 multiple root 을 갖지 않는 것이다. (즉, 모든\\( i = 1,…,k\\) 에 대하여, \\(deg(p_{i}) = 1\\) 이고, \\(f_{i} = 1\\) 인 것이다.)

(따름정리 8.4.2.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이 diagonalizable 이고 W가 V의 T-invariant sub-space 이면, \\(T|_{W}\\) 도 diagonalizable 이다.

(정의 8.4.3.) \\(T , S \in \mathfrak{L}\mathfrak{M}\\) 일 때, V의 하나의 기저 \\(\mathfrak{B}\\) 에 관해 \\(\left[T\right]_{\mathfrak{B}}^{\mathfrak{B}}\\) 와 \\(\left[S\right]_{\mathfrak{B}}^{\mathfrak{B}}\\) 가 모두 대각행렬이면, 우리는 T와 S가 simultaneously diagonalizable 하다고 말한다. 여러 개의 linear operator 의 경우에도 마찬가지로 정의한다.

(명제 8.4.4.) \\(T , S \in \mathfrak{L}\mathfrak{M}\\)이고, 조건 \\(TS = ST\\) 를 만족한다고 하자. 이 때, T와 S가 각각 diagonalizable 이면 T,S 는 simultaneously diagonalizable 이다.

(subsection 8.5) T-Cyclic Subspace

(정의 8.5.1.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때, \\(V = \lbracef(T) v | f(t) \in F\left[t\right]\rbrace\\) 인 \\(v \in V\\) 가 존재하면, V를 T-cyclic space 라 부르고, \\(V = F\left[t\right] v = \lbracef(T) v | f(t) \in F\left[t\right]\rbrace\\) 로 표기한다.

(명제 8.5.4.) \\(T \in \mathfrak{L}\mathfrak{M} V = F\left[t\right] v\\) 가 T-cyclic 이면, 다음이 성립한다. 

\\(\phi_{T}(t) = m_{T}(t).\\)

\\(\mathfrak{B} = {v, Tv, T^{2}v, …, T^{n-1} v}\\) 는 V의 기저. 단,\\( n = dim V = deg (m_{T})\\) . 

\\(\left[T\right]_{\mathfrak{B}}^{\mathfrak{B}}\\) 는 \\(m_{T}(t)\\) 에 대응하는 companion matrix.

(정의 8.5.7.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이고, W는 V의 T-invariant subspace 라고 하자. 이 때 W가 \\((T|_{W})\\)-cyclic 이면 , W 를 V의 T-cyclic subspace 라고 부른다.

(정의 8.5.9.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이고, \\(0 \neq w \in V\\) 일 때, \\(F\left[t\right] w = {f(T) w | f(t) \in F\left[t\right]} = \langle w , Tw , T^{2}w, … \rangle\\) 로 표기하고, \\(F\left[t\right] w\\) 를 =[T-cyclic subspace of V generaged by w] 라고 부른다. 

\\(W = F\left[t\right] w\\) 로 놓을 때, \\(m_{w}(t) = m_{(T|_{W})} (t)\\) 로 간략히 표기하고, \\(m_{w}(t)\\) 를 [minimal polynomial of w in V] 라고 부른다.

(관찰 8.5.11.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 이고, \\(0 \neq w \in V\\) 일 때, \\(W = F\left[t\right]w\\) 라고 놓으면, 다음이 성립한다.

\\( m_{w}(T) = \phi_{T|w} (t)\\).

\\(\mathfrak{C} = {w, Tw, …, T^{m-1} w}\\) 는 W의 기저. 단,\\( m = dim W = deg(m_{w})\\) .

\\(\left[T|_{W}\right]_{\mathfrak{C}}^{\mathfrak{C}}\\) 는 \\(m_{w}(t)\\) 에 대응하는 companion matrix.

\\(m_{T} (t)\\) 는 \\(m_{w} (t)\\) 의 배수.

(subsection 8.6) Cyclic Decomposition Theorem

(Cyclic Decomposition Theorem) (정리 8.6.1.) \\(T \in \mathfrak{L}\mathfrak{M}\\) 일 때, \\(m_{T} (t) = p(t)^{f}\\) 라고 가정하자. 이 때 \\(p(t)\\) 는 \\(F\left[t\right]\\) 의 monic irreducible polynomial 이다. 그러면, \\(V = U_{1} \oplus U_{2} \oplus \cdots \oplus U_{h}\\) 인 V의 (T-invariant) T-cyclic subspace \\(U_{1}, …, U_{h}\\) 가 존재한다. 그리고, \\(\phi_{T|_{U_{j}}}(t) = m_{T|_{U_{j}}}(t) = p(t)^{r_{j}} (j = 1,…,h)\\) 로 표기할 떄, 다음 조건 \\(f = r_{1} \ge r_{2} \ge \cdots \ge r_{h} \ge 1\\) 을 만족하는 자연수 h 와 \\(r_{1} , … , r_{h}\\) 는 유일하게 결정된다.

(따름정리 8.6.2) 두 square matrix \\(A, B \in \mathfrak{M}_{n,n}(F)\\) 에 대해, \\(A ~ B\\) 인지 여부를 결정해주는 invariant 들의 집합은 \\({p_{i}(t), h_{i}, r_{ij}}\\( 이다.
