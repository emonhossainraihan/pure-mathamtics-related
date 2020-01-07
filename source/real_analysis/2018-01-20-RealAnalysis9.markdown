---



layout: post



title : (Real Analysis 실해석) 삼각급수



date : 2018-01-20 08:53:24 +0900



---

(section 9) 삼각급수

(subsection 9.1) 푸리에-스틸체스 변환

(정의) 주기함수의 푸리에변환 f \mapsto \hat{f} : L^{1}(\mathbb{T}) \to c_{0}(\mathbb{Z}) 는 노음감소 단사 중동형이다. 그 치역은 c_{0}(\mathbb{Z}) 의 점별곱하기에 대하여 닫혀있는데, 이를 A(\mathbb{Z}) 라 쓰고 푸리에대수라 부른다. 또한 \hat{f} \in \mathcal{l}^{1}(\mathbb{Z}) 인 f \in L^{1}(\mathbb{T}) 전체의 집합을 A(\mathbb{T}) 라 쓰자. 그러면 임의의 f \in A(\mathbb{T}) 가 연속함수임을 알고 있으므로. 이를 요약하면 다음과 같다.

\begin{matrix} f & \in & A(\mathbb{T}) & \subset & C(\mathbb{T}) & \subset & \L^{2}(\mathbb{T}) & \subset & \L^{1}(\mathbb{T}) & & \\ \updownarrow & & \updownarrow & & \updownarrow & &\updownarrow & & \updownarrow & & \\ \hat{f} &\in & \mathcal{l}^{1}(\mathbb{Z}) & \subset  & \mathfrak{X} & \subset & \mathcal{l}^{2}(\mathbb{Z}) & \subset & A(\mathbb{Z}) & \subset & c_{0} (\mathbb{Z}) \end{matrix}

대응관계 L^{2}(\mathbb{T}) \leftrightarrow \mathcal{l}^{2}(\mathbb{Z}) 는 내적이 보존되는 힐버트공간 동형사상이다.

(정의) 대응관계 A(\mathbb{T}) \leftrightarrow \mathcal{l}^{1}(\mathbb{Z}) 를 살펴보자. 각 a \in \mathcal{l}^{1}(\mathbb{Z}) 에 대하여 \hat{a} (t) = \sum_{n = -\infty}^{\infty} a(n)e^{-int} , t \in \mathbb{T} 라 정의하면 \hat{a} 는 연속함수가 되므로 선형사상 a \mapsto \hat{a} : \mathcal{l}^{1} (\mathbb{Z}) \to C(\mathbb{T}) 를 얻는다. 이 사상의 치역은 A(\mathbb{T}) 가 된다. 이 선형사상은 \mathcal{l}^{1}(\mathbb{Z}) 의 푸리에변환이라 불린다.

(정의) 국소옹골공간 X에서 정의된 유계연속함수 전체의 벡터공간을 C^{b}(X) 라 쓰면 f \mapsto \| f \|_{sup} 는 이 공간의 노음이 된다. 만일 X가 이산공간이면 c^{b}(X) 라 쓴다. 따라서 \mu \mapsto \hat{\mu} : M(\mathbb{T}) \to c^{b}(\mathbb{Z}) 는 노음감소 선형사상이 되는데, 이를 푸리에-스틸체스 변환이라 부른다.

이 변환을 L^{1}(\mathbb{T}) 로 제한하면 푸리에 변환을 얻는다.

(정의) 두 복소측도 \mu, \nu \in M(\mathbb{T}) 에 대하여 C(\mathbb{T}) 의 선형범함수를 h \mapsto \int_{\mathbb{T} \times \mathbb{T}} h(s + t) d( \mu \times \nu)(s,t) , h \in C(\mathbb{T}) 와 같이 정의하자. 이는 C(\mathbb{T}) 의 유계선형범함수가 되는데, 이에 대응하는 복소측도를 \mu * \nu \in M(\mathbb{T}) 라 쓴다. 

다음 부등식 \| \mu * \nu \| \le \| \mu \| \| \nu \| , \mu, \nu \in M(\mathbb{T}) 이 성립한다.

(정의) 만일 \mu, \nu \in M(\mathbb{T}) 가 절대연속측도이고 각각 f , g \in L^{1}(\mathbb{T}) 에 대하여 d \mu (s) = f(s) ds 와 d \nu (t) = g(t)dt 로 각각 표현되면, d(\mu \times \nu) = (f * g) dm 이 된다. 따라서, 측도의 곱하기 \mu * \nu 를 L^{1}(\mathbb{T}) 에 제한하면 L^{1}- 함수의 곱하기가 된다.

(명제) 정규보렐측도공간 M(\mathbb{T}) 는 항등원을 가지는 바나하대수이고, L^{1}(\mathbb{T}) 는 M(\mathbb{T}) 의 이데알이다.

L^{1}(\mathbb{T}) 는 M(\mathbb{T}) 의 이데알이라 함은, f \in L^{1}(\mathbb{T}) 이고 \mu \in M(\mathbb{T}) 이면 f * \mu \in L^{1} (\mathbb{T}) 임을 뜻한다.

(정의) \mu, \nu \in M(\mathbb{T}) 와 각 n \in \mathbb{Z}) 에 대하여 푸리에-스틸체스 변환은 M(\mathbb{T}) 에서 c^{b}(\mathbb{Z}) 로 가는 준동형이 된다. 따라서, 이 변환의 치역이 점별곱하기에 닫혀있는데, 이를 푸리에-스틸체스 대수라 부르고, B(\mathbb{Z}) 라 쓴다.

(정리 9.1.2) 푸리에-스틸체스 변환 \mu \mapsto \hat{\mu} 는 M(\mathbb{T}) 에서 c^{b}(\mathbb{Z}) 로 가는 노음감소 단사 준동형이다.

(정의) 지금부터 f \in C(\mathbb{T}) 와 \mu \in M(\mathbb{T}) 에 대하여 \langle f, \mu \rangle = \int_{\mathbb{T}} f d \mu 라 쓴다. 

(명제) 임의의 f \in C(\mathbb{T}) 와 \mu \in M(\mathbb{T}) 에 대하여 \lim_{n \to \infty} \sum_{k = -n}^{n} ( 1- \frac{|k|}{n+1}) \hat{f}(k) \hat{\mu}(-k) = \lim_{n \to \infty} \langle K_{n} * f , \mu \rangle = \langle f, \mu \rangle 이다.

\langle P , \mu \rangle = \sum_{k} \hat{P} (k) \hat{\mu} (-k) , P \in T(\mathbb{T}) , \mu \in M(\mathbb{T}) 이다.

(정의) 삼각다항식은 연속함수로 이해할 수도 있지만 측도로 이해할 수도 있다. 삼각다항식 P를 측도로 이해하는 경우 그 노음을 \| P \|_{M(\mathbb{T})} 라 쓴다. 

(정리 9.1.3) 함수 a : \mathbb{Z} \to \mathbb{C} 에 대하여 다음은 동치이다.

a \in B(\mathbb{Z}) 이다.

임의의 P \in T(\mathbb{T}) 에 대하여 |\sum_{k} \hat{P}(k) a(-k)| \le M \| P \|_{sup} 이 성립하는 상수 M 이 존재한다.

M’ := \sup_{n \in \mathbb{N}} \| \sum_{k = -n}^{n} (1-\frac{|k|}{n+1}) a(k) u_{k} \|_{M(\mathbb{T}} < \infty 이다.

(명제) a \in B(\mathbb{Z}) 이고 \hat{\mu} = a 인 경우, d \mu_{n} = [\sum_{k = -n}^{n} (1-\frac{|k|}{n+1}) \hat{\mu}(k) u_{k}] dm 으로 정의된 측도 \mu_{n} 을 생각하면 \lim_{n \to \infty} \langle f, \mu_{n} \rangle = \langle f, \mu \rangle, f \in C(\mathbb{T}) 를 얻는다. 측도는 C(\mathbb{T}) 에서 정의된 선형범함수이므로, 이는 측도열 \langle \mu_{n} \rangle 이 \mu 로 점별수렴함을 말한다.

(정의) 함수 a : \mathbb{Z} \to \mathbb{C} 가 성질 c_{1}, c_{2}, …, c_{k} \in \mathbb{C}, n_{1}, …, n_{k} \in \mathbb{Z} \implies \sum_{i,j =1}^{k} a(n_{i} – n_{j}) c_{i}\hat{c}_{j} \ge 0 을 만족하면 이를 양부호수열이하 부른다.

(헬그로츠)(정리 9.1.4) 함수 a : \mathbb{Z} \to \mathbb{C} 가 양부호수열일 필요층분조건은 a가 양측도의 푸리에-스틸체스 변환임이다.

(정의) 정수집합에서 정의된 양부호수열 전체의 집합을 P(\mathbb{Z}) 라 쓴다. 이 때, P(\mathbb{Z}) 가 더하기와 양수곱에 의하여 닫혀있음은 자명하다.

임의의 \mu \in M(\mathbb{T}) 가 양측도들의 선형결합으로 쓸 수 있음을 알고 있으므로, 다음 관계 B(\mathbb{Z}) = {(a_{1} – a_{2}) + i(a_{3} – a_{4}) : a_{i} \in P(\mathbb{Z}) } 가 성립함을 알 수 있다.

(subsection 9.2) 푸리에-쉬와르츠 변환

(정의) 무한번 미분가능하고 주기가 2 \pi 인 주기함수 전체의 집합을 \mathcal{D}(\mathbb{T}) 라 둔다. 

(정의) 함수 a : \mathbb{Z} \to \mathbb{C} 가 성질 \sup{|n|^{p} |a(n)| : n \in \mathbb{Z}} < \infty , p = 1,2, … 를 만족하면, 이를 빠른감소수열이라 부른다. 즉, f \in \mathcal{D} (\mathbb{T}) 이면 \hat{f} 는 빠른감소수열이다.

(정의) \mathcal{D}(\mathbb{T}) 에 거리를 정의한다. d(f,g) = \sum_{p = 0}^{\infty} \frac{2^{-p} \| D^{p} f – D^{p} g \|_{sup}}{1 + \| D^{p} f – D^{p} g \| } = , f,g \in \mathcal{D}(\mathbb{T}) 라 정의한다.

(명제 9.2.1) 벡터공간 \mathcal{D} (\mathbb{T}) 의 함수열 \langle f_{n} \rangle 과 f \in \mathcal{D} (\mathbb{T}) 에 대하여 다음은 동치이다.

\lim_{n \to \infty} d(f_{n}, f) = 0 이다.

각 p = 0,1,… 에 대하여 \langle D^{p} f_{n} \rangle 이 D^{p} f 로 고르게 수렴한다.

임의의 양수 \epsilon >0 에 대하여 n \ge N, p < \frac{1}{\epsilon} \implies \| D^{p}f_{n} – D^{p} f \|_{sup} < \epsilon 이 성립하는 자연수 N 이 존재한다.

(명제 9.2.2) 푸리에변환 f \mapsto \hat{f} 는 \mathcal{D}(\mathbb{T}) 에서 빨리감소하는 수열 전체의 벡터공간으로 가는 전단사대응이다. 또한 각 f \in \mathcal{D} (\mathbb{T}) 에 대하여 \lim_{n \to \infty} d(f, \sum_{k = -n}^{n} \hat{f} (k) u_{k}) = 0 이 성립한다.

(명제) d(f + h, g+h) = d(f,g) , f,g,h \in \mathcal{D} (\mathbb{T}) . 두 점을 나란히 평행이동해도 그 거리가 변하지 않는다.

\mathcal{D}(\mathbb{T}) 의 더하기가 (f_{0}, g_{0}) \in \mathcal{D}(\mathbb{T}) \times \mathcal{D}(\mathbb{T}) 에서 연속임을 알 수 있다.

(정의) 각 P = 0,1,2, … 에 대하여 \| f \|_{P} = max{\| D^{p} f \|_{sup} : p = 0,1,2, …, P }, f \in \mathcal{D} (\mathbb{T}) 라 정의하면 이는 벡터공간 \mathcal{D} (\mathbb{T}) 의 노음이 되므로, N_{p} = {f \in \mathcal{D} (\mathbb{T}) : \| f \|_{P} \le 2^{-P}} 는 볼록집합이 된다.

(정의) 위상공간의 한 점 x의 근방들의 모임 \mathcal{N} 이 있을 때, 임의의 x를 포함하는 열린집합 V 에 대하여 x \in N \subset V 가 되는 N \in \mathcal{N} 이 존재하면 \mathcal{N}을 점 x의 국소위상기저 혹은 국소기저라 부른다. 

\mathcal{D} (\mathbb{T}) 의 볼록집합들의 모임 {N_{p} : P = 0,1,2,…} 는 원점의 국소기저가 된다.

(정의) 평행이동은 위상동형사상이므로, 원점의 국소기저를 평행이동하면 각 점의 국소기저를 얻을 수 있다. 원점의 국소기저를 그냥 국소기저라 부른다. 근방이란 0의 근방을 말한다.

(정의) 벡터공간 X에 평행이동에 불변인 거리가 있어서 완비공간이 되고 볼록집합으로 이루어진 국소기저를 가지면 이를 프레쉐 공간이라 부른다. 

\mathcal{D} (\mathbb{T}) 는 프레쉐 공간이다. 임의의 바나하공간은 프레쉐 공간이다.

(정의) \mathcal{D} (\mathbb{T}) 에 정의된 연속선형범함수 전체의 벡터공간을 \mathcal{D}’ (\mathbb{T}) 라 쓰자. 이는 관계 P \le Q \implies (\mathcal{D} (\mathbb{T}), \| \|_{P})^{*} \subset (\mathcal{D} (\mathbb{T}), \| \|_{Q})^{*} \subset \mathcal{D}’ (\mathbb{T}) 이다.

(정리 9.2.3) 벡터공간 \mathcal{D} (\mathbb{T}) 의 선형범함수 \phi 에 대하여 다음은 동치이다.

\phi 가 거리공간 (\mathcal{D} (\mathbb{T}), d) 에서 \mathbb{C} 로 가는 연속함수이다.

적절한 양수 C>0 와 자연수 P 에 대하여 다음 f \in \mathcal{D} (\mathbb{T}) \implies |\phi (f)| \le C \| f \|_{P} 이 성립한다.

(정의) \phi \in \mathcal{D}’ (\mathbb{T}) 와 f \in \mathcal{D} (\mathbb{T}) 에 대하여 \langle f, \phi \rangle  = \phi (f) 라 쓰기로 약속한다.

각 \phi \in \mathcal{D}’ (\mathbb{T}) 와 f \in \mathcal{D} (\mathbb{T}) 에 대하여 (\phi \boxtimes f) (t) = \langle f_{-t} , \phi \rangle , t \in \mathbb{T} 라 정의한다.

(정의) \phi \boxtimes f \in \mathcal{D} (\mathbb{T}) 임을 알 수 있다. 따라서, 각 \phi, \psi \in \mathcal{D} ‘ (\mathbb{T}) 에 대하여 \langle f, \phi * \psi \rangle = \langle \psi \boxtimes f , \phi \rangle , f \in \mathcal{D} (\mathbb{T}) 와 같이 정의할 수 있다.

(정의) \phi, \phi_{n} 이 \mathcal{D} (\mathbb{T}) 의 선형범함수일 때, \lim_{n \to \infty} \langle f, \phi_{n} \rangle = \langle f , \phi \rangle , f \in \mathcal{D} (\mathbb{T}) 가 성립하면 \langle \phi_{n} \rangle 이 \phi 로 수렴한다고 정의하고, 이를 \phi_{n} \to \phi 라 쓴다.

(명제 9.2.4) 만일 각 n = 1,2, … 에 대하여 \phi _{n} \in \mathcal{D} ‘ (\mathbb{T}) 이고 \phi_{n} \to \phi 이면 \phi \in \mathcal{D} ‘ (\mathbb{T}) 이다.

(고른유계원칙) (정리 9.2.5) 프레쉐공간 X 에서 정의된 연속선형범함수열 \langle \phi_{k} \rangle 가 주어져 있고, 각 x \in X 에 대하여 \phi (x) = \lim_{k \to \infty} \phi_{k} (x) 이면 \phi 도 연속선형범함수이다.

(정의) 각 \phi \in \mathcal{D} ‘ (\mathbb{T}) 에 대하여 \hat{\phi} (n) = \langle u_{-n}, \phi \rangle , n \in \mathbb{Z} 라 정의하자. 각 n \in \mathbb{Z} 에 대하여 \hat{\phi * \psi }(n) = \hat{\phi} (n) \hat{\psi} (n) 이 성립한다.

(정의) 함수 a : \mathbb{Z} \to \mathbb{C} 가 있을 떄, 적절한 자연수 p 에 대하여 n \mapsto |n|^{-p} a(n) 이 유계이면 이를 슬슬증가수열이라 한다. 

슬슬증가수열 전체의 벡터공간이 점별곱하기에 대하여 닫혀있다.

따라서 \phi \mapsto \hat{\phi} 는 \mathcal{D} ‘ (\mathbb{T}) 에서 슬슬증가수열 전체의 집합으로 가는 준동형인데, 이를 푸리에-쉬와르츠 변환이라 한다.

(명제) 임의의 수열 a : \mathbb{Z} \to \mathbb{C} 에 대하여 삼각다항식 \phi_{n} = \sum_{k = -n}^{n} a(k) u_{k} , n = 1,2, … 라 하자. 각 m \in \mathbb{Z} 와 n = 1,2, … 에 대하여 \langle u_{m}, \phi_{n} \rangle = \sum_{k = -n}^{n} a(k) \langle u_{m}, u_{k} \rangle = \begin{cases} a(-m) & |m| \le n \\ 0 & |m| > n \end{cases} 임을 알 수 있다.

(정리 9.2.6) 푸리에-쉬와르츠 변환은 \mathcal{D} ‘ (\mathbb{T}) 에서 슬슬증가하는 수열 전체의 대수로 가는 전단사 준동형이다.

(명제) ‘빨감’ , ‘슬증’ 이 빠른감소수열 과 슬슬증가수열 전체의 공간을 나타낼 때, \begin{matrix} \mathcal{D} (\mathbb{T}) & \subset & C(\mathbb{T}) & \subset & \L^{2}(\mathbb{T}) & \subset & M(\mathbb{T}) & \subset & \mathcal{D} ‘ (\mathbb{T})  \\ \updownarrow & & \updownarrow & & \updownarrow & &\updownarrow & & \updownarrow \\ 빨감 & \subset  & \mathfrak{X} & \subset & \mathcal{l}^{2}(\mathbb{Z}) & \subset & B(\mathbb{Z}) & \subset & 슬증 \end{matrix}

로 나타낼 수 있다. C(\mathbb{T}) 의 쌍대공간이 M(\mathbb{T}) 이고, \mathcal{D} (\mathbb{T}) 의 쌍대공간이 \mathcal{D} ‘ (\mathbb{T}) 이다.

(subsection 9.3) 약위상

(정의) 프레쉐공간 X 에서 정의된 모든 연속선형범함수 전체의 벡터공간을 X^{*} 라 쓰고, 기호 \langle x, \phi \rangle = \phi(x) , x \in X , \phi \in X^{*} 를 그대로 유지한다.

(정의) 복소평면 \mathcal{C} 는 이미 위상공간이므로 \mathcal{C} ^{X} 도 곱위상을 생각함으로써 위상공간이 되고, X^{*} 를 \mathcal{C}^{X} 의 부분위상공간으로 이해할 수 있다 따라서 X^{*} 의 위상은 {\phi \in X^{*} : \langle x, \phi \rangle \in U} , x \in X, 열린집합 U \subset \mathbb{C} 을 포함하는 최소의 위상인데, 이렇게 정의된 X^{*} 의 위상을 약^{*}-위상이라 한다.

복소평면이 하우스도르프공간이므로 그 곱공간 \mathcal{C}^{X} 의 부분공간 X^{*} 도 하우스도르프 공간이다.

(명제) X^{*} 의 약^{*} -위상 은 모든 선형범함수 \Lambda_{x} (단, x \in X) 가 연속이 되도록 하는 최소의 위상이다.

(정의) 임의의 집합 A \subset X 에 대하여 A^{ \bullet } = {\phi \in X^{*} : |\phi (x)| \le 1 (x \in A) } 라 정의하자. 

(명제) 각 유한집합 F \subset X 에 대하여 \phi _{0} + F^{ \bullet } 을 다 모으면 이는 약^{*} -위상에 관한 \phi_{0} \in X^{*} 의 국소기저가 된다. 집합모임 {F^{\bullet} : F \subset X, F 는 유한집합} 은 원점의 국소기저가 된다.

(정의) 벡터공간 의 부분집합 A, B 와 스칼라 \alpha \in \mathbb{C} 에 대하여 A + B = {x + y : x \in A, y \in B} , \alpha A = { \alpha x : x \in A } 라 정의한다. 벡터공간 X 에 위상이 주어지고 더하기와 스칼라곱이 연속이면 이를 위상벡터공간이라 한다.

힐버트공간이나 바나하공간, 프레쉐공간은 모두 위상벡터공간이 된다.

(정의) 위상벡터공간 X에서 정의된 연속선형범함수들의 벡터공간을 X^{*} 라 쓰고, 이를 X의 쌍대공간이라 한다. 벡터공간 X^{*} 에 약^{*} -위상이 부여된 위상벡터공간을 X^{*w} 로 표시하자.

(명제 9.3.1) 위상벡터공간 X의 쌍대공간 X^{*w} 의 그물 \langle \phi_{i} : i \in I \rangle 와 \phi 가 있을 때, \lim_{i} \phi_{i} = \phi 일 필요충분조건은 \lim_{i} \langle x, \phi_{i} \rangle = \langle x , \phi \rangle , x \in X 이다.

(정의) 위상벡터공간의 쌍대공간에 주어진 약^{*} -위상은 국소기저 F^{ \bullet } 가 모두 볼록집합이다. 이와 같이 볼록집합으로 이루어진 국소기저를 가지는 위상벡터공간을 국소볼록공간이라 한다.

(바나하-알라오글루) (정리 9.3.2) 위상벡터공간의 근방 V 에 대하여 V^{\bullet} 는 약^{*} -위상에 관하여 옹골집합이다.

(정의) 벡터공간의 볼록집합 C 와 점 x \in C 에 대하여, 다음 조건이 성립할 때 x를 C의 꼭지점이라 부른다.

y,z \in C , x = ty + (1-t)z, 0 < t < 1 \implies x = y = z 

(정의) 벡터공간의 점 x가 {x_{1}, …, x_{n}} 의 볼록결합이라는 말은 x = t_{1}x_{1}, …, t_{n}x_{n} , t_{1} + … + t_{n} = 1 , t_{i} \ge 0 ( i = 1, … , n) 을 만족하는 실수 t_{1}, …, t_{n} \in [0,1] 이 존재함을 뜻한다.

(명제) (크라인-밀만정리) 국소볼록공간에서 임의의 볼록옹골집합은 항상 꼭지점을 가지고 있으며 그 꼭지점들의 볼록결합을 모두 모으면 원래 볼록집합의 조밀한 부분집합이 된다.

(명제 9.3.3) 바나하공간 X가 다른 바나하공간 Y의 쌍대공간이라 하자. 그러면 단위공 \bar{X_{1}} = {x \in X : \| x \| \le 1} 이 꼭지점을 가진다.

따라서 바나하공간 L^{1}(\mathbb{T}) 의 단위공에는 꼭지점이 없으므로 이로부터 L^{1}(\mathbb{T}) 에는 약^{*} -위상을 정의하는 것이 불가능하는 것을 알 수 있다.

