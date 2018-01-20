---



layout: post



title : 노음공간



date : 2018-01-20 08:52:54 +0900



---

(section 6) 노음공간

(subsection 6.1) 쌍대공간

(정의) 두 노음공간 사이에 정의된 선형사상 T : X \to Y 에 대하여 \lVert T\rVert = sup{\lVert T(x) \rVert : x \in X, \lVert x \rVert \le 1} 이라 정의하자. 만일 \lVert T\rVert < \infty 이면 T 를 유계선형사상이라 부르고 \lVert T\rVert 를 T의 노음이라 한다.

선형사상 T : X \to Y 의 노음이란 X의 단위공 {x \in X : \lVert x \rVert \le 1} 의 치역이 Y에서 얼마나 늘어나는가 재는 것이다.

(명제 6.1.1) 노음공간 사이의 선형사상 T : X \to Y 에 대하여 다음은 동치이다.

T가 유계사상이다

T가 연속이다.

T가 한 점 x_{0} \in X 에서 연속이다.

(명제 6.1.2.2) 임의의 노음공간 X 에서 Y 로 가는 유계선형사상 전체의 집합 B(X,Y) 는 노음공간이 된다. 만일 Y가 바나하공간이라면 B(X,Y) 도 바나하공간이다.

(정의) 그 치역이 스칼라 \mathbb{C} 인 선형사상을 선형범함수라 하고, X에서 정의된 유계선형범함수 전체의 노음공간을 X^{*} 라 표시한다. 즉, X* = B(X,\mathbb{C}) 이다. X* 은 항상 바나하공간이 되는데, X^{*}를 X의 쌍대공간이라 한다.

(정의) 양측도 (X, \mu) 가 주어지면 임의의 q \in [1,\infty]에 대하여 g \mapsto \phi_{g} : L^{q} (\mu) \to L^{p}(\mu)^{*} 가 선형사상임이 바로 확인되는데, 이 사상이 노음을 보존한다는 것을 보였다. (단,p = 1, q = \infty 인 경우 (X, \mu) 가 \sigma-유한이라 가정한다) 이렇게 노음을 보존하는 선형사상을 등거리사상이라 부른다.

등거리사상은 단사사상이다.

(정리 6.1.3) 만일 1 \le p < \infty 이면 g \mapsto \phi_{g} : \mathcal{l}^{q} \to (\mathcal{l}^{p})^{*} 은 전단사 등거리사상이다. (단, p,q 는 켤레지수) 

(한-바나하)(정리 6.1.4) 노음공간 X와 그 부분공간 Y가 주어져있다. 그러면 임의의 \psi \in Y^{*} 에 대하여 다음 성질 \phi |_{Y} = \psi,   \lVert \phi \rVert = \lVert \psi \rVert 을 만족하는 \phi \in X^{*} 가 존재한다.

(따름정리 6.1.5) 노음공간 X의 점 x 가 x \neq 0 이면 \phi(x) = \lVert x \rVert 이고 \lVert \phi \rVert 인 \phi \in X^{*} 가 존재한다.

따라서, 노음공간 X는 항상 X^{**} 의 부분공간이다.

(정의) 만일 x \mapsto T_{x} : X \to X^{**} 가 전사사상이면 X를 반사공간이라 부른다. 

그 예로 바나하공간 \mathcal{l}^{p} (1 < p < \infty) 는 반사공간이다.

부분집합 Y 의 닫힘은 \bar{Y}로 표시한다.

(따름정리 6.1.6) 노음공간 X의 부분공간 Y와 한 점 x \in X 에 대하여 다음은 동치이다.

x \in \bar{Y} 이다.

\phi \in X^{*} 이고 \phi |_{Y} = 0 이면 \phi (x) = 0 이다.

(subsection 6.2) 바나하공간의 선형사상

(정의)거리공간 (X,d) 의 점 x \in X 와 양수 r > 0 에 대하여 x 의 근방을 N_{X} (x,r) = {y \in X : d(x,y) < r} 로 정의하고, N(x,r)로 쓴다. X가 노음공간일 때 0 의 근방 N_{X}(0,r) 은 X_{r} 이라 쓴다.

(베르) (정리 6.2.1) 완비거리공간 X의 닫힌집합열 \langle C_{n} \rangle 의 합집합이 전체공간이 되면, 그 중 한 닫힌 집합은 열린집합을 품는다.

(따름정리 6.2.2) 완비거리공간의 조밀 열린집합열의 교집합은 비어있지 않다.

(열린사상정리)(정리 6.2.3) 바나하공간 사이에 정의된 유계선형사상 T : X \to Y 가 전사사상이라 하자. 그러면 T(X_{1}) \supset Y_{delta} 인 양수 \delta >0 가 존재한다.

(따름정리 6.2.4) 바나하공간 사이에 정의된 전사 유계선형사상 T : X \to Y 는 항상 열린사상이다.

(따름정리 6.2.5) 바나하공간 사이에 정의된 유계선형사상 T : X \to Y 가 전단사사상이면 그 역사상 T^{-1} : Y \to X 도 유계사상이다.

(정의) 각 n = 1,2, … 에 대하여 D_{n}(T) = \sum_{k = -n}^{n} u_{k}(t) = \frac{sin(n+\frac{1}{2}) t}{sin \frac{1}{2} t} , t \in \mathbb{T} 라 정의하자. 함수열 \langle D_{n} \rangle 은 디리끌렛 핵이라 불린다.

(명제) 주기함수의 푸리에 변환 L^{1}(\mathbb{T}) \to c_{0}(\mathbb{Z}) 이 전사사상이 아니다.

(닫힌그래프정리)(정리 6.2.6) 바나하공간 사이의 선형사상 T : X \to Y 가 조건 x_{n} \in X, lim_{n \to \infty} x_{n} = x, lim_{n \to \infty} T(x_{n}) = y \implies T(x) = y 를 만족하면 T는 유계선형사상이다.

(고른유계원칙) (바나하-쉬타인하우스 정리) (정리 6.2.7) 바나하공간 X 에서 노음공간 Y 로 가는 유계선형사상들의 모임 {T_{\alpha} : \alpha \in A} 가 주어져있다. 만일 각 x \in X 에 대하여 M(x) = \sup{\lVert T_{\alpha} (x) \rVert: \alpha \in A} < \infty 이면 \sup{\lVert T_{\alpha} \rVert: \alpha \in A} < \infty 이다.

(따름정리 6.2.8) 바나하공간 X에서 노음공간 Y로 가는 유계선형사상열 \langle T_{n} \rangle 이 있는데, 각 x \in X 에 대하여 Y 의 수열 \langle T_{n} (x) \rangle 이 수렴한다고 가정하자. 이 때, T(x) = \lim_{n \to \infty} T_{n} (x) 라 두면 T : X \to Y 는 유계선형사상이다.

(명제) 푸리에 급수가 점별수렴하지 않는 연속함수가 존재한다.

(subsection 6.3) 힐버트공간

복소벡터공간 X가 있을 때, 함수 (x,y) \mapsto \langle x,y \rangle : X \times X \to \mathbb{C} 가 다음 성질들을 만족하면 이를 내적이라 하고, 내적이 정의되어있는 벡터공간을 내적공간이라 한다.

각 y \in Y 에 대하여 x \mapsto \langle x,y \rangle : X \to \mathbb{C} 가 선형범함수이다.

각 x, y \in X 에 대하여 \langle x,y \rangle = \bar{\langle y,x \rangle}

각 x \in X 에 대하여 \langle x,x \rangle \ge 0 이다.

x = 0 \iff \langle x,x \rangle = 0 이다.

(정의) 부등식 | \langle x,y \rangle |^{2} \le \langle x,x \rangle \langle x,y \rangle , x, y \in X 를 얻는데, 이를 쉬바르츠 부등식이라 한다.

(명제) 각 x \in X 에 대하여 \lVert x \rVert = \langle x,x \rangle^{1/2} 라 정의하면 x \mapsto \lVert x \rVert 가 노음이 된다. 따라서 임의의 내적공간은 노음공간이 된다.

(정의) 완비내적공간을 힐버트 공간이라 한다.

(정의) 내적공간의 노음은 등식 \lVert x+y \rVert^{2} + \lVert x-y \rVert^{2} = 2 \lVert x \rVert^{2} + 2 \lVert y \rVert^{2} 을 만족하는데, 이를 나란히꼴 등식이라 부른다.

(명제) 임의의 y \in H 에 대하여 \phi_{y} : X \mapsto \langle x,y \rangle , x \in H 는 유계선형범함수이고, \lVert \phi_{y} \rVert = \lVert y \rVert 이다. 따라서 y \mapsto \phi_{y} : X \to X^{*} 는 등거리 단사사상이다. 선형사상은 아니다. (정리 6.3.3) 에 의해 전사사상이다.

(정의) 각 \alpha \in \mathbb{C} 에 대하여 \phi_{\alpha y} = \bar{\alpha} \phi_{y} 가 되는 사상을 켤레선형사상이라 부른다.

(정리 6.3.1) 힐버트 공간 H의 닫힌볼록집합 C 와 x_{0} \in H \setminus C 에 대하여 d = inf{\lVert x_{0} – y \rVert : y \in C} 라 두면 \lVert x_{0} – y_{0} \rVert = d 인 y_{0} \in C 가 유일하게 존재한다.

(정의) 내적공간의 두 벡터 x,y 가 \langle x, y \rangle = 0 일 때, x 와 y가 서로 수직이라고 하고 x \perp y 라 쓴다. 부분집합 E의 임의의 벡터와 수직인 벡터를 모두 모은 집합을 E^{\perp} 라 표시한다.

(따름정리 6.3.2) 힐버트공간 H의 부분공간 E가 닫힌 진부분공간이라면 E^{\perp} \supsetneqq {0} 이다. 

(정리 6.3.3) 힐버트공간 H 에서 임의의 y \in H 에 대하여 \phi_{y} : X \mapsto \langle x,y \rangle , x \in H, y \mapsto \phi_{y} : X \to X^{*} 에 의해 정의된 사상 y \mapsto \phi_{y} 는 전단사 등거리 켤레선형사상이다.

(정의) 내적공간 H의 부분집합 {u_{\alpha} : \alpha \in A} 가 다음 조건을 만족할 때, 이를 정규직교집합이라 부르고, 이에 의하여 생성된 H의 부분공간을 P_{A} 라 쓰자.

\langle u_{\alpha} , u_{\beta} \rangle = \begin{cases} 1 & \alpha = \beta \\  0 & \alpha \neq \beta \end{cases}

(명제 6.3.4) 내적공간 H의 정규직교집합 {u_{\alpha} : \alpha \in A} 의 유한부분집합 {u_{\alpha} : \alpha \in F} 가 주어져 있다. 이 때, 임의의 고정된 x \in H 에 대하여 부등식 \bigg\| x - \sum_{\alpha \in F} \langle x, u_{\alpha} \rangle u_{\alpha} \bigg\| \le \| x – y \| , y \in P_{F} 이 성립하고, y = \sum_{\alpha \in F} \langle x, u_{\alpha} \rangle u_{\alpha} 일 때에 한하여 등호가 성립한다. 

또한, 각 x \in H 에 대하여 부등식 \sum_{\alpha \in F} | \langle x, u_{\alpha} \rangle |^{2} \le \| x \|^{2} 이 성립한다.

(베셀 부등식) (따름정리 6.3.5) 내적공간 H에 주어진 임의의 정규직교집합 {u_{\alpha} : \alpha \in A } 에 대하여, 부등식 \sum_{\alpha \in A} | \langle x, u_{\alpha} \rangle |^{2} \le \| x \|^{2}, x \in H 이 성립한다.

(정리 6.3.6) 힐버트공간 H 의 정규직교집합 \mathfrak{U} = {u_{\alpha} : \alpha \in A } 에 대하여 다음은 동치이다.

각 x \in H 에 대하여 등식 \sum_{\alpha \in A} | \langle x, u_{\alpha} \rangle |^{2} = \| x \|^{2} 이 성립한다.

각 x, y \in H 에 대하여 등식 \sum_{\alpha \in A} \langle x, u_{\alpha} \rangle \bar{\langle y, u_{\alpha} \rangle} = \langle x,y \rangle 이 성립한다.

만일 \mathfrak{V} \supset \mathfrak{U} 인 정규직교집합 \mathfrak{V} 이 있으면 \mathfrak{V} = \mathfrak{U} 이다.

벡터공간 P_{A} 가 H 안에서 조밀하다.

(정의) \sum_{\alpha \in A} \langle x, u_{\alpha} \rangle \bar{\langle y, u_{\alpha} \rangle} = \langle x,y \rangle 는 파시발 등식이라 불린다.

(정의) (정리 6.3.6) 에 있는 조건들을 만족하는 정규직교집합 {u_{\alpha} : \alpha \in A } 을 힐버트공간 H 의 정규직교기저라 한다. 

(정의) 힐버트공간 사이에 정의되어 내적을 보존하는 선형사상을 힐버트공간 동형사상이라 부른다.

(정리 6.3.7) 힐버트공간 H의 정규직교기저 {u_{\alpha} : \alpha \in A } 에 대하여 \{Phi} :x \mapsto \hat{x} : H \to \mathcal{l}^{2} (A) 는 전단사 힐버트공간 동형사상이다.

(명제) u_{n}(t) = e^{int} 로 정의한 {u_{n} : n \in \mathbb{Z}} 는 L^{2}(\mathbb{T}) 의 정규직교기저가 된다.

등식 \sum_{n= -\infty}^{\infty} \hat{f}(n) \bar{\hat{g}(n)} = \frac{1}{2 \pi} \int_{-\pi}^{\pi} f(t) \bar{g(t)} dt, f, g \in L^{2}(\mathbb{T}) 도 역시 파시발 등식이라 부른다.

등식 \lim_{n \to \infty} \bigg\| f - \sum_{k = -n}^{ n} \hat{f}(k) u_{k}\ bigg\|_{2} = 0, f \in L^{2}(\mathbb{T})

실수축 \mathbb{R} 의 원래 르벡측도에 \frac{1}{2 \pi} 한 측도공간을 \hat{\mathbb{R}} 이라 쓰자. 그러면 등식 \Int_{\mathbb{R}} |f(x)|^{2} dx = \Int_{\mathbb{\hat{R}}} |\hat{f}(\alpha)|^{2} d\alpha, f \in C_{c}(\mathbb{R}) 이 성립한다. 역변환공식은 물론 f(x) = \Int_{\mathbb{\hat{R}}} \hat{f}(\alpha) e^{i \alpha x} d\alpha 로 표현된다.

(명제) 함수공간 C_{c}(\mathbb{R}) 을 L^{2} (\mathbb{R}) 의 부분공간으로 생각하면, 등거리 선형사상 f \mapsto \hat{f} : C_{c} (\mathbb{R}) \to L^{2} (\hat{\mathbb{R}}) 을 얻게 된다. 그런데 C_{c}(\mathbb{R}) 이 L^{2} (\mathbb{R}) 안에서 조밀하므로 이 사상을 L^{2}(\mathbb{R}) 에 확장하여 등거리 선형사상 \mathcal{F} : L^{2}(\mathbb{R}) \to L^{2}(\hat{\mathbb{R}}) 을 얻을 수 있다. 만일 f \L^{1}(\mathbb{R}) \cap L^{2}(\mathbb{R}) 이면 두 사상이 동시에 정의되며, \hat{f} = \mathcal{F} (f) 이다.

(정의) 위 명제에서 정의된 \mathcal{F} : L^{2}(\mathbb{R}) \to L^{2}(\hat{\mathbb{R}}) 는 전단사 등거리사상이며 이를 플랑셰를 변환이라 한다.

(정리 6.3.8) 각 f \in L^{1}(\mathbb{R}) \cap L^{2}(\mathbb{R}) 에 대하여 \hat{f} = \mathcal{F} (f) 를 만족하는 힐버트공간 동형사상 \mathcal{F} : L^{2}(\mathbb{R}) \to L^{2}(\hat{\mathbb{R}}) 이 유일하게 존재한다.

(정의) 플랑셰를 변환이 힐버트공간 동형사상이란 말을 수식으로 쓰면 \Int_{\mathbb{R}} f(x) \bar{g(x)}dx = \frac{1}{2\pi} \Int_{\mathbb{R}} \hat{f}(\alpha)\bar{\hat{g}(\alpha)} d\alpha 가 되는데, 이 역시 파시발 등식이라 불린다.

