---



layout: post



title : [Calculus on Manifolds] Differentiation



date : 2018-01-20 11:53:04 +0900



---

(Section 2) Differentiation

(subsection) Basic Definition

(Def) A function f : \mathbf{R}^{n} \to \mathbf{R}^{m} is differentiable at a \in \mathbf{R}^{n} if there is a linear transformation \lambda : \mathbf{R}^{n} \to \mathbf{R}^{m} s.t. \lim_{h \to 0} \frac{|f(a+h) – f(a) - \lambda(h)| }{|h|} = 0.

The linear transformation \lambda is denoted Df(a) and called the derivative of f at a.

(Thm 2.1) If f : \mathbf{R}^{n} \to \mathbf{R}^{m} is differentiable at a \in \mathbf{R}^{n}, there is a unique linear transformation \lambda : \mathbf{R}^{n} \to \mathbf{r}^{m} s.t. \lim_{h \to 0} \frac{|f(a+h) – f(a) - \lambda(h)| }{|h|} = 0.

(Def) The matrix of Df(a) : \mathbf{R}^{n} \to \mathbf{R}^{m} with respect to the unsual bases of \mathbf{R}^{n} and \mathbf{R}^{m}, this m \times n matrix is called the Jacobian matrix of f at a, and denoted f’(a).

(prop) a function f : \mathbf{R}^{n} \to \mathbf{R}^{m} to be differentiable on A if f is differentiable at a for each a \in A. If f : A \to \mathbf{R}^{m} , then f is called differentiable if f can be extended to a differentiable function on some open set containing A.

(subsection) Basic Theorems

(Chain Rule) (Thm 2.2) If f : \mathbf{R}^{n} \to \mathbf{R}^{m} is differentiable at a, and g : \mathbf{R}^{m} \to \mathbf{R}^{p} is differentiable at f(a), then the composition g \bullet f : \mathbf{R}^{n} \to \mathbf{R}^{p} is differentiable at a, and D(g \bullet f ) (a) = Dg(f(a)) \bullet Df(a).

(Thm 2.3) 

If f : \mathbf{R}^{n} \to \mathbf{R}^{m} is a constant function (that is, if for some y \in \mathbf{R}^{m} we have f(x) = y for all x \in \mathbf{R}^{n}), then Df(a) = 0.

If f : \mathbf{R}^{n} \to \mathbf{R}^{m} is a linear transformation, then Df(a) = f.

If f : \mathbf{R}^{n} \to \mathbf{R}^{m}, then f is differentiable at a \in \mathbf{R}^{n{ iff each f^{i} is, and Df(a) = (Df^{1}(a), \cdots, Df^{m}(a)). Thus f’(a) is the m \times n matrix whose ith row is (f^{i})’(a).

If s : \mathbf{R}^{2} \to \mathbf{R} is defined by s(x,y) = x + y, then Ds(a,b) = s.

If p : \mathbf{R}^{2} \to \mathbf{R} is defined by p(x,y) = x \cdots y, then Dp(a,b)(x,y) = bx + ay. Thus p’(a,b) = (b,a).

(Cor 2.4) If f,g : \mathbf{R}^{n} \to \mathbf{R} are differentiable at a, then D(f+g)(a) = Df(a) + Dg(a), D(f \cdot g) (a) = g(a)Df(a) + f(a) Dg(a). If, moreover, g(a) \neq 0, then D(f/g)(a) = \frac{g(a)Df(a) – f(a)Dg(a)}{[g(a)]^{2}}.

(subsection) Partial Derivatives

(Def) If f : \mathbf{R}^{n} \to \mathbf{R} and a \in \mathbf{R}^{n} , the limit \lim_{h \to 0} \frac{f(a^{1}, \cdots, a^{i} +h, \cdots, a^{n}) – f(a^{1}, \cdots, a^{n}) } {h} if it exists, is denoted D_{i}f(a), and called the ith partial derivative of f at a.

(Def) If D_{i}f(x) exists for all x \in \mathbf{R}^{n}, we obtain a function D_{i}f : \mathbf{R}^{n} \to \mathbf{R} . The jth partial derivative of this function at x, that is, D_{j}(D_{i}f) (x) , is often denoted D_{i,j} f(x).

(Thm 2.5) If D_{i,j} f and D_{j,i} f are continuous in an open set containing a, then D_{i,j} f(a) = D_{j,i} f(a). The function D_{i,j} f is called a second-order (mixed) partial derivative of f.

(prop) the order of i_{1}, \cdots, i_{k} is immaterial in D_{i1, \cdots, ik} f if f has continuous partial derivatives of all orders. A function with this property is called a C^{\infty} function.

(Thm 2.6) Let A \subset \mathbf{R}^{n}. If the maximum (or minimum) of f : A \to \mathbf{R} occurs at a point a in the interior of A and D_{i}f(a) exists, then D_{i}f(a) = 0.

(subsection) Derivatives

(Thm 2.7) If f : \mathbf{R}^{n} \to \mathbf{R}^{m} is differentiable at a, then D_{j}f^{i}(a) exists for 1 \le i \le m, 1 \le j \le n and f’(a) is the m \times n matrix (D_{j}f^{i}(a)).

(Thm 2.8) If f : \mathbf{R}^{n} \to \mathbf{R}^{m}, then Df(a) exists if all D_{j}f^{i}(x) exists in an open set containing a and if each function D_{j}f^{i} is continuous at a. Such a function f is called continuously differentiable at a.

(Thm 2.9) Let g_{1} , \cdots, g_{m} : \mathbf{R}^{n} \to \mathbf{R} be continuously differentiable at a, and let f : \mathbf{R}^{m} \to \mathbf{R} be differentiable at (g_{1}(a), \cdots, g_{m}(a)). Define the function F : \mathbf{R}^{n} \to \mathbf{R} by F(x) = f(g_{1}(x), \cdots, g_{m}(x)). Then D_{i}F(a) = \sum_{j = 1}^{m} D_{j}f(g_{1}(a), \cdots, g_{m}(a)) \cdot D_{i}g_{j}(a).

(prop) for the function F : \mathbf{R}^{2} \to \mathbf{R} defined by F(x,y) = f(g(x,y), h(x),k(y)) where h,k : \mathbf{R} \to \mathbf{R}. Letting a = (g(x,y), h(x), k(y)), we obtain D_{1}F(x,y) = D_{1}f(a) \cdot D_{1}g(x,y) + D_{2} f(a) \cdot h’(a), D_{2}F(x,y) = D_{1}f(a) \cdot D_{2}g(x,y) + D_{3}f(a) \cdot k’(y).

(subsection) Inverse Functions

(Lem 2.10) Let A \subset \mathbf{R}^{n} be a rectangle and let f : A \to \mathbf{R}^{n} be continuously differentiable . If there is a number M s.t. |D_{j}f^{i}(x) | \le M for all x in the interior of A< then |f(x) – f(y)| \le n^{2} M|x-y| for all x, y \in A.

(Inverse Function Theorem) (Thm 2.110 Suppose that f : \mathbf{R}^{n} \to \mathbf{R}^{n} is continuously differentiable in an open set containing a, and det f’(a) \neq 0. Then there is an open set V containing a and an open set W containing f(a) s.t. f : V \to W has a continuous inverse f^{-1} : W \to V which is differentiable and for all y \in W satisfies (f^{-1})’(y) = [f’(f^{-1}(y))]^{-1}.

an inverse function f^{-1} may exist even if det f’(a) = 0. However, if det f’(a) = 0, then f^{-1} cannot be differentiable at f(a).

(subsection) Implicit Functions

(Implicit Function Theorem) (Thm 2.12) Suppose f : \mathbf{R}^{n} \times \mathbf{R}^{m} \to \mathbf{R}^{m} is continuously differentiable in an open set containing (a,b) and f(a,b) = 0. Let M be the m \times m matrix (D_{n+j}f^{i}(a,b)) 1 \le i,j \le m. If det M \neq 0, there is an open set A \subset \mathbf{R}^{n} containing a and an open set B \subset \mathbf{R}^{m} containing b, with the following property : for each x \in A there is a unique g(x) \in B s.t. f(x,g(x)) = 0. The function g is differentiable. These functions are said to be defined implicitly by the equation f(x,y) = 0.

(Thm 2.13) Let f : \mathbf{R}^{n} \to \mathbf{R}^{p} be continuously differentiable in an open set containing a, where p \le n. If f(a) = 0 and the p \times n matrix(D_{j}f^{i}(a)) has rank p, then there is an open set A \subset \mathbf{R}^{n} containing a and a differentiable function h : A \to \mathbf{R}^{n} with differentiable inverse s.t. f \bullet h (x^{1}, \cdots, x^{n}) = (x^{n-p+1}, \cdots, x^{n}).

