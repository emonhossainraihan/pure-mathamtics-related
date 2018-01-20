---



layout: post



title : \[Real Analysis 실해석] 이중적분



date : 2018-01-20 08:52:34 +0900



---

(section 4) 이중적분

(subsection 4.1) 곱측도

(명제) 집합 X, Y 에 각각 양측도 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak(I), \nu) 가 주어져 있다. 집합 X \times Y 의 \sigma-대수는 \mathfrak(R) = {S\timesT \subset X\timesY : S \in \mathfrak{S}, T \in \mathfrak{T}}를 포함해야 한다.

(정의 1) 집합 E \subset X \times Y 와 x \in X, y \in Y 에 대하여 E_{x} = {y \in Y : (x,y) \in E}, E^{y} = {x \in X : (x,y) \in E} 라고 정의하자. 만일 각 x \in X, y \in Y 에 대하여 E_{x} \in \mathfrak{T}, E^{y} \in \mathfrak{S} 라면 두 함수 \phi : x \mapsto \nu(E_{x}) = \int_{Y} \chi_{E}(x,y) d\nu(y), \psi : y \mapsto \nu(E^{y}) = \int_{X} \chi_{E}(x,y) d\mu(y) 로 정의할 수 있다. 

(정의 2) 만일 두 함수 \phi, \psi 가 각각 잴 수 있는 함수이고 등식 \int_{X} \phi d\mu = \int_{Y} \psi d\nu 이면 이 공통값을 E의 측도로 정의한다.

(정의) X와 Y가 유한측도를 가지는 부분집합들로 분할될 수 있다 가정한다. 즉, X = \bigsqcup_{n = 1}^{\infty} X_{n}, Y=\bigsqcup_{m = 1}^{\infty} Y_{m} 이라 가정한다. (단, 각 m, n = 1,2,…에 대하여 \mu(X_{n}), \nu(Y_{m}) < \infty) 두 집합 모임 \mathfrak{B} = {E \in \mathfrak{S} \times \mathfrak{T} : (정의 1) 에서 정의한 두 함수 \phi, \psi 가 잴 수 있고 (정의 2)의 등식이 성립한다}

\mathfrak{C} = {E \in \mathfrak{S} \times \mathfrak{T} : E \cap (X_{n} \times Y_[m]) \in \mathfrak{B} (m,n = 1,2,…)}

(도움정리 4.1.1) 집합모임 \mathfrak{B}와 \mathfrak{C} 에 대하여 다음이 성립한다.

\mathfrak{B} 는 단조증가하는 집합열의 합집합에 대하여 닫혀있다. 

\mathfrak{B} 는 서로소인 집합열의 합집합에 대하여 닫혀있다.

\mathfrak{C} 는 단조증가하는 집합열의 합집합과 단조감소 집합열의 교집합에 대하여 닫혀있다.

만일 E_{1} , …, E_{n} \in \mathfrak{R} 이 서로소이면 \bigsqcup_{n = 1}^{N} E_{n} \in \mathfrak{C}이다.

(정의) 전체집합 X가 유한측도를 가지는 부분집합열의 합집합으로 표시되면 , (X ,\mu) 를 \sigma -유한측도 라 한다.

(정리 4.1.2) 양측도 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak{T},\nu) 가 주어져 있을 때, 잴수있는 상자들을 포함하는 최소의 \sigma-대수를 \mathfrak{S} \times \mathfrak{T} 라 쓰자. 만일 E \in \mathfrak{S} 이면, 임의의 x \in X 와 y \in Y 에 대하여 E_{x} \in \mathfrak{T} 및 E^{y} \in \mathfrak{S 가 성립한다. 만일 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak{T},\nu) 가 각각 \sigma-유한이면 (정의 1) 의 \phi,\psi 가 각각 잴 수 있는 함수이고 (정의 2)의 등식이 성립한다.

(정의) (정의 2)의 등식의 공통값을 (\mu \times \nu)(E) 라 쓰면, (X \times Y, \mathfrak{S} \times \mathfrak{T} ,  \mu \times \nu) 를  \sigma -유한측도 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak{T},\nu)의 곱측도라 부른다.

(정의) 르벡측도 (\mathbb{R}, \mathfrak{M}, m) 에 대해 좌표공간 \mathbb(R)^{n} 의 열린 집합들을 포함하는 최소의 \sigma-대수를 \mathfrak{B}_{n} 이라 쓰면, \mathfrak{B}_{2} \subset \mathfrak{M} \times \mathfrak{M} 이 된다. 집합모임 \mathfrak{B}_{n} 에 들어가는 \mathbb{R}^{n} 의 부분집합을 보렐집합이라고 한다. 

닫힌집합, G_{\delta} 집합, F_{\delta}-집합 등은 보렐집합의 예이다.

(정의) 측도 (X,\mathfrak{S}, \mu) 가 성질 E \subset F , F \in \mathfrak{S} , \mu(F) = 0 \implies E \in \mathfrak{S} 를 만족하면 이를 완비측도라 한다.

(명제 4.1.3) 양측도 (X, \mathfrak{S}, \mu) 에 대하여 집합모임 \mathfrak{S}^{*} = {E \subset X : A \subset E \subset B 및 \mu(B\setminus A) = 0 을 만족하는 A,B \in \mathfrak{S} 가 존재한다.} 을 생각하고, 각 E \in \mathfrak{S}^{*} 에 대하여 \mu^{*}(E) = \mu(A) 라 정의하자. 그러면 (X, \mathfrak(S)^{*}, \mu^{*}) 는 완비측도가 된다.

(정의) (\mathfrak{M} \times \mathfrak{M})^{*} = \mathfrak{B}_{2}^{*} 이다. 이 \sigma -대수를 \mathfrak{M}_{2} 라 두고 이 위에서 정의된 측도 (m \times m) 을 m_{2} 라 쓰면 완비측도 (\mathbb{R}^{2}, \mathfrak{M}_{2}, m_{2}) 를 얻는데, 이를 \mathbb{R}^{2} 의 르벡측도라 한다.

(subsection 4.2) 푸비니 정리

(정의) 지금부터 집합 X, Y 에 양측도 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak{T}, \nu) 가 주어져있다고 가정하고 X \times Y 위에 정의된 임의의 함수 f 에 대하여 f_{x} : y \mapsto f(x,y), f^{y} : x \mapsto f(x,y) 라 정의한다.

(명제 4.2.1) 함수 f : X \times Y \to \mathbb{R}^{*} 이 \mathfrak{S} \times \mathfrak{T} 에 대하여 잴 수 있는 함수라 하자. 그러면, 임의의 x \in X 와 y \in Y 에 대하여 f_{x} 와 f^{y} 는 각각 \mathfrak{T} 와 \mathfrak{S} 에 대하여 잴 수 있는 함수이다.

(토넬리)(정리 4.2.2) 양측도 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak{T}, \nu) 가 각각 \sigma-유한이라고 하자. 그러면 임의의 잴 수 있는 함수 f : X \times Y \to [0,\infty] 에 대하여 다음이 성립한다.

함수 x \mapsto \int_{Y}f_{x}d\nu 와 y \mapsto \int_{X}f^{y}d\mu 가 각각 잴 수 있는 함수이다.

등식 \int_{X}[\int_{Y}f_{x}d\nu]d\mu = \int_{X\timesY}fd(\mu\times\nu) = \int_{y} [\int_{X} f^{y}d\mu] d\nu

(푸비니)(정리 4.2.3) 양측도 (X, \mathfrak{S}, \mu) 와 (Y, \mathfrak{T}, \nu)가 각각 \sigma -유한이라고 하자. 잴 수 있는 함수 f:X \times Y \to \mathbb{C} 가 \int_{X} [\int_{Y} |f(x,y)| d\nu(y) ] d\mu(x) < \infty 를 만족하면 다음이 성립한다.

f \in L^{1}(\mu \times \nu) 이다. 또한, 거의 모든 x \in X 에 대하여 f_{x} \in L^{1}(\nu) 이고, 거의 모든 y \in Y 에 대하여 f^{y} \in L^{1}(\mu) 이다.

거의 모든 점에서 정의된 두 함수 x \mapsto \int_{Y} f_{x}d\nu 와 y \mapsto \int_{x}f^{y} d\mu 가 각각 적분가능함수이다.

등식 \int_{X}[\int_{Y} f_{x}d\nu] d\mu = \int_{X \times Y}fd(\mu \times \nu) = \int_{Y}[\int_{X} f^{y}d\mu] d\nu 이 성립한다.

(정의) 좌표공간 \mathbb{R}^{n} 위에 정의된 함수가 \sigma-대수 \mathfrak{B} 에 대하여 잴 수 있으면 이를 보렐함수라 부른다. 그냥 잴 수 있는 함수라 하면 르벡측도 (\mathfrak{M}_{n}, m_{n}) 에 대하여 잴 수 있음을 뜻한다.

(명제 4.2.4) 양측도 (X, \mathfrak{S} , \mu) 에 대하여 잴 수 있는 함수인 f : X \to \mathbb{R} 과 보렐함수 g : \mathbb{R} \to \mathbb{R} 에 대하여 그 합성함수 g \bullet f : X \to \mathbb{R} 은 잴 수 있는 함수이다.

(명제 4.2.5) 좌표공간 \mathbb{R}^{n} 에서 정의된 잴 수 있는 함수 f 가 주어지면, 거의 모든 점에서 f = g 인 보렐함수 g 가 존재한다.

(토넬리-푸비니)(정리 4.2.6) 좌표평면 \mathbb{R}^{2} 에서 정의된 잴 수 있는 함수 f 에 대하여 다음이 성립한다.

거의 모든 점 x 와 y 에 대하여, f_{x} 및 f^{y} 는 잴 수 있는 함수이다.

만일 0 \le f \le \infty 이면 등식 \int_{\mathbb{R}}\int_{\mathbb{R}}f(x,y) dxdy = \int_{\mathbb{R}\times \mathbb{R}} f dm_{2} = \int_{\mathbb{R}}\int_{\mathbb{R}}f(x,y) dydx 이 성립한다.

만일 f : \mathbb{R}^{2} \to \mathbb{C} 이고 \int_{\mathbb{R}}\int_{\mathbb{R}} |f(x,y)| dxdy < \infty 이면 f \in L^{1}(m_{2}) 이다. 또한, 거의 모든 x, y 에 대하여 f_{x}, f^{y} \in L^{1}(m_{1}) 이고 등식 \int_{\mathbb{R}}\int_{\mathbb{R}}f(x,y) dxdy = \int_{\mathbb{R}\times \mathbb{R}} f dm_{2} = \int_{\mathbb{R}}\int_{\mathbb{R}}f(x,y) dydx 이 성립한다.

(subsection 4.3) 적분가능함수의 곱하기

(정의) 적분가능함수 f,g \in L^{1}(\mathbb{R}) 에 대하여 x \mapsto \int_{\mathbb{R} f(y)g(x-y) dy 로 정의된 새로운 L^{1}- 함수를 f*g 라 쓰고, 이를 f 와 g의 곱하기 또는 컨볼류션이라 부른다. \lVert f * g\rVert_{1} \le \lvert f\rVert_{1} \lVert g \rVert_{1} , f,g \in L^{1}(\mathbb{R}) 이 된다.

(명제 4.3.1) 각 f,g,h \in L^{1}(\mathbb{R}) 와 상수 \alpha, \beta \in \mathbb{C} 에 대하여 다음이 성립한다.

거의 모든 점 x 에 대하여 |(f*g)*h|(x) = |f*(g*h)|(x) 가 성립한다.

각 x에 대하여 (f*g)(x) = (g*f)(x) 이다.

거의 모든 점 x에 대하여 |(\alpha f + \beta g)*h|(x) = |\alpha(f*h) + \beta(g*h)|(x) 가 성립한다.

(정의) 일반적으로, 바나하공간 X에 연산 (x,y) \mapsto xy 가 정의되어 결합법칙 및 분배법칙과 부등식 \lVert xy\rVert \le \lvert x\rVert \lVert y \rVert , x,y \in X 를 만족하면, 이를 바나하대수라 한다. L^{1}(\mathbb{R}) 은 바나하대수이다.

(명제 4.3.2) 만일 함수 g가 미분가능하고 f,g,g’ \in L^{1}(\mathbb{R}) 이면, f*g 가 미분가능하고 (f*g)’ = f*g’ 이 성립한다.

(명제 4.3.3) 두 양수 p,q \in (1,\infty)가 켤레지수라 하자. 그러면 임의의 f\in L^{p}(\mathbb{R}) 과 g \in L^{q}(\mathbb{R}) 에 대하여 f * g \in C_{0}(\mathbb{R}) 이다.

