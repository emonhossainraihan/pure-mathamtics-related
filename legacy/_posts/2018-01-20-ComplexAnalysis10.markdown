---



layout: post



title : (Complex Analysis) Applications of Theta functions



date : 2018-01-20 09:52:04 +0900



---

(section 10) Applications of Theta functions

(subsection 1) Product formula for the Jacobi theta function

(Def) Jacobi’s theta function is defined for z \in \mathbb{C} and \tau \in \mathbb{H} by \Theta (z|\tau) = \sum_{n = - \infty}^{\infty} = \sum_{n = - \infty}^{\infty} e^{\pi i n^{2} \tau} e^{2 \pi i n z}.

Two significant special cases are \theta(\tau) and \vartheta(t), which are defined by \theta(\tau) = \sum_{n = -\infty}^{\infty} e^{\pi i n^{2} \tau} , \tau \in \mathbb{H}, \vartheta(t) = \sum_{n = -\infty}^{\infty} e^{-\pi n^{2} t}, t>0.

For example, heat kernel was given by H_{t}(x) = \sum_{n = - \infty}^{\infty} = \sum_{n = - \infty}^{\infty} e^{-4\pi^{2} n^{2} t} e^{2 \pi i n x}, and therefore H_{t}(x) = \Theta(x|4\pi i t).

(Prop 1.1.) The function \Theta satisfies the following properties :

\Theta is entire in z \in \mathbb{C} and holomorphic in \tau \in \mathbb{H}.

\Theta(z+1|\tau) = \Theta(z | \tau).

\Theta(z + \tau | \tau) = \Theta(z|\tau) e^{-\pi i \tau} e^{-2\pi i z}

\Theta(z|\tau) = 0 whenever z = 1/2 + \tau/2 + n + m\tau and n,m \in \mathbb{Z}.

(Def) A product \prod(z|\tau) that enjoys the same structural properties as \Theta(z|\tau) as a function of z. This product is defined for z \in \mathbb{C} and \tau \in \mathbb{H} by \prod(z|\tau) = \prod_{n=1}^{\infty} (1-q^{2n}) (1+ q^{2n-1}e^{2\pi i z}) (1+ q^{2n-1}e^{-2\pi i z}) , where we have used the notation that is standard in the subject, namely q = e^{\pi i \tau}. The function \prod(z|\tau) is sometimes referred to as the triple-product.

(Prop 1.2.) The function \prod(z|\tau) satisfies the following properties :

\prod(z,\tau) is entire in z \in \mathbb{C} and holomorphic for \tau \in \mathbb{H}.

\prod(z+1|\tau) = \prod(z | \tau).

\prod(z + \tau|\tau) = \prod(z|\tau) e^{-\pi i \tau} e^{-2\pi i z}.

\prod(z|\tau) = 0 whenever z = 1/2 + \tau/2 + n + m\tau and n , m \in \mathbb{Z}. Moreover, these points are simple zeros of \prod(\cdot | \tau) , and \prod(\cdot | \tau) has no other zeros.

(Product formula) (Thm 1.3.) For all z \in \mathbb{C} and \tau \in \mathbb{H} we have the identity \Theta(z|\tau) = \prod(z | \tau).

(Cor 1.4.) If Im(\tau)>0 and q = e^{\pi i \tau}, then \theta(\tau) = \prod_{n=1}^{\infty} (1-q^{2n}) (1+ q^{2n-1})^{2}. Thus \theta(\tau) \neq 0 for \tau \in \mathbb{H}.

(Cor 1.5.) For each fixed \tau \in \mathbb{H}, the quotient (log \Theta(z|\tau))” = \frac{\Theta(z|\tau) \Theta”(z|\tau) – (\Theta’(z|\tau))^{2}}{\Theta(z|\tau)^{2}} is an elliptic function of order 2 with periods 1 and \tau, and with a double pole at z = 1/2 + \tau/2.

In the above, the primes ‘ denote differentiation with respect to the z variable.

(subsubsection 1.1.) Further transformation laws

(Thm 1.6.) If \tau \in \mathbb{H}, then \Theta(z|-1/\tau) = \sqrt{\frac{\tau}{i}} e^{\pi i \tau z^{2}} \Theta(z\tau | \tau) for all z \in \mathbb{C}. Here \sqrt{\frac{\tau}{i}} denotes the branch of the square root defined on the upper half-plane, that is positive when \tau = it, t >0.

(Cor 1.7.) If Im(\tau) >0, then \theta(-1/\tau) = \sqrt{\frac{\tau}{i}}\theta(\tau).

(Cor 1.8.) If \tau \in \mathbb{H}, then \theta(1-1/\tau) = \sqrt{\frac{\tau}{i}} \sum_{n=-\infty}^{\infty} e^{\pi i (n+1/2)^{2} \tau} = \sqrt{\frac{\tau}{i}}( 2 e^{\pi i \tau/4} + \cdots). The second identity means that \theta(1-1/\tau) \sim \sqrt{\frac{\tau}{i}} 2e^{i\pi \tau/4} as Im(\tau) \to \infty.

(Def) Dedekind eta function, which is defined for Im(\tau) >0 by \eta(\tau) = e^{\frac{\pi i \tau}{12}} \prod_{n=1}^{\infty} (1- e^{2\pi i n \tau}).

(prop 1.9.) If Im(\tau) >0, then \eta(-1/\tau) = \sqrt{\tau/i} \eta(\tau).

(subsection 2) Generating functions

(Def) Given a sequence {F_{n}}_{n=0}^{\infty}, its generating function F(x) = \sum_{n=0}^{\infty} F_{n}x^{n}. 

(Def) The partition function is defined as follows : if n is a positive integer, we let p(n) denote the numbers of ways n can be written as a sum of positive integers. For instance, p(1) = 1, and p(2) = 2 since 2 = 2+0 = 1+1. We set p(0) = 1.

(Thm 2.1.) If |x| < 1, then \sum_{n=1}^{\infty} p(n) x^{n} = \prod_{k=1}^{\infty} \frac{1}{1-x^{k}}.

(Def) Let p_{e,u}(n) denote the number of partitions of n into an even number of unequal parts, and p_{0,u} (n ) the number of partitions of n into an odd number of unequal parts. Then , Euler proved that, unless n is a pentagonal number, one has p_{e,u}(n) = p_{o,u}(n) . By definition, pentagonal numbers are integers n of the form k(3k+1)/2, with k \in \mathbb{Z}.

(Prop 2.2.) \prod_{n=1}^{\infty}(1-x^{n}) = \sum_{k=-\infty}^{\infty} (-1)^{k}x^{\frac{k(3k+1)}{2}}

(subsection 3) The theorems about sum of squares

(subsubseciton 3.1.) The two-squares theorem

(Def) divisor functions : d_{1}(n) denote the number of divisors of n of the form 4k +1, and d_{3} (n) the number of divisors of n of the form 4k +3. 

define r_{2}(n) to be the number of ways n can be written as the sum of two squares, counting obvious repetitions; that is, r_{2}(n) is the number of pairs (x,y) x, y \in \mathbb{Z}, so that n = x^{2} + y^{2} .

Define r_{4}(n) to be the number of ways of expressing n as a sum of four squares.

(Thm 3.1.) If n \ge 1, then r_{2}(n) = 4(d_{1}(n) – d_{3}(n)).

If n = p_{1}^{\alpha_{1}}\cdots p_{r}^{\alpha_{r}} is the prime factorization of n where p_{1},…,p_{r} are distinct, then : The positive integer n can be represented as the sum of two squares iff every prime p_{j} of the form 4k + 3 that occurs in the factorization of n has an even exponent a_{j}.

(Prop 3.2.) The identity r_{2}(n) = 4(d_{1}(n) – d_{3}(n)) , n \ge 1, is equivalent to the identities \theta(\tau)^{2} = 2 \sum_{n=-\infty}^{\infty}\frac{1}{q^{n} + q^{-n}} = 1 + 4 \sum_{n=1}^{\infty} \frac{q^{n}}{1+q^{2n}}. whenever q = e^{\pi i \tau} and \tau \in \mathbb{H}.

(Prop 3.3.) The function \mathcal{C}(\tau) = \sum 1/cos(\pi n \tau) , defined in the upper half-plane, satisfies 

\mathcal{C}(\tau +2) = \mathcal{C}(\tau).

\mathcal{C}(\tau) = (i/\tau)\mathcal{C}(-1/\tau).

\mathcal{C}(\tau) \to 1 as Im(\tau) \to \infty.

\mathcal{C}(1-1/\tau) \sim 4(\tau/i) e^{\pi i \tau/2} as Im(\tau) \to \infty.

Moreover, \theta(\tau)^{2} satisfies the same properties.

(Thm 3.4.) Suppose f is a holomorphic function in the upper half-plane that satisfies:

f(\tau +2) = f(\tau),

f(-1/\tau) = f(\tau),

f(\tau) is bounded,

then f is constant.

(Def) A subset of the closed upper half-plane, which is defined by \mathcal{F} = {\tau \in \bar{\mathbb{H}} : |Re(\tau)|\le 1 and |\tau| \ge 1}. The points corresponding to \tau = \mp 1 are called cusps.

(Lem 3.5.) Every point in the upper half-plane can be mapped into \mathcal{F} using repeatedly one or another of the following fractional linear transformations or their inverses: T_{2} : \tau \mapsto \tau +2, S : \tau \mapsto -1/\tau.

For this reason, \mathcal{F} is called the fundamental domain for the group of transformations generated by T_{2} and S.

(Def) We let G denote the group generated by T_{2} and S. Since T_{2} and S are fractional linear transformations, we may represent an element g \in G by a matrix g = \begin{pmatrix} a & b \\ c & d \end{pmatrix} with the understanding that g(\tau) = \frac{a\tau + b}{c\tau + d}. Since the matrices representing T_{2} and S have integer coefficients and determinant 1, the same is true for all matrices of elements in G. In particular, if \tau \in \mathbb{H}, then Im(g(\tau)) = \frac{Im(\tau)}{|c\tau + d|^{2}}.

(subsection 3.2.) The four-squares theorem

(Def) \sigma_{1}^{*}(n) equals the sum of divisors of n that are not divisible by 4.

(Thm 3.6.) Every positive integer is the sum of four squares, and moreover r_{4}(n) = 8 \sigma_{1}^{*}(n) for all n \ge 1.

(Prop 3.7.) The assertion r_{4}(n) = 8\signa_{1}^{*} (n) is equivalent to the identity \theta(\tau)^{4} = \frac{-1}{\pi^{2}} E_{2}^{*}(\tau), where \tau \in \mathbb{H}.

(Prop 3.8.) The function E_{2}^{*}(\tau) defined in the upper half-plane has the following properties :

E_{2}^{*}(\tau + 2) = E_{2}^{*}(\tau).

E_{2}^{*}(\tau) = -\tau^{-2} E_{2}^{*{}(-1/\tau).

E_{2}^{*}(\tau) \to -\pi^{2} as Im(\tau) \to \infty.

|E_{2}^{*} (1-1/\tau)| = O(|\tau^{2} e^{\pi i \tau}|) as Im(\tau) \to \infty.

moreover -\pi^{2}\theta^{4} has the same properties.

(Def) The forbidden Eisenstein series F and its reverse \tilde{F}, which is obtained from reversing the order of summation : F(\tau) = \sum_{m} \sum_{n} \frac{1}{(m\tau + n)^{2}} and \tilde{F} (\tau) = \sum_{n} \sum_{m} \frac{1}{(m\tau + n)^{2}}. In both cases, the term n = m = 0 is omitted.

(Lem 3.9.) The functions F and \tilde{F} satisfy :

F(-1/\tau) = \tau^{2} \tilde{F}(\tau),

F(\tau) - \tilde{F}(\tau) = 2\pi i/\tau.

F(-1/\tau) = \tau^{2}F(\tau) – 2\pi i \tau.

