---



layout: post



title : 복소측도



date : 2018-01-20 08:53:04 +0900



---

(Section 7) 복소측도

(subsection 7.1) 부호측도와 복소측도

(정의) 만일 함수 \lambda : \mathfrak{S} \to \mathbb{R}^{*} 가 다음 성질을 만족하고 \mu(\empty) = 0 이면, 이를 부호가 붙은 측도라 한다.

{A_{n} \in \mathfrak{S} : n = 1,2, …} 가 서로소 \implies \lambda \biggl \bigsqcup_{n=1}^{\infty} A_{n} \biggr = \sum_{n = 1}^{\infty} \lambda (A_{n})

(정의) 만일 함수 \lambda : \mathfrak{S} \to \mathbb{C}가 다음 성질을 만족하고 \mu(\empty) = 0 이면, 이를 복소측도라 한다.

{A_{n} \in \mathfrak{S} : n = 1,2, …} 가 서로소 \implies \lambda \biggl \bigsqcup_{n=1}^{\infty} A_{n} \biggr = \sum_{n = 1}^{\infty} \lambda (A_{n})

(명제) 복소측도의 합과 스칼라곱은 다시 복소측도가 된다.

(정의) 복소측도 \lambda : \mathfrak{S} \to \mathbb{C} 가 주어졌을 떄, 각 E \in \mathfrak{S} 에 대하여 \lambda_{1} (E) 와 \lambda_{2} (E) 를 각각 \lambda (E) \in \mathbb{C}의 실수부분과 허수부분으로 정의하면, \lambda_{1} 와 \lambda_{2} 는 부호측도가 되고 \lambda = \lambda_{1} + i \lambda_{2} 이다.

(정의) 집합 X의 \sigma -대수 \mathfrak{S} 에 부호측도 \lambda 가 정의되어 있을 때, 집합 P \in \mathfrak{S} 가 성질 E \in \mathfrak{S} , E \subset P \implies \lambda (E) \ge 0 을 만족하면 이를 양집합이라 부르고, 성질 E \in \mathfrak{S} , E \subset P \implies \lambda (E) \le 0 을 만족하면 이를 음집합이라 정의한다.

(명제) 양집합의 부분집합은 항상 양집합이다. 만일 {P_{n} : n = 1,2, …} 이 양집합들의 모임이면 그 합집합 P 도 양집합이다.

(한 분해정리) (정리 7.1.1) 만일 \sigma -대수 (X,\mathfrak{S}) 에 부호측도 \lambda 가 주어지면 X 는 양집합과 음집합으로 분할된다. 만일 두 가지 분할 (P_{1}, Q_{1}) 과 (P_{2}, Q_{2}) 가 있으면, 임의의 E \in \mathfrak{S} 에 대하여 \lambda(E \cap P_{1}) = \lambda(E \cap P_{2}), \lambda(E \cap Q_{1}) = \lambda(E \cap Q_{2}) 가 성립한다.

(정의) 이제, 부호측도 \lambda 에 의하여 X 를 양집합 P 와 음집합 Q 로 분할하였을 때, 각 E \in \mathfrak{S} 에 대하여 \lambda_{+}(E) = \lambda(E \cap P), \lambda_{-}(E) = -\lambda(E \cap Q) 라 정의할 수 있다. 그러면 \lambda_{+}(E) 와 \lambda_{-}(E) 는 양측도가 되고 \lambda (E) = \lambda_{+}(E) - \lambda_{-}(E), E \in \mathfrak{S} 가 된다.

또한, 각 E \in \mathfrak{S} 에 대하여 | \lambda |(E) = \lambda_{+}(E) + \lambda_{-}(E)라 정의하면 | \lambda | 도 양측도이다.

(명제 7.1.2) 집합 X의 \sigma -대수 \mathfrak{S} 에서 정의된 부호측도 \lambda가 주어지면, 각 E \in \mathfrak{S} 에 대하여 | \lambda |(E) = \sup \biggl{ \sum_{n = 1}^{\infty} | \lambda (E_{n}) | : E_{n} \in \mathfrak{S} , E \bigsqcup_{n = 1}^{\infty} E_{n}\biggr} 이 성립한다.

(정의) \lambda 가 \sigma -대수 (X, \mathfrak{S}) 의 복소측도일 때 | \lambda |(E) = \sup \biggl{ \sum_{n = 1}^{\infty} | \lambda (E_{n}) | : E_{n} \in \mathfrak{S} , E \bigsqcup_{n = 1}^{\infty} E_{n}\biggr}

(정의) 집합 X의 \sigma -대수 \mathfrak{S} 에서 정의된 복소측도 \lambda 가 주어져 있을 때, E \mapsto |\lambda|(E) 는 양측도가 된다.

(정의) 복소측도 \lambda 를 \lambda = (\lambda_{1+} - \lambda_{1-}) + i ( \lambda_{2+} - \lambda_{2-} ) 와 같이 양측도의 선형결합으로 나타낼 수 있다. 임의의 E \in \mathfrak{S} 에 대하여 | \lambda | (E) < \infty 이며 특히 | \lambda | (X) < \infty 인데, \lVert \lambda \rVert = | \lambda | (X) 라 정의한다. 전체측도 \mu(X) 값이 유한인 양측도를 유한 양측도라 정의하는데, 유한 양측도는 복소측도이나 양측도는 복소측도가 아니다.

(subsection 7.2) 라돈-니코딤 정리와 르벡 분해정리

(정의) 집합 X 위의 \sigma -대수 \mathfrak{S} 위의 양측도 \mu 와 부호측도 혹은 복소측도 \lambda 가 성질 E \in \mathfrak(S), \mu(E) = 0 \implies \lambda(E) = 0 를 만족하면 \lambda 를 \mu 에 대한 절대연속측도라 하고 \lambda \ll \mu 라 쓴다. 

또한 성질 \lambda (E) = \lambda (A \cap E) , \mu (E) = \mu (B \cap E) , E \in \mathfrak{S} 를 만족하는 서로소인 A, B \in \mathfrak{S} 가 있으면 \lambda 를 \mu 에 대한 특이측도라 말하며, 이 때 \lambda \perp \mu 라 쓴다.

(명제) 실수축 위에서 \lambda = \lambda_{1} + i \lambda_{2} 와 같이 정의된 측도는 르벡측도에 대하여 절대연속이다. 디락측도는 르벡측도에 대한 특이측도이다.

(명제) 양측도 \mu 에 대하여 절대연속인 두 복소측도의 선형결합은 다시 절대연속이다. \mu 에 대한 특이측도의 선형결합도 다시 특이측도이다. 만일 복소측도가 양측도 \mu 에 대하여 동시에 절대연속이며 특이측도라 하면 \lambda = 0 이다.

(정의) \sigma-대수 (X, \mathfrak{S}) 에 고정된 양측도 \mu 가 주어져 있을 때, 임의의 복소측도를 절대연속측도와 특이측도의 합으로 표시할 수 있는데, 이를 르벡 분해라 부른다. 

(정의) 르벡분해의 절대연속부분은 함수로 표현되는데, 이 함수를 \mu 에 대한 \lambda 의 라돈-니코딤 도함수라 부른다.

(르벡-라돈-니코딤)(정리 7.2.1) 집합 X 의 \sigma -대수 \mathfrak{S} 위에서 정의된 \sigma -유한 양측도 \mu 와 복소측도 \lambda 에 대하여 성질 \lambda = \lambda_{a} + \lambda_{s} , \lambda_{a} \ll \mu , \lambda_{s} \perp \mu 를 가지는 측도 \lambda_{a} , \lambda_{s} 가 유일하게 존재한다. 또한 다음 등식 \lambda_{a} (E) = \int_{E} hd \mu , E \in \mathfrak{S} 이 성립하는 h \in L^{1}(X, \mu ) 가 유일하게 존재한다. 만일 \mu 와 \lambda 가 \sigma -유한 양측도이면 성질 \lambda = \lambda_{a} + \lambda_{s} 을 만족하는 측도 \lambda_{a} 와 \lambda_{s} , 그리고 등식 \lambda_{a} (E) = \int_{E} hd \mu , E \in \mathfrak{S}를 만족하는 잴 수 있는 함수 h : X \to [0,\infty] 가 유일하게 존재한다.

(정의) 두 측도 lambda_{a} 와 \mu 가 관계식 \lambda_{a} (E) = \int_{E} hd \mu , E \in \mathfrak{S} 를 만족할 때, 이를 d \lambda_{a} = h d \mu , h = \bigg[ \frac{d \lambda_{a}}{d \mu} \bigg] 로 쓴다.

(극형식분해) (정리 7.2.2) 집합 X에서 정의된 임의의 복소측도 \lambda 에 대하여 성질 d \lambda = hd| \lambda | , |h| = 1 을 만족하는 h \in L^{1}(X,| \lambda |) 가 유일하게 존재한다.

(정의) 복소함수 f \in L^{1}(X, |\lambda|) 의 복소측도 에 관한 적분은, 집합 X에 정의된 복소측도 \lambda 의 극형식 분해 d \lambda = hd| \lambda | 가 주어졌을 때, 등식 \int_{X} \lambda d \mu = (\int_{X} \lambda_{1+} d \mu - \int_{X} \lambda_{1-}) d \mu + i ( \int_{X} \lambda_{2+}  d \mu - \int_{X} \lambda_{2-} d \mu ) 로 주어진다.

(정리 7.2.3) 집합 X 의 \sigma -대수에서 정의된 \sigma -유한 양측도 \mu 에 대하여 L^{p}( \mu )^{*} = L^{q}( \mu ) 이다. (단, p, q 는 켤레지수이고, 1 \le p < \infty )

(따름정리 7.2.4) 집합 X 에 \sigma -유한 양측도 \mu 가 주어져 있고, 1 \le p \le \infty 라 하자. 만일 X에서 정의된 잴 수 있는 함수 g 가 성질 h \in L^{q}( \mu ) \implies \bigg| \int_{X} ghd \mu \bigg| \le M \| h \|_{q} (단, p, q 는 켤레지수) 을 만족하면 g \in L^{p}( \mu ) 이고 \| g \|_{p} \le M 을 만족한다.

(subsection 7.3) 실직선의 보렐측도

(정의) 보렐집합 위에서 정의된 복소측도를 보렐측도라 한다. 유계구간의 측도값이 항상 유한인 양측도인 보렐측도를 정규 양보렐측도라 부른다.

(정의) 실직선의 정규 양보렐측도 \lambda 에 대하여, 함수 \alpha_{\lambda} : \mathbb{R} \to \mathbb{R} 을 다음과 같이 정의한다. \alpha_{\lambda} 는 단조증가이고 오른쪽연속함수이다.

\alpha_{\lambda} = \begin{cases} \lambda (( 0, x \rbrack ), & x >0 \\ 0, & x = 0 \\ - \lambda (( x, 0 \rbrack ),  & x < 0 \end {cases}

(정의) 구간 [a,b] 위에서 정의된 유계실함수 f : [a,b] \to \mathbb{R} 에 대하여 리만-스틸체스 적분 \int_{a}^{b} fd \alpha_{\lambda} 를 생각한다. 이는 리만적분과 비슷한 과정을 거쳐 정의된다.

(명제) 함수 f : \mathbb{R} \to \mathbb{R} 이 연속이고 그 받침이 유계구간 (A,B) 에 들어간다면, 등식 \int_{\mathbb{R}} f d \lambda = \int_{A}^{B} f(x) d \alpha_{\lambda} (x) 이다. 따라서 함수공간 C_{c}(\mathbb{R}) 에서 정규 양보렐측도에관한 적분은 리만-스틸체스 적분과 같다.

(정의) 한 점의 측도값이 항상 0 인 측도를 연속측도라 부른다.

(명제 7.3.1) 실직선에서 정의된 정규 양보렐측도 \lambda 에 대하여, 함수 \alpha_{\lambda} 가 점 x 에서 연속일 필요충분조건은 \lambda({x}) = 0 이다.

(정리 7.3.2) 실직선에 정의된 정규 양보렐측도 \lambda 에 대하여 다음은 동치이다.

\lambda \ll m 이다.

\alpha_{\lambda} 가 임의의 유계닫힌구간 위에서 절대연속이다.

(정리 7.3.3) 실직선 위에서 정의된 정규 양보렐측도 \lambda 는 임의의 보렐집합 E \in \mathfrak{B} 에 대하여 다음 등식들을 만족한다.

\lambda(E) = \inf{\lambda(U) : U \supset E, U 는 열린집합이다.}

\lambda(E) = \sup{\lambda(K) : K \subset E, K 는 유계닫힌집합이다.}

(따름정리 7.3.4) 만일 \lambda \ll m 이고 거의 모든 점에서 \alpha_{\lambda} ‘ = 0 이면 \lambda = 0 이다.

(정리 7.3.5) 실직선에 정의된 정규 양보렐측도 \lambda 에 대하여 다음은 동치이다.

\lambda \perp m 이다.

거의 모든 점에서 \alpha_{\lambda} ‘ = 0 이다.

(따름정리 7.3.6) 실직선 위의 정규 양보렐측도 \lambda 가 르벡측도 m 에 대하여 절대연속이면 거의 모든 점에서 [\frac{d \lambda }{d m}] = \alpha_{\lambda}’ 이 성립한다.

(명제) 거의 모든 점에서 도함수가 0 이지만 상수함수가 아닌 연속함수가 존재하며 칸토르 함수가 대표적이다.

(명제) 실직선 위에 정의된 정규 양보렐측도 \lambda 는 절대연속측도 \lamba_{a}, 연속특이측도 \lambda_{s}, 디락측도의 합으로 표현되는 측도 \lambda_{d} 의 합으로 쓸 수 있다. 이들 측도엣 얻어지는 단조증가함수를 각각 \alpha_{a} , \alpha_{s}, \alpha_{d} 라 두면 \alpha_{a} 는 절대연속함수, \alpha_{s} 는 그 도함수가 거의 모든 점에서 0인 연속함수, \alpha_{d} 는 불연속함수이다. \lambda 에 의하여 얻어지는 단조증가함수를 \alpha 라 두면 \alpha = \alpha_{a} + \alpha_{s} + \alpha_{d} 이고 등식 \lambda_{a} (E) = \int_{E} \alpha_{a} ‘ dm = \int_{E} \alpha ‘ dm , E \in \mathfrak{B} 이 성립한다.

