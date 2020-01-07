---



layout: post



title : (Real Analysis 실해석) 위상과 측도



date : 2018-01-20 08:53:14 +0900



---

(section 8) 위상과 측도

(subsection 8.1) 국소옹골공간

(정의) 집합 X의 부분집합 모임 \mathfrak{T} 가 다음 성질들

\empty , X \in \mathfrak{T}

\mathfrak{T} 는 임의의 합집합에 대하여 닫혀있다.

\mathfrak{T}는 유한교집합에 대하여 닫혀있다.

을 만족할 때 이 \mathfrak{T} 를 X 의 위상이라 하고, 위상이 주어진 집합을 위상공간이라 한다. \mathfrak{T} 에 들어가는 집합을 열린집합이라 하며, 그 여집합이 \mathfrak{T} 에 들어가는 집합을 닫힌집합이라 부른다. 임의의 집합 S \subset X 에 대하여 S를 포함하는 모든 닫힌 부분집합들의 교집합을 \bar{S} 라 쓰고 이를 S의 닫힘이라 한다. S 안에 들어가는 열린집합 전체의 합집합을 S의 내부라 하고 이를 int S 라 쓴다.

(정의) 모든 부분집합을 다 모으면 위상이 되는데, 이러한 위상이 주어진 위상공간을 이산공간이라 한다. 위상공간 (X, \mathfrak{T}) 와 X의 부분집합 Y \subset X 가 있을 때 \mathfrak{T} |_{Y} = {A \cap Y : A \in \mathfrak{T} } 는 Y 의 위상이 되는데, (Y , \mathfrak{T} |_{Y}) 를 (X, \mathfrak{T}) 의 부분공간이라 한다.

(정의) 위상공간 X, Y 사이에 정의된 함수 f : X \to Y 가 있을 떄, 임의의 열린 집합 V \subset Y 에 대하여 그 역상 f^{-1} (V) 가 X의 열린 집합이면 f 를 연속함수라 한다. 두 위상공간 X< Y 사이에 전단사함수 f 가 존재하며 f 와 f^{-1} 모두 연속 이면 X와 Y가 서로 위상동형이라 한다.

(정의) 위상공간 (X, \mathfrak{T}) 의 모든 열리집합이 집합모임 \mathfrak{B} \subset \mathfrak{T} 에 있는 집합들의 합집합으로 표시되면 \mathfrak{B} 를 이 공간의 위상기저 또는 기저라 한다.

(정의) 집합모임 {X_{\alpha} : \alpha \in A }의 곱집합을 \prod_{\alpha \in A} X_{\alpha} = {\xi : A \to \bigcup_{\alpha \in A} X_{\alpha} : \xi (\alpha ) \in X_{\alpha} (\alpha \in A)} 라 정의한다. 각 \alpha \in A 에 대하여 \pi_{\alpha} (\xi ) = \xi ( \alpha ) , \xi \in \prod_{\alpha \in A} X_{\alpha} 와 같이 정의된 함수 \pi_{\alpha} : \prod_{\alpha} X_{\alpha} \to X_{\alpha} 를 정사영이라 한다. 위상공간 모임 {(X_{\alpha}, \mathfrak{T}_{\alpha}): \alpha \in A} 에 대하여, …(p215)

(subsection 8.2) 리쓰 표현정리

(정의) 위상공간 X의 열린집합으로 포함하는 최소의 \sigma -대수 \mathfrak{B} 에 들어가는 집합을 보렐집합이라 하고, (X, \mathfrak{B}) 에 정의된 측도를 보렐측도라 한다. 보렐측도에 관하여 잴 수 있는 함수를 보렐함수라 한다. 

(정의) 만일 국소옹골공간 X 에 주어진 양보렐측도 \mu 가 성질 K 가 옹골집합 \implies \mu (K) < \infty 를 만족하면 임의의 f \in C_{c}(X) 에 대하여 \int_{X} f d \mu \in \mathbb{C} 이고, \Lambda _{\mu} : f \mapsto \int_{X} fd \mu : C_{c} (X) \to \mathbb{C} 는 C_{c} (X) , f \ge 0 \implies \Lambda_{\mu} (f) \ge 0 이 성립하는데, 이러한 C_{c} (X) 의 선형범함수를 양선형범함수라 부른다.

만일 \Lambda 가 C_{c}(X) 의 양선형범함수이면, g, h \in C_{c}(X) 가 실함수일 때 g \le h \implies \Lambda (g) \le \Lambda (h) 이다.

(정의) X가 국소옹골공간이라 가정하고, C_{c} (X) 의 양선형범함수 \Lambda : C_{c} (X) \to \mathbb{C} 가 주어져 있다고 하자. 임의의 열린집합 V \subset X 에 대하여 \mu (V) = \sup{\lambda (f) : f \prec V} 라 정의하고, 임의의 E \subset X 에 대하여 \mu (E) = \inf {\mu(V) : V \supset E , V 는 열린집합} 이라 정의한다. 이로써 집합 X에 정의된 외측도 \mu : \mathcal{P} (X) \to [0, \infty ] 를 얻었다. 양측도 (X, \mathfrak{S}, \mu) 를 얻을 수 있다. \mathfrak{B} \subset \mathfrak{S} 임을 알 수 있고 \mu 를 \mathfrak{B} 에 제한하면 보렐측도를 얻는다.

(도움정리 8.2.1) 지금까지 만든 보렐측도 \mu 는 다음 성질을 가진다.

K가 옹골집합이면 \mu (K) < \infty 이고, 다음 등식 \mu (K) = \inf {\lambda (f) : K \prec f} 이성립한다.

임의의 열린집합 E가 다음 등식 \mu (E) = \sup {\mu(K) : K \supset E , K 는 옹골집합} 을 만족한다.

(리쓰 표현정리)(정리 8.2.2) 국소옹골 하우스도르프 공간 X가 주어져 있을 때, 벡터공간 C_{c} (X) 에서 정의된 임의의 양선형범함수 \Lambda 에 대하여 다음 성질들

임의의 f \in C_{c} (X) 에 대하여 \Lambda (f) = \int_{X} fd \mu 이다.

임의의 보렐집합 E에 대하여 \mu (E) = \inf {\mu(V) : V \supset E , V 는 열린집합} 이 성립한다.

임의의 열린집합 E에 대하여 \mu (E) = \sup {\mu(K) : K \supset E , K 는 옹골집합} 이 성립한다.

를 만족하는 보렐측도 \mu 가 유일하게 존재한다. 이 때, 측도 \mu는 조건 K 가 옹골집합 \implies \mu (K) < \infty 를 만족한다. 또한, \mu(E) < \infty 인 임의의 보렐집합 E에 대하여 \mu (E) = \sup {\mu(K) : K \supset E , K 는 옹골집합} 이 성립한다.

(정의) 국소옹골공간에 정의된 양보렐측도가 조건 K 가 옹골집합 \implies \mu (K) < \infty 를 만족하고 임의의 보렐집합에 대하여 \mu (E) = \inf {\mu(V) : V \supset E , V 는 열린집합} 와 \mu (E) = \sup {\mu(K) : K \supset E , K 는 옹골집합}이 성립하면 이를 정규보렐측도라 한다.

(명제) 리쓰 표현정리에 의하여 주어진 측도가 \sigma -유한측도라면 이는 정규측도이다. 셀 수 있는 옹골부분집합의 합집합으로 표시되는 공간을 \sigma -옹골공간이라 하는데, 이 경우 리쓰 표현정리에 의해 얻어지는 측도가 정규측도가 된다.

(명제) 실직선의 정규 양보렐측도 \mu 에 대하여 단조증가하는 오른쪽연속함수 \alpha_{\mu} 를 정의하여 대응관계 \mu \mapsto \alpha_{\mu} 를 얻었고, 이 단조함수에 의하여 정의되는 C_{c} (\mathbb{R}) 의 리만-스틸체스 적분이 앞에서 \Lambda _{\mu} : f \mapsto \int_{X} fd \mu : C_{c} (X) \to \mathbb{C} 로 정의된 양선형사상 \Lambda_{ \mu } 임을 알았다. 이 대응관계는 일대일 대응이다.

(명제) 만일 f \in C_{c} (\mathbb{R}^{2} ) 의 받침이 R = [a,b] \times [c,d] 에 들어가면 f 는 R 위에 연속함수이므로 이중적분 \int \int_{R} f 을 생각할 수 있는데, 이는 푸비니 정리에 의해 르벡적분 \int_{\mathbb{R}^{2}} f dm_{2} 와 같은 값이다. 따라서 양선형범함수 f \mapsto \int \int_{R} f : C_{c}( \mathbb{R}^{2} ) \to \mathbb{C} 에 의하여 얻어진 보렐측도는 르벡측도 m_{2} 를 보렐집합에 제한한것이다.

(section 8.3) 연속함수와 보렐측도

(정의) 리쓰 표현정리에 의해 얻어진 국소옹골공간의 양측도를 준정규 양보렐측도라 부른다.

X 의 준정규 양보렐측도와 C_{c} (X) 의 양선형범함수는 일대일대응 관계를 가진다.

(루진) (정리 8.3.1) 국소옹골공간 X에 준정규 양보렐측도 \mu 와 잴 수 있는 함수 f : X \to \mathbb{C} 가 주어져 있고, f 는 유한측도집합 A 바깥에서 0 이라 가정하자. 이 때, 임의의 양수 \epsilon > 0 에 대하여 \mu({x \in X : f (x) \neq g (x) }) < \epsilon 을 만족하는 연속함수 g \in C_{c} (X) 가 존재한다. 만일 f \in L^{\infty} (X, \mu) 이면 \| g \|_{\infty} \le \| f \|_{\infty} 가 되도록 g \in C_{c} (X) 를 택할 수 있다.

(정리 8.3.2) 국소옹골공간 X에 준정규 양보렐측도 \mu 가 주어져 있을 때, C_{c} (X) 는 L^{p} (X, \mu) 의 조밀한 부분공간이다 (단, 1 \le p < \infty)

(정의) 국소옹골공간 X에서 정의된 복소 정규보렐측도 전체의 벡터공간을 M(X) 라 쓰면 이는 \lambda \mapsto \| \lambda \| 에 관하여 노음공간이 된다.

(도움정리 8.3.3) 실노음공간 C_{0}^{\mathbb{R}} (X) 에서 정의된 유계 실선형범함수 \phi 에 대하여 \phi = \phi_{+} - \phi_{-} , \| \phi \| = \| \phi_{+} \| + \| \phi_{-} \| 인 양선형범함수  \phi_{+}, \phi_{-} 가 존재한다.

(정리 8.3.4) 국소옹골공간 X에 대하여 C_{0} (X)^{*} = M(X) 이다.

(명제 8.3.5) 국소옹골공간 X의 실함수공간 C_{c}^{\mathbb{R}} (X) 의 실부분공간 A 가 스톤-바이에르쉬티라스 정리의 첫번째와 두번째 가정을 만족한다고 가정하자. 또한, 임의의 옹골집합 K 에 대하여 K \prec h 인 h \in A 가 존재한다고 가정하자. 그러면 A는 노음공간 (C_{c}^{\mathbb{R}} (X), \| \|_{\sup}) 안에서 조밀하다.

(정의 8.18) X에서 정의된 보렐함수 f와 Y에서 정의된 보렐함수 g가 주어지면 X \times Y 에서 정의된 함수 (x,y) \mapsto f(x), (x,y) \mapsto g(x) 는 각각 \mathfrak{B}_{X} \times \mathfrak{B}_{Y} 에서 잴 수 있는 함수이고, 따라서 함수 (x,y) \mapsto f(x)g(y) , (x,y) \in X \times Y 는 \mathfrak{B}_{X} \times \mathfrak{B}_{Y} 에 관하여 잴 수 있는 함수이다.  만일 f \in C_{c} (X) 이고 g \in C_{c} (Y) 이면 위 처럼 정의된 함수는 C_{c} (X,Y) 에 들어가는데, 이런 형태의 함수들에 의해 생성된 C_{c} (X \times Y) 의 부분공간을 \mathcal{A} 라 두자. 

(정의) 만일 \mu, \nu 가 각각 X, Y 의 \sigma -유한 준정규 양보렐측도라면, 임의의 F \in C_{c}(X \times Y) 는 L^{1} (\mu \times \nu) 에 들어간다. 따라서 C_{c} (X \times Y)의 양선형범함수 F \mapsto \int_{ X \times Y} F d( \mu \times \nu ) , F \in C_{c} (X \times Y ) 를 생각할 수 있다. 이 선형범함수에 대응하는 준정규 양보렐측도는 \sigma – 대수 \mathfrak{B}_{X} \times \mathfrak{B}_{Y} 위에서 곱측도 \mu \times \nu 와 그 측도값이 일치하고, X \times Y 에서 정의된 보렐함수에 대하여 토넬리-푸비니 정리가 성립한다.

(정의) (정의 8.18) 처럼 정의된 함수를 f \otimes g 라 표시하자. 만일 \mu 와 \nu 가 각각 국소옹골공간 X와 Y의 복소 정규보렐측도이면, F \mapsto \int_{X \times Y} F \cdot (h \otimes k) d(| \mu | \times | \nu |), F \in C_{0} (X \times Y) 는 C_{0} (X \times Y)의 유계선형범함수가 되고, 이에 대응하는 복소정규보렐측도를 \mu \times \nu 라 쓴다. 

\| \mu \times \nu \| \le \| \mu \| \| \nu \| 

(명제) 만일 F \in C_{0} (X \times Y) 이면 임의의 x \in X 에 대하여, F_{x} \in C_{0} (Y) 이고, 함수 x \mapsto \int_{Y} F_{x} d \nu : X \to \mathbb{C} 가 C_{0} (X) 에 들어간다.

(명제) 임의의 복소정규보렐측도 \mu \in M(X) 와 \nu \in M(Y) 에 대하여 푸비니 정리 \int_{X \times Y} F d ( \mu \times \nu ) \int_{X} \int_{Y} F(x,y) d \nu (y) d \mu (x) , F \in C_{0} (X \times Y) 가 성립한다.

