## <b>Convex functions</b>
---

### <center><b>Definition</b></center>
$f$ is concave if $-f$ is convex

### <center><b>Examples on R</b></center>

convex:
- affline: $ax+b$ on $\mathbf{R}$
- exponential: $e_{ax}$, for any $a\in\mathbf{R}$
- powers: $x^\alpha$
- powers of absolute value
- negative entropy $x\log{x}$ on $\mathbf{R_{++}} $

concave:
- affine
- power $x_{\alpha} on $ \mathbf{R_{++}}$, for $0\leq \alpha \leq 1$
- logarith

### <center><b> Examples on R^n and R^{$m\times n$}</b> </center>
affine functions are convex and concave, all norms are convex
eg. $R^n$
- affine
- norms: 

eg. $\mathbf{R^{m \times n}}$:
- affine
- spectral( maximum singular value) norm
$$ 
f(X) = \lVert X \lVert _2 = \sigma_{max}(X) = ( \lambda _{max}(X_T X))^{1/2}
$$

### <center><b>Restriction of a convex function to a line</b></center>
$ f: R^n \to R$ is convex iff. 
$$g(t) = f(x+tv)$$
is convex
eg. 
$$
\begin{align*}
g(t) &= &\log \det{(X+tV)} = & \log \det X + \log \det(I + tX^{-1/2}VX^{-1/2}) \\
& & =& \log \det X + \sum^n_{i=1} \log(1+t \lambda _i)
\end{align*}
$$

### <center><b>Extended-value extension</b></center>
$$
\tilde{ f }(x) = f(x), \ \ \ x\in \text{dom} f, \ \ \ \tilde{f}(x) = \infty, x\notin \text{dom} f 
$$

### <center><b> First-order condition</b></center>
$f$ is cvx iff.
$$
f(y) \geq f(x) + \nabla f(x)^T(y-x)
$$

### <center><b> Second-order conditions</b></center>
- f is cvx iff 
$$\nabla ^2 f(x) \succeq 0 \ \ \ \text{for all } x\in \text{dom} f$$
- if $\nabla^2 f(x) \succeq 0 $ for all $x\in$ dom $f$, then $f$ is strictly cvx.

### <center><b> Examples </b></center>
- **quadratic function**:
- **least-squares objective**:
- **quadratic-over-linear**:
- **log-sum-exp**:
- **geometrix mean**: is concave

### <center><b> Epigraph and sublevel set</b></center>

$\alpha$-**sublevel** set of $f:\mathbf{R}^n \to \mathbf{R}$:
$$
C_\alpha =
\{x\in \text{dom}f|f(x) \leq \alpha\}
$$
sublevel sets of convex functions are convex  
**epigraph** of $f:\mathbf{R}^n \to \mathbf{b}$  
$f$ is convex iff. epi $f$ is a convex set

### <center><b> Operations that preserve convexity</b></center>
- nonnegative weighted sum
- composition with affine function
- pointwise maximum and supremum
- composition
- minization
- perspecive

### <center><b> Quasiconvex functions</b></center>
$f: \mathbf{R}^n \to \mathbf{R} $ is quasiconvex if *dom* $f$ is convex and the sublevel sets:
$$ S_\alpha = \{ x \in \text{dom} f | f(x) \leq \alpha \}$$
are convex for all $\alpha$
- $f$ is quasiconcave if $-f$ is quasiconvex
- $f$ is quasilinear if $f$ is quasiconvex and quasiconcave
- **Quasiconvex Properties**
    - modified Jensen inequaliy 
    $$ 0 \leq \theta \leq 1 implies f(\theta x + (1-\theta)y) \leq \max \{ f(x), f(y)\} $$
    - first-order condition:
    $$ f(y) \leq f(x) \implies \nabla f(x) ^T (y-x) \leq 0 $$

### <center><b>Log-concave and log-convex functions</b></center> 
a positive function $f$ is log-concave if $\log f$ is concave:
$$ f(\theta x+(1-\theta)y) \geq f(x)^\theta f(y)^{1-\theta} \text{for} 0 \leq \theta \leq 1$$

- intergration: if $f: \mathbf{R}^n \times \mathbf{R}^m \to R $ is log-concave then 
$$ g(x) = \int f(x, y) dy $$ 
is log concave


### <center><b>Convexity with respect to generalized inequalities</b></center>


## <b>Convex optimization problems</b>
---


















