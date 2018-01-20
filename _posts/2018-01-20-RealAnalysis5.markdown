---



layout: post



title : 푸리에 변환



date : 2018-01-20 08:52:44 +0900



---

(section 5) 푸리에 변환

(subsection 5.1) 푸리에 급수

(정의) 실수군 \mathbb{R} 을 부분군 {2\pi n : n = 0, \mp 1, \mp 2,…} 으로 나눈 몫을 \mathbb{T} 라 두고, 실수축의 거리를 그대로 쓴다. \int_{\mathbb{T}} f = \frac{1}{2\pi} \int_{-\pi}^{\pi} f(x)dx 라 정의한다.

(정의) 각 f,g : \mathbb{T} \to \mathbb{C} 와 t \in \mathbb{T} 에 대하여 (f*g)(t) = \int_{\mathbb{T}} f(s)g(t-s) ds 라 정의한다. 그러면 L^{1}(\mathbb{T}) 는 바나하대수가 된다.

(정의) 각 f \in L^{1}(\mathbb{T}) 와 정수 n = 0, \mp 1, \mp 2, … 에 대하여 \hat{f}(n) = \int_{\mathbb{T}} f(t)e^{-int}dt 라 정의하면 |\hat{f}(n)| \le \lVert f \rVert_{1} 이다. 

(정의) 각 n = 0, \mp 1, \mp 2, …., 에 대하여 u_{n}(t) = e^{int} , t\in \mathbb{T} 라 두면 관계식 u_{n} * f = \hat{f}(n)u_{n} , n \in \mathbb{Z}, f \in L^{1}(\mathbb{T}) 이 바로 확인되는데, 특히 (u_{n} * f)(0) = \hat{f}(n) 이다. 또한 다음이 성립한다.

\hat{u_{n}}(m) = \begin{cases}1&m = n \\ 0, m \neq n \end{cases}

(정의) 무한급수 \sum_{n = -\infty}^{\infty} \hat{f}(n) u_{n} 을 f \in L^{1}(\mathbb{T}) 의 푸리에급수라 부르고, 그 계수 {\hat{f}(n) : n \in \mathbb{Z}} 를 f의 푸리에계수라 부른다.

(명제 5.1.1) 각 f, g \in L^{1}(\mathbb{T}) 및 상수 a,b \in \mathbb{C} 와 n \in \mathbb{Z} 에 대하여 등식들 \hat{af + bg}(n) = a\hat{f}(n) + b\hat{g}(n), \hat{f * g} (n) = \hat{f}(n) \hat{g}(n) 이 성립한다. 또한, 각 t \in \mathbb{T} 에 대하여 다음 등식 \hat{f_{t}}(n) = \hat{f}(n) u_{n}(-t), n \in \mathbb{Z} 이 성립한다.

(명제 5.1.2) 만일 f 가 주기 2\pi 인 미분가능함수고 f’ \in L^{1}(\mathbb{T} 이면 등식 \hat{f’}(n) = in \hat{f}(n), n \in \mathbb{Z} 이 성립한다.

(정리 5.1.3) 각 p \in [1,\infty) 에 대하여, 연속함수공간 C(\mathbb{T}) 는 L^{p}(\mathbb{T})의 조밀한 부분공간이다.

(정의) 집합 \mathbb{T} 에서 정의된 함수 f 와 t \in \mathbb{T} 에 대하여, 그 평행이동을 f_{t}(s) = f(s-t), s \in \mathbb{T} 라 정의한다.

(정리 5.1.4) 각 함수 f \in L^{p}(\mathbb{T}) 에 대하여 (단, 1 \le p < \infty) 함수 t \mapsto f_{t} : \mathbb{T} \to L^{p}(\mathbb{T}) 는 고른연속함수이다.

(정리 5.1.5) 함수열 \langle h_{n} \rangle 이 다음 성질 h_{n} \ge 0, \int_{\mathbb{T}} h_{n} = 1, lim_{n \to \infty} \int_{\mathbb{T}\setminus[-\delta,\delta]} h_{n} = 0 (0 < \delta < \pi) 를 만족하면, 임의의 f \in L^{1}(\mathbb{T}) 에 대하여 lim_{n \to \infty} \lVert f – h_{n} * f \rVert_{1} = 0 이 성립한다.

(정리 5.1.6) 함수열 \langle h_{n} \rangle 이 성질  h_{n} \ge 0, \int_{\mathbb{T}} h_{n} = 1, lim_{n \to \infty} \int_{\mathbb{T}\setminus[-\delta,\delta]} h_{n} = 0 (0 < \delta < \pi) 을 만족하면, 임의의 f \in C(\mathbb{T}) 에 대하여 lim_{n \to \infty} lim_{n \to \infty} \lVert f – h_{n} * f \rVert_{\infty} = 0 이 성립한다.

(정의) 각 n = 1, 2, … 에 대하여 K_{n} = \sum_{k = -n}^{n} (1-\frac{|k|}{n+1}) u_{k} 이라 정의했을 때, \langle K_{n} \rangle 을 페제르 핵이라 한다. 이는 성질 h_{n} \ge 0, \int_{\mathbb{T}} h_{n} = 1, lim_{n \to \infty} \int_{\mathbb{T}\setminus[-\delta,\delta]} h_{n} = 0 (0 < \delta < \pi) 을 모두 만족한다.

(정의) {u_{n} : n \in \mathbb{Z} }의 유한선형결합으로 표시되는 함수를 삼각다항식이라 부르고, 삼각다항식의 벡터공간을 T(\mathbb{T}) 라 쓴다. 삼각다항식 P = \sum_{n = -N}^{N} a_{n}u_{n} 의 푸리에계수 \hat{P} (n) = a_{n} 으로 주어진다.

(정리 5.1.7) 함수공간 T_{\mathbb{T}} 는 L^{1}(\mathbb{T})의 조밀한 부분공간이다.

(정리 5.1.8) 만일 f \in L^{1}(\mathbb{T}) 이고 \hat{f} = 0 이면 거의 모든 점에서 f = 0 이다.

(따름정리 5.1.9) 만일 f \in L^{1}(\mathbb{T}) 이고 \hat{f} \in \mathcal{l}^{1}(\mathbb{Z}) 이면, 거의 모든 점 t \in \mathbb{T} 에서 등식 f(t) = \sum_{n \in \mathbb{Z}} \hat{f}(n) e^{int} 이 성립한다.

(리만-르벡) (정리 5.1.10) 각 f \in L^{1}(\mathbb{T}) 에 대하여 lim_{n \to \mp \infty} \hat{f} (n) = 0 이 성립한다.

(정의) 정수집합에서 정의된 함수 a : n \mapsto a(n) 가운데 lim_{n \to \mp \infty} a(n) = 0 인 것 전체의 벡터공간을 c_{0}(\mathbb{Z}) 라 쓰고, \mathcal{l}^{\infty}(\mathbb{Z}) 의 노음을 그대로 사용한다.

(정리 5.1.11) 변환 f \mapsto \hat{f} 는 바나하대수 L^{1}(\mathbb{T}) 에서 c_{0}(\mathbb{Z}) 로 가는 노음감소 일대일 선형사상이다.

(정의) 두 함수 a, b \in c_{0}(\mathbb{Z}) 에 대하여 그 곱 a,b 를 (ab)(n) = a(n)b(n) , n \in \mathbb{Z} 라 정의하면 c_{0}(\mathbb{Z}) 는 바나하대수가 된다. 따라서 (정리 5.1.11)의 변환은 바나하대수 사이의 정의된 선형사상으로 곱하기를 보존한다. 이를 준동형이라 한다.

(따름정리 5.1.12) 함수공간 T(\mathbb{T}) 는 C(\mathbb{T}) 의 조밀한 공간이다.

(따름정리 5.1.13) 함수공간 T(\mathbb{T}) 는 L^{p}(\mathbb{T}) (단, 1 \le p < \infty)의 조밀한 공간이다.

(바이에르쉬트라스) (정리 5.1.14) 구간 [0,1] 위에서 다항식으로 정의된 함수들의 공간은 C[0,1] 에서 조밀하다.

(subsection 5.2) 푸리에적분

(정의) 임의의 f \in L^{1}(\mathbb{R}) 과 \alpha \in \mathbb{R} 에 대하여 푸리에적분 \hat{f} (\alpha) 를 \hat{f}(\alpha) = \int_{\mathbb{R}} f(x)e^{-i \alpha x} dx 과 같이 정의한다. 그러면 |\hat{f} (\alpha )| \le \lVert f \rVert_{1} , \alpha \in \mathbb{R} 이 성립한다.

(정의) 임의의 f \in L^{1}(\mathbb{R}) 에 대하여 \hat{f} 는 유계연속함수가 되는데, \hat{f} 를 f 의 푸리에변환이라 한다. 각 \alpha \in \mathbb{R} 에 대하여 u_{\alpha}(x) = e^{i \alpha x} , x \in \mathbb{R} 로 나타내면 등식 u_{\alpha} * f = \hat{f} (\alpha) u_{\alpha}, \alpha \in \mathbb{R} 이 성립한다.

(명제 5.2.1) 각 f, g \in L^{1}(\mathbb{R}) 및 상수 a,b \in \mathbb{C} 와 n \in \mathbb{Z} 에 대하여 등식들 \hat{af + bg}(n) = a\hat{f}(n) + b\hat{g}(n), \hat{f * g} (n) = \hat{f}(n) \hat{g}(n) , \alpha \in \mathbb{R} 이 성립한다. 또한, 각 \alpha \in \mathbb{R} 에 대하여 다음 등식 \hat{f u_{\alpha}} = (\hat{f})_{\alpha} , \hat{f_{x}}(\alpha) = \hat{f}(\alpha) u_{\alpha}(-x), x \in \mathbb{R} 이 성립한다.

(명제 5.2.2) 함수 f \in L^{1}(\mathbb{R}) 에 대하여 다음이 성립한다.

각 x \in \mathbb{R} 에 대하여 g(x) = -ixf(x) 라 정의하였을 때, 만일 g \in L^{1}(\mathbb{R}) 이면 \hat{f} 가 미분가능하고 등식 \hat{f}’ (\alpha) = \hat{g}(\alpha) , \alpha \in \mathbb{R} 이 성립한다.

만일 f 가 미분가능하고 f’ \in L^{1}(\mathbb{R}) 이면 등식 \hat{f’} (\alpha) = i \alpha \hat{f} ( \alpha ), \alpha \in \mathbb{R} 이 성립한다.

(정리 5.2.3) 각 f \in L^{1}(\mathbb{R}) 에 대하여 \hat{f} \in C_{0}(\mathbb{R}) 이다.

(정리 5.2.4) 함수모임 { h_{\lambda} : \lambda \in (0, \infty) } 이 다음 성질 h_{\lambda} \ge 0, \int_{\mathbb{R}} h_{\lambda} = 1, lim_{\lambda \to \infty} \int_{\mathbb{R}\setminus[-\delta,\delta]} h_{\lambda} = 0 (0 < \delta ) 를 만족하면 다음이 성립한다.

임의의 f \in L^{1} (\mathbb{R}) 에 대하여 lim_{\lambda \to \infty} \lVert f – h_{\lambda} * f \rVert_{1} = 0 이 성립한다.

임의의 유계 고른연속함수 f : \mathbb{R} \to \mathbb{C} 에 대하여 lim_{\lambda \to \infty} \lVert f – h_{\lambda} * f \rVert_{\infty} = 0 이 성립한다.

(명제) 함수 h : \mathbb{R} \to \mathbb{C} 가 다음 두 조건 h \ge 0 , \int_{\mathbb{R}} h = 1 을 만족할 때, h_{\lambda} (x) = \lambda h(\lambda x), x \in \mathbb{R}, \lambda > 0 이라 두면 {h_{\lambda} : \lambda > 0} 가 성질들 h_{\lambda} \ge 0, \int_{\mathbb{R}} h_{\lambda} = 1, lim_{\lambda \to \infty} \int_{\mathbb{R}\setminus[-\delta,\delta]} h_{\lambda} = 0 (0 < \delta ) 를 만족한다. 두 조건을 만족시키는 함수 h가 h(x) = \frac{1}{2\pi} \int_{\mathbb{R}} p(\alpha)u_{\alpha}(x) d\alpha 일 때 매우 유용하게 쓰인다.

(정의)  H(x) = \frac{1}{2\pi} \int_{\mathbb{R}} e^{-|\alpha|} e^{i \alpha x} d\alpha = \frac{1}{\pi} \frac{1}{1+x^{2}} 라 두면 위 명제의 조건을 충족하며, H_{\lambda} = \frac{1}{2\pi} \int_{\mathbb{R}} e^{-|\alpha/\lambda|} e^{i \alpha x} d\alpha = \frac{1}{2 \pi} \frac {2\lambda}{1+\lambda^{2} x^{2}} 이 되는데, {H_{\lambda} : \lambda > 0 } 을 뽀아송 핵이라 부른다.

(정의) 실수 \mathbb{R} 에서 정의된 함수 f \in C_{c}(\mathbb{R}) 가운데 n 번 미분가능하고 n계 도함수 f^(n) 이 연속인 함수들의 모임을 C_{c}^{n}(\mathbb{R}) 이라 쓰고, C_{c}^{\infty} (\mathbb{R}) = \bigcup_{n=1}^{\infty} C_{c}^{n}(\mathbb{R}) 이라 두면 이는 벡터공간이 된다.

(명제 5.2.5) 함수공간 C_{c}^{\infty} (\mathbb{R}) 는 노음공간 L^{1}(\mathbb{R}) 이나 C_{0} (\mathbb{R}) 에서 조밀한 부분공간이다.

(역변환공식) (정리 5.2.6) 만일 f \in L^{1}(\mathbb{R}) 이고 \hat{f} \in L^{1}(\mathbb{R}) 이면, 등식 f(x) = \frac{1}{2 \pi} \int_{\mathbb{R}} \hat{f}(\alpha) e^{i \alpha x} d\alpha 이 거의 모든 점 x 에서 성립한다.

f가 연속함수이면 등식은 모든 x \in \mathbb{R} 에 대하여 성립한다.

(정리 5.2.7) 만일 f \in L^{1}{\mathbb{R}} 이고 \hat{f} = 0 이면 거의 모든 점에서 f = 0 이다.

(정의) 각 \lambda > 0 에 대하여 K_{\lambda} (x) = \frac{1}{2 \pi} \int_{\mathbb{R}} \max{1- \frac{|\alpha|}{\lambda}, 0} u_{\alpha}(x) d\alpha = \frac{1}{2 \pi} \int_{\mathbb{R}} \biggl( 1- \frac{|\alpha|}{\lambda} \biggr) e^{i \alpha x} d\alpha 라 두면 함수모임 {K_{\lambda} : \lambda > 0} 을 페제르 핵이라 부른다.

(정의) G(x) = \frac{1}{2 \pi} \int_{\mathbb{R}} e^{-\alpha^{2}/2}u_{\alpha}(x) d\alpha 라 두자. 이로부터 얻어지는 함수모임 {G_{\lambda} : \lambda > 0} 을 가우스 핵이라 부른다.

(명제) g 와 \hat{g} 가 L^{1}-연속함수일 때 등식 g(x) = \frac{1}{2\pi} \hat{\hat{g}}(-x) , x \in \mathbb{R} 이 성립함을 말한다.

(명제) \hat{K_{\lambda}} (\alpha) =  \max{1- \frac{|\alpha|}{\lambda}, 0}, \hat{P_{\lambda}} (\alpha) = e^{-|\alpha/\lambda|}, \hat{G_{\lambda}} (\alpha) = e^{-\alpha^{2}/2\lambda^{2}} 

(정리 5.2.8) 푸리에 변환 f \mapsto \hat{f} 는 바나하공간 L^{1}(\mathbb{R}) 에서 C_{0} (\mathbb{R}) 로 가는 일대일 노음감소 중동형이고 그 치역이 조밀하다. 단 C_{0}(\mathbb{R})의 곱하기는 점별곱하기 (fg)(x) = f(x)g(x) 로 주어진다.

(정의) 르벡적분가능함수 f \in L^{1}(\mathbb{R}) 이 주어지면, 급수 F(t) = \sum_{n = -\infty}^{\infty} f(t-2n \pi) 가 거의 모든 점 t \in \mathbb{T} 에서 절대수렴하고 F \in L^{\mathbb{T}} 가 된다. F의 푸리에 급수가 t \in \mathbb{T} 에서 점별수렴한다면 등식 \sum_{n = -\infty}^{\infty} f(t – 2n\pi) = \frac{1}{2\pi} \sum_{n = -\infty}^{\infty} \hat{f}(n) e^{int} 를 얻는데, 이는 푸리에급수와 푸리에 적분의 관계를 보여주며 를 뽀아송 등식이라 한다.

