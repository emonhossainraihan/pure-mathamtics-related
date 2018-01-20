---



layout: post



title :  (Complex Analysis) The Fourier Transform



date : 2018-01-20 09:52:04 +0900



---

(Section 4) The Fourier Transform

(Def) If f is a function on \mathbb{R} that satisfies appropriate regularity and decay conditions, then its Fourier transform is defined by \hat(\xi) = \int_{-\infty}^{\infty} f(x) e^{-2\pi ix \xi} dx , \xi \in \mathbb{R}, and its counterpart, the Fourier inversion formula, holds f(x) = = \int_{-\infty}^{\infty} \hat{f}(\xi) e^{2\pi ix \xi} d\xi

(Def) The condition, given by the Paley-Wiener theorem, is that there be a holomorphic extension of f to \mathbb{C} that satisfies the growth condition |f(z)| \le Ae^{2\piM|z|} for some constant A>0. Functions satisfying this condition are said to be of exponential type.

(Def) A function f is of moderate decrease if f is continuous and there exists A >0 so that |f(x)| \le A/(1+x^{2}) for all x \in \mathbb{R} . A more restrictive condition is that f \in S, the Schwarz space of testing functions, which also implies that \hat{F} belongs to S.

(subsection 1) The class \mathfrak{F}

(Def) For each a >0 we denote by \mathfrak{F}_{a} the class of all functions f that satisfy the following two conditions :

The function f is holomorphic in the horizontal strip S_{a} = {z \in \mathbb{C} : |Im(z)| <a } . 

There exists a constant A >0 s.t. |f(x+iy)| \le \frac{A}{1+x^{2}} for all x \in \mathbb{R} and |y|<a.

(Def) Denote by \mathfrak{F} the class of all functions that belong to \mathfrak{F}_{a} for some a.

(subsection 2) Action of the Fourier transform on \mathfrak{F}

(Thm 2.1.) If f belongs to the class \mathfrak{F}_{a} for some a > 0 , then |\hat{f}(\xi)| \le Be^{-2\pib |\xi|} for any 0 \le b < a.

(Thm 2.2.) If f \in \mathfrak{F}, then the Fourier inversion holds, namely f(x) = \int_{-\infty}^{\infty} \hat{f}(\xi) e^{2\pi ix \xi}d \xi for all x \in \mathbb{R}.

(Lem 2.3.) If A is positive and B is real, then \int_{0}^{\infty} e^{-(A+iB)\xi} d\xi = \frac{1}{A+iB}.

(Thm 2.4.) If f \in \mathfrak{F}, then \sum_{n \in \mathbb{Z}}f(n) = \sum_{n \in \mathbb{Z}} \hat{f}(n).

(subsection 3) Paley-Wiener theorem

(Thm 3.1.) Suppose \hat{f} satisfies the decay condition |\hat{f}(\xi)} \le Ae^{-2\pi a |\xi|} for some constants a, A >0. Then f(x) is the restriction to \mathbb{R} of a function f(z) holomorphic in the strip S_{b} = {z \in \mathbb{C} : |Im(z)|<b}, for any 0 < b < a.

(Cor 3.2.) If \hat{f} (\xi) = O(e^{-2\pi a |\xi|} ) for some a >0 , and f vanishes in a non-empty open interval, then f = 0.

(Thm 3.3.) Suppose f is continuous and of moderate decrease on \mathbb{R}. Then f has an extension to the complex plane that is entire with |f(z)| \le Ae^{2\piM|z|} for some A>0, iff \hat{f} is supported in the interval [-M,M].

(Thm 3.4.) Suppose F is a holomorphic function in the sector S = {z : -\pi/4 < arg z < \pi/4 } that is continuous on the closure of S. Assume |F(z)| \le 1 on the boundary of the sector, and that there are constants C, c>0 s.t. |F(z)| \le Ce^{c|z|} for all z in the sector. Then |F(z)| \le 1 for all z \in S.

(Thm 3.5.) Suppose f and \hat{f} have moderate decrease. Then \hat{f} (\xi) = 0 for all \xi < 0 iff f can be extended to a continuous and bounded function in the closed upper half-plane {z = x + iy : y \ge 0} with f holomorphic in the interior.

(section 5) Entire Functions

(subsection 1) Jensen’s formula

(Thm 1.1.) Let \Omega be an open set that contains the closure of a disc D_{R} and suppose that f is holomorphic in \Omega, f(0) \neq 0, and f vanishes nowhere on the circle C_{R}. If z_{1},…,z_{N} denote the zeros of f inside the disc(counted with multiplicities). then log |f(0)| = \sum_{k = 1}^{N} log(\frac{|z_{k}|}{R}) + \frac{1}{2\pi} \int_{0}^{2\pi} log |f(Re^{i\theta})| d\theta.

(Lem 1.2.) If z_{1},…,z_{N} are the zeros of f inside the disc D_{R}, then \int_{0}^{R} n(r) \frac{dr}{r} = \sum_{k=1}^{N} log |\frac{R}{z_{k}}|.

(subsection 2) Functions of finite order

(Def) Let f be an entire function. If there exists a positive number \rho and constants A,B >0 s.t. |f(z)| \le Ae^{B|z|^{\rho}} for all z \in \mathbb{C}, then we say that f has an order of growth \le \rho. We deine the order of growth of f as \pho_{f} = \inf \tho, where the infimum is over all \pho >0 s.t. f has an order of growth \le \rho.

(Thm 2.1.) If f is an entire function that has an order of growth \le \rho, then:

n(r) \le Cr^{\rho} for some C>0 and all sufficiently large r.

If z_{1},z_{2},… denote the zeros of f, with z_{k} \neq 0, then for all s > \rho we have \sum_{k=1}^{\infty} \frac{1}{|z_{k}|^{s}} < \infty.

(subsection 3) Infinite products 

(subsubsection 3.1.) Generalities

(Def) Given a sequence {a_{n}}_{n=1}^{\infty} of complex numbers, we say that the product \prod_{n=1}^{\infty} (1+a_{n}) converges if the limit \lim_{N \to \infty} \prod_{n=1}^{\infty}(1+a_{n}) of the partial products exists.

(Prop 3.1.) If \sum |a_{n}| < \infty, then the product \prod_{n=1}^{\infty} (1+a_{n}) converges. Moreover, the product converges to 0 iff one of its factors is 0.

(prop 3.2.) Suppose {F_{n}} is a sequence of holomorphic functions on the open set \Omega. If there exist constatns c_{n} >0 s.t. \sum c_{n} < \infty and |F_{n}(z) – 1| \le c_{n} for all z \in \Omega, then

The product \prod_{n =1}^{\infty} F_{n}(z) converges unifotmly in \Omega to a holomorphic function F(z).

If F_{n}(z) does not vanish for any n, then \frac{F’(z)}{F(z)} = \sum_{n=1}^{\infty} \frac{F’_{n}(z)}{F_{n}(z)}.

(subsubseciton 3.2.) Example : The product formula for the sine function

(prop) \frac{sin \pi z}{\pi} = z \prod_{n=1}^{\infty} (1-\frac{z^{2}}{n^{2}}).

(subsection 4) Weierstrass infinite products

(Thm 4.1.) Given any sequence {a_{n}} of complex numbers with |a_{n}| \to \infty as n \to \infty, there exists an entire function f that vanishes at all z = a_{n} and nowhere else. Any other such entire function is of the form f(z) e^{g(z)}} , where g is entire.

(Def) For each integer k \ge 0 we define canonical factors by E_{0}(z) = 1-z and E_{k}(z) = (1-z)e^{z + z^{2}/2 + \cdot + z^{k}/k}, for k \ge 1. The integer k is called the degree of the canonical factor.

(Lem 4.2.) If |z| \le 1/2, then |1-E_{k}(z)| \le c|z|^{k+1} for some c>0.

(subsection 5) Hadamard’s factorization theorem

(Thm 5.1.) Suppose f is entire and has growth order \rho_{0}. Let k be the integer so that k \le \rho_{0} < k+1. If a_{1}, a_{2}, … denote the (non-zero) zeros of f, then f(z) = e^{P(z)} z^{m} \prod_{n=1}^{\infty} E_{k}(z/a_{n}) , where P is a polynomial of degree \le k, and m is the order of the zero of f at z = 0.

(Lem 5.2.) The canonical products satisfy |E_{k}(z)| \ge e^{-c|z|^{k+1}} if |z| \le 1/2 and |E_{k}(z)} \ge |1-z| e^{-c’|z|^{k}} if |z| \ge 1/2.

(Lem 5.3.) For any s with \rho_{0} < s < k+1, we have |\prod_{n=1}^{\infty} E_{k} (z/a_{n})| \ge e^{-c|z|^{s}}, except possibly when z belongs to the union of the discs centered at a_{n} of radius |a_{n}|^{-k-1}, for n = 1,2,3,…

(Cor 5.3.) There exists a sequence of radii, r_{1},r_{2},…, with r_{m} \to \infty, s.t. |\prod_{n=1}^{\infty} E_{k}(z/a_{n})| \ge e^{-c|z|^{s}} for |z| = r_{m}.

(Lem 5.5.) Suppose g is entire and u = Re(g) satisfies u(z) \le Cr^{s} whenever |z| = r for a sequence of positive real numbers r that tends to infinity. Then g is polynomial of degree \le s.

