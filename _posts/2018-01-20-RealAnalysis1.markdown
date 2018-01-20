---



layout: post



title : \[Real Analysis 실해석] 르벡적분



date : 2018-01-20 08:52:03 +0900



---

(section 1) 르벡적분

(subsection 1.1) 잴 수 있는 집합과 측도

(정의) 열린 집합 U \mathbb{R}의 한 점 x \in U 를 고정하고 a_{x} = inf{a\in \mathbb{R} : (a,x) \subseteq U } , b_{x} = sup{b\in \mathbb{R} : (a,b) \subseteq U } 라 정의한다. I_{x} = (a_{x} , b_{x}) 라 두자. U = \bigcup_{x \in U} I_{x} 는 서로소인 열린 구간들의 합집합이다.

(명제 1.1.1) 실수의 부분집합 U \subseteq \mathbb{R} 가 열린 집합이라면, U는 셀 수 있는 서로소인 열린 구간의 합집합으로 표시된다. 또한 이 표시방법은 한 가지 뿐이다.

(정의) 열린 집합 U \mathbb{R} 가 서로소인 열린 구간의 합집합 \sqcup_{n}(a_{n} b_{n}) 으로 표시되었을 때 그 길이 \lambda(U) 를 \lambda(U) = \sum_{n = 1}^{\infty} (b_{n} – a_{n}) 으로 정의한다.

(정의) 임의의 집합 S \subset \mathbb{R} 에 대하여 그 길이 \mu(S) 를 \mu(S) = inf{\lambda(U) : U \supseteq S, U는 열린 집합} 으로 정의한다.

(정의) 집합 S \subset \mathbb{R}과 점 x \in \mathbb{R} 에 대하여 x + S = {x + y \in \mathbb{R} : y \in S} 로 정의하고 이를 집합 S 의 평행이동이라 부른다.

(명제 1.1.2) 함수 \mu : \mathcal{P}(R) \to [0,\infty] 는 다음 성질을 가진다.

만일 S \subseteq T 이면 \mu(S) \le \mu(T) 이다.

만일 I 가 a, b를 양끝점으로 하는 구간이면 \mu(I) = |b – a| 이다.

임의의 x \in \mathbb{R} 와 S \ini \mathcal{R} 에 대하여 \mu(x + S) = \mu(S)이다.

임의의 셀 수 있는 집합 모임 {S_{n} : n = 1,2,…} 에 대하여 \mu \biggl( \bigcup_{n = 1}^{\infty} S_{n} \biggr) \le \sum_{n=1}^{\infty} \mu(S_{n}) 이 성립한다.

(정의) 집합 E \subseteq \mathbb{R}이 다음 조건 A \subseteq \mathbb{R} \implies \mu(A) = \mu(A \cap E) + \mu(A \cap E^{c}) 를 만족하면 E를 잴 수 있는 집합이라 부르고, 잴 수 있는 집합 전체의 모임을 \mathfrak{M} 이라 쓴다.. 잴 수 있는 집합의 조건은 카라테오도리 조건이라 불린다.

(정리 1.1.3) 집합 모임 \mathfrak{M}은 다음 성질을 가진다.

\empty \subset \mathfrak{M}

만일 E \in \mathfrak{M} 이면 E^{c} \in \mathfrak{M} 이다.

만일 E, F \in \mathfrak{M} 이면 E \cup F \in \mathfrak{M} 이다.

각 n = 1,2, … 에 대하여 E_{n} \in \mathfrak{M} 이면 \bigcup_{n} E_[n] \in \mathfrak{M} 이다.

만일 \mu€ = 0 이면 E \in \mathfrak{M} 이다.

집합 I 가 구간이면 I \in \mathfrak{M} 이다.

집합 S가 열린 집합이면 S \in \mathfrak{M} 이다.

(정리 1.1.4) 각 n \ 1,2, … 에 대하여 E_{n} \in \mathfrak{M} 이고 집합모임 {E_{n}} 이 서로소이면 등식 \mu \biggl( \bigsqcup_{n = 1}^{\infty} E_{n} \biggr) = \sum_{n=1}^{\infty} \mu(E_{n}) 이 성립한다.

(따름정리 1.1.5) 잴 수 있는 단순증가 집합열 <E_{n}> 에 대하여 등식 \mu \biggl( \bigcup_{n = 1}^{\infty} E_{n} \biggr) = \lim_{n \to \infty} \mu(E_{n}) 이 성립한다. 또한 잴 수 있는 단순감소 집합열 <F_{n}> 에 대하여 \mu(F_{1}) < \infty 이면 등식 \mu \biggl( \bigcap_{n = 1}^{\infty} F_{n} \biggr) = \lim_{n \to \infty} \mu(F_{n}) 이 성립한다.

(정의) 열린 집합들의 셀 수 있는 교집합으로 표시되는 집합을 G_{delta} -집합 이라 하고, 닫힌 집합들의 셀 수 있는 합집합으로 표시되는 집합을 F_{delta} -집합이라 부른다. 이 두 부류의 집합들은 잴 수 있다.

(명제 1.1.6) 집합 E \subset \mathbb{R} 에 대하여 다음이 동치이다.

E가 잴 수 있는 집합이다.

임의의 양수 \epsilon > 0 에 대하여 F \subset E \subset U, \mu(U \setminus F) < \epsilon 인 열린 집합  U 와 닫힌 집합 F 가 존재한다.

B \subset E \subset A , \mu(A \setminus B) = 0 를 만족하는 G_{delta}= 집합 A 와 F_{delta} -집합 B 가 존재한다.

(따름정리 1.1.7) 임의의 잴 수 있는 집합 E \subset \mathbb{R} 에 대하여 등식 \mu(E) = \sup{\mu(K) : K \subset E, K 는 닫힌 유계집합}

(정의) 우선 구간 I = [0,1] 을 삼등분하여 가운데 열린구간 J_{1} 를 들어내고, 즉 C_{1} = I \setminus J_{1} 이라 두고 C_{1}의 두 구간에 대하여도 똑 같은 일을 되풀이한다. C_{2} 의 네 구간에 대하여도 똑 같은 일을 되풀이한다. 이렇게 하여 얻은 닫힌 집합열 \langle C_{n} \rangle 들의 교집합을 C = \bigcup C_{n} 이라 두고 이를 칸토르 집합이라 한다.

(정의) 함수 \mu : \mathcal{P} (\mathbb{R}) \to [0,\infty] 를 \mathfrak{M} 에 제한했을 때 이를 m : \mathfrak{M} \to [0,\infty] 이라 쓰자. 

(정의) 임의의 집합 X의 멱집합의 부분집합 \mathfrak{S} 가 (정리 1.1.3) 의 첫 번쨰 조건부터 네 번째 조건까지를 만족하면, 이를 \sigma – 대수라 부른다. 

(정의) X의 \sigma – 대수가 주어지고 함수 \mu : \mathfrak{S} \to [0,\infty] 가 조건 \mu \biggl( \bigsqcup_{n = 1}^{\infty} E_{n} \biggr) = \lim_{n \to \infty} \mu(E_{n}) 를 만족하면, (\mathfrak{S}, \mu) 를 X의 측도라 하고, \mathfrak{S} 의 원들을 잴 수 있는 집합이라 부른다.

따라서 (\mathfrak{M},m) 은 \mathbb{R}의 측도인데, 이를 르벡 측도라 한다.

(정의) 집합 X의 한 점 x \in X를 고정하고, 임의의 집합 A \subset X 에 대하여 \delta_{x}(A) = \begin{cases}1 & x \in A \\ 0 & x \notin A \end{cases} 라 정의하면 (\mathcal{P}(X) , \delta_{x}) 는 X의 측도가 되는데, 이렇게 정의된 측도를 디락 측도라 부른다.

(subsection 1.2)잴 수 있는 함수와 적분

(정의) 확장실수체 \mathbb{R}^{*} = \mathbb{R} \cup {\mp \infty}

(정의) 잴 수 있는 집합 E \subseteq \mathbb{R} 에서 정의된 함수 f : E \to \mathbb{R}^{*} 이 다음 조건 a\in \mathbb{R} \implies {x \in E : f(x) > a} \in \mathfrak{M} 을 만족하면 이를 잴 수 있는 함수라 한다.

(정의) 집합 A \subseteq \mathbb{R} 에 대하여, 그 특성함수 \chi_{A} : \mathbb{R} \to \mathbb{R} 를 \chi_{A}(x) = \begin{cases}1 & x \in A \\ 0 & x \notin A \end{cases} 라 정의하자.

그러면 집합 A가 잴 수 있을 필요충분조건은 \chi_{A} 가 잴 수 있는 함수임이다.

(명제 1.2.1) 잴 수 있는 집합 E 에서 정의된 함수 f : E \to \mathbb{R}^{*} 에 대하여 다음은 동치이다.

함수 f는 잴 수 있는 함수이다.

임의의 a \in \mathbb{R} 에 대하여 {x \in E : f(x) \ge a} \in \mathfrak{M} 이다. 

임의의 a \in \mathbb{R} 에 대하여 {x \in E : f(x) < a} \in \mathfrak{M} 이다. 

임의의 a \in \mathbb{R} 에 대하여 {x \in E : f(x) \le a} \in \mathfrak{M} 이다.

(따름정리 1.2.2) 함수 f: E \to \mathbb{R}^{*} 이 잴 수 있으면, 임의의 a \in \mathbb{R}^{*} 에 대하여 집합 {x \in E : f(x) = a} 는 잴 수 있다.

(명제 1.2.3) 잴 수 있는 집합 E 에서 \mathbb{R}^{*} 로 가는 함수들에 대하여 다음이 성립한다.

연속함수 f : E \to \mathbb{R} 은 잴 수 있다.

만일 f, g가 잴 수 있고 \alpha \in \mathbb{R} 이면 f + g, fg, \alpha f 도 잴 수 있다.

각 n = 1,2, …. 에 대하여 f_{n} 이 잴 수 있으면 함수 x \mapsto \inf_{n} f_{n} (x) 와 x \mapsto \sup_{n}f_{n}(x) 도 잴 수 있다.

각 n = 1,2, …. 에 대하여 함수 f_{n} 이 잴 수 있으면 점별극한함수 \limsup_{n} f_{n} , \liminf_{n} f_{n}, \lim_{n} f_{n} 도 잴 수 있다.

함수 f : E \to \mathbb{R}^{*} 이 잴 수 있고, g : \mathbb{R} \to \mathbb{R} 이 연속이면 그 합성함수 g \bullet f 도 잴 수 있다. 여기서, f(x) = \mp \infty 인 x \in E 에 대해서는 (g \bullet f) (x) = \mp \infty 로 정의한다.

(정의) 잴 수 있는 함수 f : E \to \mathbb{R} 의 치역이 유한집합이면, 이를 단순함수라 한다.

치역이 {c_{1}, …, c_{n}} 인 단순함수 s : E \to \mathbb{R} 가 있을 때, 각 i = 1,2,…, n 에 대하여 E_{i} = { x \in E : s(x) = c_{i}} 라 두면 {E_{i}} 는 서로소이고 s 는 s = \sum_{i = 1}^{n} c_{i} \chi_{E_{i}} 같이 잴 수 있는 특성함수들의 선형결합으로 표시할 수 있다.

(정의) 정의된 단순함수가 s \ge 0 일때, 그 적분을 \int_{E} s = \sum_{i = 1}^{n} c_{i} m(E_{i}) 라 정의한다.

\int_{E} (s+t) = \int_{E} s + \int_{E} t

\int_{E} (cs) = c\int_{E} s

s \le t \implies \int_{E} s \le \int_{E} t

(정의) 잴 수 있는 함수 f : E \to [0, +\infty] 의 적분을 \infty_{E} f = sup{\infty_{E} s : 0 \le s \le f, s 는 단순함수}  로 정의한다.

0 \le g \le f \implies 0 \le \int g \le \int f

(정리 1.2.4) 임의의 잴 수 있는 함수 f : E \to [0,\infty] 는 단조증가하는 단순함수의 점별극한함수로 표시된다.

(따름정리 1.2.5) 임의의 잴 수 있는 함수 f : E \to [0, +\infty] 는, 적절한 양수열 \left \langle c_{n} \right \rangle 과 잴 수 있는 집합열 \left \langle E_{n} \right \rangle 에 대하여 f = \sum_{n = 1}^{\infty} c_{n} \chi_{E_{i}} 로 표시된다.

(정의) 함수 f : X \to \mathbb{R}^{*} 에 대하여 f_{+} (x) = max{f(x),0}, f_{-} (x) = - min{f(x),0}, x \in X 라 두면 f_{+}, f_{-} \ge 0 이고 f = f_{+} – f_{-} 이다. 만일 함수 f : E \to \mathbb{R}^{*} 가 잴 수 있으면 (명제 1.2.3)에 의하여 f_{+} 와 f_{-} 도 잴 수 있다. 

(정의) 함수 f 의 적분을 \int_{E} f = \int_{E} f_{+} - \int_{E} f_{-} 라 정의한다. 만일 함수 f_{+} 와 함수 f_{-} 의 적분값이 모두 무한이면 f의 적분을 정의하지 않는다.

(정의) 함수 f_{+}와 f_{-} 의 적분값이 모두 유한일 때, 함수 f 를 르벡적분 가능한 함수 혹은 L^{1}-함수라 부른다. 또한, 잴수 있는 집합 E 위에서 정의된 르벡적분 가능한 함수 전체의 집합을 L^{1} (E) 라 쓴다.

만일 f \le g 이면 \iint_{E} f \le \int_{E} g 이다.

만일 m(E) = 0 이면, 임의의 함수 f : E \to \mathbb{R}^{*} 가 잴 수 있고 \int_{E} f = 0 이다.

(정리 1.2.6) 서로소인 잴 수 있는 집합 모임 {A_{n} : n = 1,2, …} 에 대하여 A = \sqcup_{n = 1}^{\infty} A_{n} 이라 하자. 그러면 임의의 잴 수 있는 함수 f : A \to [0,\infty] 에 대하여 등식 \infty_{A} f = \sum_{n = 1}^{\infty} \int_{A_{n}} f 이 성립한다.

(따름정리 1.2.7) 잴 수 있는 함수 f 에 대하여 f \in L^{1} (E) 일 필요충분조건은 |f| \in L^{1} (E) 이고 이 때 부등식 |\int_{E} f| \le \int_{E} |f|  이 성립한다.

(정의) 잴 수 있는 집합 E 의 각 점 x \in E 에 관한 명제 P(x) 가 있을 때, m({x \in E : P(x) 가 성립하지 않는다}) = 0 이면 거의 모든 점에서 P(x) 가 성립한다고 한다.

(명제 1.2.8) 잴 수 있는 함수 f : E \to [0,\infty] 의 적분값이 유한이면 f는 거의 모든 점에서 유한값을 가진다.

(정의) 잴 수 있는 집합 E에서 정의된 복소함수 f : E \to \mathbb{C} 에 대해 함수 f = u + iv 의 실수부를 u, 허수부를 v라 하자. u와 v가 잴 수 있으면 f가 잴 수 있다고 한다.

만일 \int_{E} |f| 가 유한값이면 f를 르벡적분가능함수라 부른다.

(정의) 복소함수의 적분을 \int_{E} (u + iv) = \int_{E} u + i \int_{E} v 라 정의한다. 앞으로 L^{1}(E) 는 E에서 \mathbb{C} 로 가는 르벡적분가능함수 전체의 집합을 나타낸다.

L^{1}(E) 는 벡터공간이다.

\int_{E} (\alpha f) = \alpha \int_{E} f  f \in L^{1}(E), \alpha \in \mathbb{C}

|\int_{E} f| \le \int_{E} |f|

(따름정리 1.2.9) 서로소인 잴 수 있는 집합모임 {A_{n} : n = 1,2,…} 에 대하여 A = \sqcup_{n = 1}^{\infty} A_{n} 이라 하자. 그러면 임의의 f \in L^{1}(A) 에 대하여 \infty_{A} f = \sum_{n = 1}^{\infty} \int_{A_{n}} f 이 성립한다.

(명제 1.2.10) 잴 수 있는 집합 E에서 정의된 잴 수 있는 함수 f 에 대하여 다음이 성립한다.

만일 f \ge 0 이고 \inf_{E} f = 0 이면 거의 모든 점에서 f = 0 이다.

만일 f \in L^{1} (E) 이고 임의의 잴 수 있는 집합 D \subset E 에 대하여 \int_{D} f = 0 이면 거의 모든 점에서 f = 0이다.

(명제 1.2.11) 구간 [a,b] 위에서 함수 f : [a,b] \to \mathbb{R} 가 잴 수 있고, 모든 점 x 에 대하여 등식 \int_{[a,x]} f = 0 이 성립하면, 거의 모든 점에서 f = 0 이다.

(subsection 1.3) 적분의 수렴정리

(단조수렴정리)(정리 1.3.1) 잴 수 있는 집합 E에서 \mathbb{R}^{*} 로 가는 잴 수 있는 함수열 \left \langle f_{n} \right \rangle 이 다음 조건 0 \le f_{n} \le f_{n+1}, n = 1, 2, … 을 만족한다고 하자. 만일 각 x \in E 에 대하여 f(x) = lim_{n} f_{n}(x) 이면, \inf_{E} f = \lim_{n \to \infty} \int_{E} f_{n} 이 성립한다.

(정리 1.3.2) 잴 수 있는 집합 E에서 정의된 잴 수 있는 함수 f, g 에 대하여 다음이 성립한다.

만일 f, g \in L^{1}(E) 이면 f + g \in L^{1} (E) 이다. 또한 f, g \ge 0 이거나 f, g \in L^{1} (E) 이면 등식 \int_{E} (f + g) = \int_{E} f + \int_{E} g 이 성립한다.

만일 f \in L^{1}(E) 이고 \alpha \in \mathbb{C} 이면, \alpha f \in L^{1} (E) 이고 등식 \int_{E} (\alpha f) = \alpha \int_{E} f 이 성립한다.

(따름정리 1.3.3) 잴 수 있는 집합 E에서 [0,\infty] 로 가는 잴 수 있는 함수열 \left \langle f_{n} \right \rangle 에 대하여 f(x) = \sum_{n = 1}^{\infty} f_{n}(x) 라 정의하면, 등식 \int_{E} f = \sum_{n = 1}^{\infty} \int_{E} f_{n} 이 성립한다.

(파투) (정리 1.3.4) 잴 수 있는 집합 E에서 [0, + \infty] 로 가는 잴 수 있는 함수열 \left \langle f_{n} \right \rangle 에 대하여, 부등식 \int_{E} (\liminf_{n \to \infty} f_{n}) \le \liminf_{n \to \infty} \int_{E} f_{n} 이 성립한다.

(르벡 수렴정리)(정리 1.3.5) 잴 수 있는 집합 E 에서 \mathbb{C} 로 가는 잴 수 있는 함수열  \left \langle f_{n} \right \rangle 이 다음 조건을 만족한다고 하자.

각 n = 1,2, … 에 대하여 |f_{n}| \le g 인 g \in L^{1}(E) 가 존재한다.

각 x \in E 에 대하여 극한값 \lim_{n} f_{n}(x) 가 존재한다. 

이 때, f(x) = lim_{n} f_{n}(x) 라 두면, f \in L^{1}(E) 이고 등식 \lim_{n \to \infty} \int_{E} |f_{n} – f| = 0, \lim_{n \to \infty} \int_{E} f_{n} = \int_{E} f 이 성립한다.

(레비)(정리 1.3.6) 잴 수 있는 집합 E 에서 \mathbb{C} 로 가는 L^{1}-함수열  \left \langle f_{n} \right \rangle 에 대하여 \sum_{n = 1}^{\infty} \int_{E} |f_{n}| < \infty 이라 가정하자. 그러면 거의 모든 x \in E 에 대하여 급수 \sum_{n = 1}^{\infty} f_{n}(x) 가 절대수렴한다. 또한, 그 극한값을 f(x) = \sum_{n = 1}^{\infty} f_{n}(x) 라 두면 f \in L^{1}(E) 이고 그 적분값은 \int_{E} f = \sum_{n = 1}^{\infty} \int_{E} f_{n} 로 주어진다.

(명제 1.3.7) 열린구간 I, J 의 곱집합 I \times J 위에서 정의된 이변수함수 f : I \times J \to \mathbb{C} 가 주어져있다. 각 x \in I 에 대하여 일변수함수 y \mapsto f(x,y) 가  잴 수 있는 함수이고, I \times J 위에서 편도함수 D_{1}f 가 존재한다고 하자. 만일 조건 |D_{1}f(x,y)| \le g(y), x \in I 를 만족하는 적분가능함수 g \in L^{1}(J) 가 존재하면 등식 \frac{d}{dx} \int_{J} f(x,y) dy = \int_{J} D_{1}f(x,y)dy 이 성립한다.

(명제)  세 조건을 만족하는 함수 \mu : \mathcal{P}(\mathbb{R}) \to [0,\infty] 는 존재하지 않는다. 

만일 I 가 a, b를 양끝점으로 하는 구간이면 \mu(I) = |b – a| 이다.

임의의 x \in \mathbb{R} 와 S \ini \mathcal{R} 에 대하여 \mu(x + S) = \mu(S)이다.

\biggl( \bigsqcup_{n = 1}^{\infty} E_{n} \biggr) = \lim_{n \to \infty} \mu(E_{n})

(명제 1.3.6) 집합 E \subset \mathbb{R} 의 모든 부분집합이 잴 수 있으면 \mu(E) = 0 이다.

(subsection 1.4) 리만적분과 르벡적분

(정의) 유계함수 f : [a,b] \to [0, \infty] 와 분할 P = {x_{0}(=a) , x_{1}, …, x_{n} (=b)} 및 i = 1,2, …, n 에 대하여 M_{i} = \sup{f(x) : x_{i-1} \le x \le x_{i}}, m_{i} = \inf{f(x) : x_{i-1} \le x \le x_{i}} 라 두고, 두 단순함수 U_{p} 와 L_{p} 를 U_{p} = f(a)_{ \chi_{{a}}} + \sum_{i = 1}^{n} M_{i\chi_{(x_{i-1}, x_{i}\rbrack}}, L_{p} = f(a)_{ \chi_{{a}}} + \sum_{i = 1}^{n} m_{i\chi_{(x_{i-1}, x_{i}\rbrack}}

(정의)상합과 하합을 U_{a}^{b} (f,P) = \int_{[a,b]} U_{p} , L_{a}^{b} (f,P) = \int_{[a,b]} L_{p} 와 같이 쓸 수 있다. 구간 [a,b]의 분할 전체의 집합을 \mathcal{P}[a,b] 라 두고 f의 리만 상적분과 리만 하적분을 각각 \overline{\int_{a}^{b} f }= \inf{ U_{a}^{b} (f,P)  : P \in \mathcal{P}[a,b] }, \underline{ \int_{a}^{b} f }= \sup{ L_{a}^{b} (f,P)  : P \in \mathcal{P}[a,b] } 와 같이 정의한다.

(정의) \lVert P \rVert := max{|y_{i} – y_{i-1}| : i = 1,2,…,m} 이라 정의하고 \lVert P_{n} \rVert 이 되도록 분할열 \langle P_{n} \rangle 을 잡으면 lim_{n \to \infty} U(f,P_{n}) = \overline{\int_{a}^{b} f } 이다. lim_{n \to \infty} L(f,P_{n}) = \underline{\int_{a}^{b} f } 이다. 만일  \underline{\int_{a}^{b} f } = \overline{\int_{a}^{b} f } 이면 f가 리만적분가능하다고 하고 그 공통값을  \int_{a}^{b} f 라 쓴다.

(정리 1.4.1) 유계함수 f : [a,b] \to \mathbb{R} 에 대하여 다음이 성립한다.

만일 f 가 리만적분가능하면 f 는 잴 수 있고, 등식 \int_{[a,b]} f = \int_{a}^{b} f 이 성립한다.

함수 f 가 리만적분가능할 필요충분조건은 거의 모든 점에서 연속임이다.

