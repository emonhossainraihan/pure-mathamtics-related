---



layout: post



title : (Real Analysis 실해석) 적분가능함수공간



date : 2018-01-20 08:52:24 +0900



---

(section 3) 적분가능함수공간

(subsection 3.1)L^{p} 공간

(정의) 잴 수 있는 집합 E \subset \mathbb{R} 과 양수 p >0 에 대하여 조건 \int_{E} |f|^{p} < \infty 를 만족하는 잴 수 있는 함수 f : E \to \mathbb{C} 의 집합을 L^{p}(E) 라 하자.

(정의) 함수 \phi : (a,b) \to \mathbb{R} (단 -\infty \le a < b \le +\infty) 이 다음 조건을 만족할 때, \phi를 볼록함수라 부른다.

a<s<t<u<b \implies \frac{\phi(t) - \phi(s)}{t-s} \le \frac{\phi(u) - \phi(t)}{u-t}

(옌센 부등식)(정리 3.1.1) 함수 f : [0,1] \to (a,b) 가 적분가능하고 \phi : (a,b) \to \mathbb{R} 이 볼록함수이면 (단 -\infty \le a < b \le +\infty) 부등식 \phi\biggl \int_{0}^{1} f \biggr \le \int_{0}^{1} (\phi \bullet f) 이 성립한다.

(정의) 두 양수 0 < p,q < \infty 가 다음 관계식 \frac{1}{p} + \frac{1}{q} 를 만족하면 이를 켤레지수라 부른다. 1, \infty 도 켤레지수라 한다.

(횔더 부등식, 민코프스키 부등식) (정리 3.1.2) 두 양수 p, q 가 켤레지수일 때, 잴 수 있는 집합 E에서 정의된 잴 수 있는 함수 f , g : E \to [0,\infty] 에 대하여 부등식이 성립한다.

\int_{e} fg \le \biggl \int_{E} f^{p}\biggr^{1/p} \biggl \int_{E} g^{p}\biggr^{1/q}

\biggl \int_{E} (f+g)^{p}\biggr^{1/p} \le \biggl \int_{E} f^{p}\biggr^{1/p} + \biggl \int_{E} g^{p}\biggr^{1/q}

(정의) 잴 수 있는 함수 f : E \to \mathbb{C} 와 p \in [1,\infty) 에 대하여 \lVert f \rVert_{p} = \biggl \int_{E} |f|^{p}\biggr^{1/p} 라 정의한다. 그러면 \lVert fg \rVert_{1} \le \lVert f \rVert_{p} \lVert g \rVert_{q} (단 1, < p,q < \infty, \frac{1}{p} + \frac{1}{q}) \lVert f + g \rVert_{p} \le \lVert f \rVert_{p}+ \lVert g \rVert_{p} (단 1 \le p < \infty) 은 횔더 부등식과 민코프스키 부등식의 또다른 형태이다. 따라서 L^{p}(E) 가 벡터공간이 된다.

(정의) 잴 수 있는 함수 f : E \to [0,\infty] 에 대하여 esssup f = \inf{\alpha \in \mathbb{R} : \mu (f^{-1}((\alpha, \infty\rbrack)) = 0 } 이라 정의하자. 위 정의에 나오는 집합이 비어있으면 esssup f = \infty 라 정의한다.

(정의) 잴 수 있는 함수 f : E \to \mathbb{C} 에 대하여 \lVert f \rVert_{\infty} = esssup|f| 라 정의한다. \lVert f \rVert_{\infty} < \infty 인 잴 수 있는 함수 f : E \to \mathbb{C} 전체의 집합을 L^{\infty} (E) 로 쓴다.

(정의) 복소벡터공간 X 에 함수 \lVert \rVert : X \to [0,\infty) 가 주어져서 다음 성질들을 만족하면 이를 노음공간이라 한다.

x \in X, \lVert x \rVert = 0 \implies x = 0

\alpha \in \mathbb{C}, x \in X \implies \lVert \alphax \rVert = |\alpha| \lVert x \rVert 

x, y \in X \implies \lVert x+y \rVert \le \lVert x \rVert + \lVert y \rVert

(명제) 노음공간 L^{p} (E) 의 원소는 ‘거의 모든 점에서 함수값이 일치한다’는 동치관계에 의한 동치류에 의하여 생기는 함수 모임이다. 그러나 그 동치류에 속하는 함수 하나를 마치 L^{p} (E)의 원소인 것처럼 쓰기로 한다.

(정의) 노음공간의 수열 \langle x_{n} \rangle 이 주어져 있을 때, 임의의 양수 \epsilon > 0 에 대하여 다음 성질 m , n > N \implies \lVert x_{n} – x_{m} \rVert < \epsilon 을 만족하는 자연수 N이 존재하면 이 수열 \langle x_{n} \rangle 을 코시수열이라 한다. 

(정의) 모든 코시수열이 수렴하는 노음공간을 바나하공간이라 한다.

(리쓰-피셔)(정리 3.1.3) 각 p \in [1,\infty] 에 대하여 L^{p} (E) 는 바나하공간이다.

(명제 3.1.4) 만일 L^{p}(E) (단, 1 \le p \le \infty) 의 수열 \langle f_{n} \rangle 이 f \in L^{p}(E) 로 수렴하면 (즉, \lVert f_{n} - f \rVert_{p} \to 0 이면) 거의 모든 점에서 f로 점별수렴하는 부분수열을 가진다.

(subsection 3.2) 잴 수 있는 함수와 연속함수

(도움정리 3.2.1) 임의의 유계닫힌집합 K \subset \mathbb{R} 와 열린집합 U \subset \mathbb{R} 가 K \subset U 이면, 다음을 만족하는 연속함수 f : \mathbb{R} \to [0,1] 이 존재한다.

0 \le f \le 1, f|_{K} = 1, f|_{\mathbb{R} \setminus U} = 0

(루진)(정리 3.2.2) 유계구간 [a,b] 위에서 정의된 잴 수 있는 함수 f : [a,b] \to \mathbb{C} 가 있을 때, 임의의 양수 \epsilon >0 에 대하여 \mu({x \in [a,b] : f(x) \neq g(x)}) < \epsilon 를 만족하는 연속함수 g : [a,b] \to \mathbb{C} 가 존재한다. 만일 f \in L^{\infty} [a,b] 이면 \lVert g\rVert _{\infty} \le \lVert f\rVert _{\infty} 가 되도록 연속함수 g 를 택할 수 있다.

(정의) 구간 [a,b] 위에서 정의된 연속함수 f : [a,b] \to \mathbb{C} 를 모두 모은 벡터공간 C[a,b]

(도움정리 3.2.3) 구간 [a,b] 에서 정의된 단순함수 s : [a,b] \to \mathbb{C} 전체의 집합 S는 L^{p}[a,b] 안에서 조밀하다. (단, 1 \le p < \infty)

(정리 3.2.4) 각 p \in [1,\infty) 에 대하여, C[a,b] 는 L^{p}[a,b] 의 조밀한 부분공간이다.

(정의) 함수 f : \mathbb{R} \to \mathbb{C} 의 받침 supp f 를 집합 {x : f(x) \neq 0} 의 닫힘으로 정의하고, 받침이 유계구간에 들어가는 경우 연속함수 전체의 벡터공간을 C_{c}(\mathbb{R}) 이라 쓴다.

(정리 3.2.5) 각 p \in [1,\infty) 에 대하여, C_{c}(\mathbb{R}) 은 L^{p}(\mathbb{R}) 의 조밀한 부분공간이다.

(정의) 집합 X의 곱집합 X \times X 에서 정의된 함수 d : X \times X \to [0,\infty) 가 다음 성질들을 만족하면 d를 거리라 하고, 거리가 주어진 집합을 거리공간이라 한다.

d(x,y) = 0 \implies x = y 이다.

d(x,y) = d(y,x) 이다.

d(x,y) \le d(x,z) + d(z,y) 이다.

 (정의) 임의의 코시수열이 수렴하는 거리공간을 완비거리공간이라 한다.

 거리공간의 부분집합은 다시 거리공간이 되며, 이를 부분공간이라 한다.

\tilde{X} 가 완비거리공간이고 X가 \tilde{X} 의 조밀한 부분공간이면 \tilde{X} 를 X의 완비화공간이라 한다.

(명제) 임의의 노음공간은 거리공간이다.

L^{p}(\mathbb{R}) 이 거리공간 (C_{c}(\mathbb{R}), \lVert \rVert_{p}) 의 완비화공간이다.

(정의) 실수축 위에서 정의된 연속함수 가운데 lim_{x \to \mp \infty} f(x) = 0 인 것들을 모두 모은 벡터공간을 C_{0}(\mathbb{R}) 이라 쓰자. 이 공간에 노음 \lVert f\rVert_{sup} = \sup{|f(x)| : x \in \mathbb{R}} 을 부여하면, 노음공간이 된다.

(정의) 실수축에 정의된 함수 f : \mathbb{R} \to \mathbb{C} 와 점 y \in \mathbb{R} 에 대하여 그 평행이동 f_{y} 를 f_{y}(x) = f(x-y), x \in \mathbb{R} 로 정의한다. 

(정리 3.2.6) 각 함수 f \in L^{p}(\mathbb{R}) 에 대하여 (단, 1 \le p < \infty) y \mapsto f_{y} : \mathbb{R} \to L^{p}(\mathbb{R}) 은 고른연속함수이다.

(도움정리 3.2.7) 유한측도집합 E \subset \mathbb{R} 에서 정의된 잴 수 있는 복소함수열 \langle f_{n} \rangle 이 거의 모든 점에서 f : E \to \mathbb{C} 로 수렴한다고 가정하자. 그러면, 임의의 양수 \epsilon >0 과 \delta >0 에 대하여 다음 성질과 \mu(A) < \delta 를 만족하는 집합 A \subset E 와 자연수 N 을 잡을 수 있다.

n \ge N, x \in E \setminus A \implies |f(x) – f_{n}(x)| < \epsilon

(에고로프)(정리 3.2.8) 유한측도집합 E \subset \mathbb{R} 에서 정의된 잴 수 있는 복소함수열 \langle f_{n} \rangle 이 거의 모든 점에서 f : E \to \mathbb{C} 로 수렴한다고 가정하자. 그러면 임의의 양수 \epsilon >0 에 대하여 다음 성질을 만족하는 집합 A \subset E 를 잡을 수 있다.

\mu(A) < \epsilon, \langle f_{n} \rangle 이 E \setminus A 위에서 고르게 수렴한다.

(subsection 3.3) 양측도와 적분

(정의) 집합 X의 부분집합모임 \mathfrak{S}가 다음 성질을 만족할 때, 이를 \sigma-대수라 부른다.

\empty \subset \mathfrak{S }

만일 A \in \mathfrak{S} 이면 A^{c} \in \mathfrak{S} 이다.

각 n = 1,2, … 에 대하여 A_{n} \in \mathfrak{S} 이면 \bigcup_{n = 1}^{\infty} A_[n] \in \mathfrak{S} 이다.

(정의) 만일 함수 \mu : \mathfrak{S} \to [0,\infty] 가 다음 성질을 만족하고 \mu(\empty) = 0 이면, 이를 양측도 혹은 그냥 측도라 한다. 또한, 집합모임 \mathfrak{S} 에 들어가는 X의 부분집합들을 잴수있는 집합이라 부른다.

{A_{n} \in \mathfrak{S} : n = 1,2, …} 가 서로소 \implies \mu\biggl \bigsqcup_{n=1}^{\infty} A_{n} \biggr = \sum_{n = 1}^{\infty} \mu(A_{n})

(명제 3.3.1) 양측도 (X, \mathfrak{S}, \mu) 에 대하여 다음이 성립한다.

A \subset B 이면 (단 A, B \in \mathfrak{S}) \mu(A) \le \mu(B) 이다.

잴수있는 단순증가 집합열 \langle A_{n} \rangle 에 대하여 등식 \mu \biggl \bigcup_{n=1}^{\infty} A_{n} \biggr = \lim_{n \to \infty} \mu(A_{n}) 이 성립한다.

잴 수 있는 단순감소 집합열 \langle A_{n} \rangle 에 대하여 \mu(A_{1}) < \infty 이면 등식 \mu \biggl \bigcap_{n=1}^{\infty} A_{n} \biggr = \lim_{n \to \infty} \mu(A_{n}) 가 성립한다.

(정의) 다음 세 가지 성질을 만족하는 함수 \mu : \mathcal{P} (X) \to [0,\infty] 를 집합 X의 외측도라 한다.

\mu(\empty) = 0

만일 S \subseteq T 이면 \mu(S) \le \mu(T) 이다.

임의의 셀 수 있는 집합 모임 {S_{n} : n = 1,2,…} 에 대하여 \mu \biggl( \bigcup_{n = 1}^{\infty} S_{n} \biggr) \le \sum_{n=1}^{\infty} \mu(S_{n}) 이 성립한다.

(정의) 카라테오도리 조건 S \subseteq X \implies \mu(S) = \mu(S \cap E) + \mu(S \cap E^{c}) 를 만족하는 집합 E \subset X 들의 모임을 \mathfrak{S} 라 한다.

(명제 3.3.2) 집합 X에 외측도 \mu : \mathcal{P} (X) \to [0, \infty] 가 주어져 있을 때, 카라테오도리 조건을 만족하는 집합모임 \mathfrak{S} 는 \sigma – 대수가 되고, \mu(S) = 0 이면 S \in \mathfrak(S) 이다. 또한 \mu 를 \mathfrak(S) 에 제한하면 측도가 된다.

(명제 3.3.3) 집합 X 에서 정의된 함수 f : X \to \mathbb{R}^{*} 에 대하여 다음은 동치이다.

함수 f는 잴 수 있는 함수이다.

임의의 a \in \mathbb{R} 에 대하여 {x \in E : f(x) \ge a} \in \mathfrak{S} 이다. 

임의의 a \in \mathbb{R} 에 대하여 {x \in E : f(x) < a} \in \mathfrak{S} 이다. 

임의의 a \in \mathbb{R} 에 대하여 {x \in E : f(x) \le a} \in \mathfrak{S} 이다.

(명제 3.3.4) 집합 X에서 정의된 함수 f : X \to [-\infty, \infty] 에 대하여 다음이 성립한다.

만일 f, g가 잴 수 있고 \alpha \in \mathbb{R} 이면 f + g, fg, \alpha f 도 잴 수 있다.

각 n = 1,2, …. 에 대하여 f_{n} 이 잴 수 있으면 함수 x \mapsto \inf_{n} f_{n} (x) 와 x \mapsto \sup_{n}f_{n}(x) 도 잴 수 있다.

각 n = 1,2, …. 에 대하여 함수 f_{n} 이 잴 수 있으면 점별극한함수 \limsup_{n} f_{n} , \liminf_{n} f_{n}, \lim_{n} f_{n} 도 잴 수 있다.

함수 f : E \to \mathbb{R}^{*} 이 잴 수 있고, g : \mathbb{R} \to \mathbb{R} 이 연속이면 그 합성함수 g \bullet f 도 잴 수 있다. 여기서, f(x) = \mp \infty 인 x \in E 에 대해서는 (g \bullet f) (x) = \mp \infty 로 정의한다.

(정의) 잴 수 있는 함수 f : E \to \mathbb{R} 의 치역이 유한집합이면, 이를 단순함수라 한다.

치역이 {c_{1}, …, c_{n}} 인 단순함수 s : E \to \mathbb{R} 가 있을 때, 각 i = 1,2,…, n 에 대하여 E_{i} = { x \in E : s(x) = c_{i}} 라 두면 {E_{i}} 는 서로소이고 s 는 s = \sum_{i = 1}^{n} c_{i} \chi_{E_{i}} 같이 잴 수 있는 특성함수들의 선형결합으로 표시할 수 있다.

(정의) 정의된 단순함수가 s \ge 0 일때, 그 적분을 \int_{E} s d\mu = \sum_{i = 1}^{n} c_{i} m\muE_{i}) 라 정의한다.

(정의) 잴 수 있는 함수 f : E \to [0, +\infty] 의 적분을 \inf_{E} f = sup{\inf_{E} s : 0 \le s \le f, s 는 단순함수}  로 정의한다.

(정의) 함수 f : X \to \mathbb{R}^{*} 에 대하여 f_{+} (x) = max{f(x),0}, f_{-} (x) = - min{f(x),0}, x \in X 라 두면 f_{+}, f_{-} \ge 0 이고 f = f_{+} – f_{-} 이다. 

(정의) 함수 f 의 적분을 \int_{E} f d\mu = \int_{E} f_{+} d\mu - \int_{E} f_{-} d\mu 라 정의한다. 만일 함수 f_{+} 와 함수 f_{-} 의 적분값이 모두 무한이면 f의 적분을 정의하지 않는다.

(정의) 함수 f_{+}와 f_{-} 의 적분값이 모두 유한일 때, 함수 f 를 적분가능함수라 한다.

 (정의) 잴 수 있는 집합 E에서 정의된 복소함수 f : E \to \mathbb{C} 에 대해 함수 f = u + iv 의 실수부를 u, 허수부를 v라 하자. u와 v가 잴 수 있으면 f가 잴 수 있다고 한다.복소함수의 적분을 \int_{E} (u + iv) d\mu = \int_{E} u d\mu + i \int_{E} v d\mu 라 정의한다. 적분가능성은 똑같이 정의한다.

(명제) 서로소인 잴 수 있는 집합 모임 {A_{n} : n = 1,2, …} 에 대하여 A = \sqcup_{n = 1}^{\infty} A_{n} 이라 하자. 그러면 임의의 잴 수 있는 함수 f : X \to [0,\infty] 및 적분가능함수 f : X \to \mathbb{C} 에 대하여 등식 \int_{A} f d\mu = \sum_{n = 1}^{\infty} \int_{A_{n}} f d\mu 이 성립한다.

(명제) 잴 수 있는 함수 f, g : X \to [0,\infty] 혹은 적분가능함수 f, g : X \to \mathbb{C} 에 대하여 등식 \int_{X} (\alpha f + \beta g) d\mu = \alpha \int_{X} f d\mu + \beta \int_{X} g d\mu 가 성립한다. (단 \alpha, \beta 는 상수)

(명제)집합 X에서 [0, + \infty] 로 가는 잴 수 있는 함수열 \left \langle f_{n} \right \rangle 에 대하여, 부등식 \int_{X} (\liminf_{n \to \infty} f_{n}) d\mu \le \liminf_{n \to \infty} \int_{X} f_{n} d\mu 이 성립한다.

(명제) 함수열  \left \langle f_{n} \right \rangle 이 거의 모든 점에서 f로 수렴하는 경우, 만일 0 \le f_{1} \le f_{2} \le … 이거나 각 n = 1,2, … 에 대하여 |f_{n}| \le g 인 g \in L^{1}(X) 가 존재한다면, 등식 \lim_{n \to \infty} \int_{X} f_{n} d\mu = \int_{X} f d\mu 이 성립한다.

(명제) X에서 [0, +\infty] 로 가는 임의의 잴수있는 함수열 \langle f_{n} \rangle 에 대하여 등식 \int_{X} \biggl( \sum_{n = 1}^{\infty} f_{n} \biggr) d\mu = \sum_{n = 1}^{\infty}\int_{X} f_{n} d\mu 를 얻는다.

(명제) X 에서 \mathbb{C} 로 가는 L^{1}-함수열  \left \langle f_{n} \right \rangle 에 대하여 급수 \sum_{n = 1}^{\infty} \int_{E} |f_{n}| 가 수렴하면, 거의 모든 x \in E 에 대하여 급수 \sum_{n = 1}^{\infty} f_{n}(x) 가 절대수렴한다. 또한, 그 극한값을 f(x) = \sum_{n = 1}^{\infty} f_{n}(x) 라 두면 f \in L^{1}(X) 이고 그 적분값은 \int_{E} f d\mu = \sum_{n = 1}^{\infty} \int_{X} f_{n} d\mu 로 주어진다.

(명제) 집합 X 에서 정의된 잴 수 있는 함수 f 에 대하여 다음이 성립한다.

만일 f \ge 0 이고 \inf_{X} f = 0 이면 거의 모든 점에서 f = 0 이다.

만일 f \in L^{1} (X) 이고 임의의 잴 수 있는 집합 D \subset X 에 대하여 \int_{D} f = 0 이면 거의 모든 점에서 f = 0이다.

(명제 3.3.5) 집합 X의 측도 \mu(X) 가 유한값이고, F \subset \mathbb{C} 가 닫힌 집합이라 하자. 만일 f \in L^{1}(X, \mathfrak{S}, \mu) 가 다음 조건을 만족하면 거의 모든 점 x \in X 에 대하여 f(x) \in F 가 성립한다.

E \in \mathfrak{S}, \mu(E) >0 \implies \frac{1}{\mu(E)} \int_{E} f d\mu \in F

(정의) 집합 X의 멱집합 \mathcal{P} 는 \sigma -대수이다. 각 A \in \mathcal{P}(X) 에 대하여 c(A) 를 집합 A의 원소의 개수라 정의하면 이는 양측도가 되는데, 함수 f : X \to \mathbb{C} 의 적분 \int_{X} f dc 를 그냥 \sum_{x \in X} f(x) 라 쓴다. 그러나 \sum_{x \in X} f(x) 는 함수 f 가 f \ge 0 이거나, 적분가능할 때에만 그 의미가 있다.

(명제) 앞의 정의의 경우 X = \sqcup_{n=1}^{\infty} X_{n} 이면 등식 \sum_{x\inX} f(x) = \sum_{n=1}^{\infty}\sum_{x \in X_{n}} f(x) 이 성립한다.

(명제 3.3.6) 함수 f : X \to \mathbb{C} 에 대하여 등식 \sum_{x \in X} |f(x)| = \sup {\sum_{x \in F} |f(x)| : F \subset X 는 유한집합이다} 이 성립한다.

(따름정리 3.3.7) 각 자연수 m,n = 1, 2, … 에 대하여 a_{m,n} \in \mathbb{C} 이 주어져있을 때, 다음이 성립한다.

만일 a_{m,n} \ge 0 이면, \sum_{n = 1}^{\infty} \sum_{m = 1}^{\infty} a_{m,n} =\sum_{m = 1}^{\infty} \sum_{n = 1}^{\infty} a_{m,n} 이 성립한다.

다음 성질 \sum_{n} b_{n} < \infty, \sum_{m=1}^{\infty} |a_{m,n}| \le b_{n} , n = 1,2, … 을 만족하는 급수 \sum b_{n} 이 있으면, \sum_{n = 1}^{\infty} \sum_{m = 1}^{\infty} a_{m,n} =\sum_{m = 1}^{\infty} \sum_{n = 1}^{\infty} a_{m,n} 이 성립한다.

(정의) 함수 f : X \to \mathbb{C} 와 p \in [1,\infty) 에 대하여 \lVert f \rVert_{p} = \biggl( \int_{X} |f|^{p} d\mu \biggr)^{1/p} 라 정의하고, \lVert f \rVert_{\infty} 역시 이전과 같이 정의한다. 

(정의) \lVert f \rVert_{p} < \infty 인 함수 f : X \to \mathbb{C} 전체의 집합을 L^{p}(X, \mathfrak{S},\mu), 줄여서 L^{p}(X,\mu) 혹은 L^{p}(\mu) 라 쓴다. 만일 E \in \mathbb{R} 이 잴 수 있는 집합이고 m 이 르벡측도라면 L^{p}(E,m) 을 그냥 L^{p}(E) 라 쓴다. L^{p}(\mu) 는 바나하공간이 된다.

(명제 3.3.8) 단순함수 s : X \to \mathbb{C} 가운데 \mu{x\in X : s(x) \neq 0} < \infty 를 만족하는 것들 전체의 집합 S는 L^{p}(\mu) 안에서 조밀하다. (단, 1 \le p < \infty)

(정의) 개수를 세는 측도에 의한 공간 L^{p}(X,\mathcal{P}, c) 는 \mathcal{l}^{p}(X) 라 쓴다. X가 자연수 집합이면 \mathcal{l}^{p} 라 쓴다. 

(명제) \mathcal{l}^{\infty} 는 유계수열공간이고 \mathcal{l}^{1} 은 절대수렴하는 수열들을 모아놓은 공간이 된다. 노음공간 \mathcal{l}^{p}({1,2,…,n}) 은 \lVert x\rVert_{p} = (|x_{1}|^{p} + … + |x_{n}|^{p})^{1/p}, x = (x_{1}, x_{2}, …, x_{n}) 으로 노음이 부여된 노음공간 (\mathbb{C}^{n}, \lVert \rVert_{p} ) 이 된다.

(정의) 벡터공간 V 의 부분집합 S \subset V 가 다음 조건을 만족하면 S를 볼록집합이라 부른다.

x , y \in S, 0 \le t \le 1 \implies tx + (1-t)y \in S

(명제) 1 \le p < q \le \infty \implies \mathcal{l}^{p}(X) \subset \mathcal{l}^{q}(X) 

\mu(X) < \infty, 1 \le p < q \le \infty \implies L^{q}(X,\mu) \subset L^{p}(X,\mu)

