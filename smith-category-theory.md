# Smith, *Category Theory*

## 9. Pairs and products, pre-categorially

In this chapter, Smith studies *pairing schemes*. A pairing scheme allows one to pair up objects that belong to pluralities of objects $\mathrm{X}$ and $\mathrm{Y}$ (following Smith, upright symbols do not denote sets but simply 'some objects', plural).

Initially such a scheme consists of four parts: Some objects $\mathrm{O}$ to serve as the pairs, projection functions $\pi_1 \colon \mathrm{O} \to \mathrm{X}$ and $\pi_2 \colon \mathrm{O} \to \mathrm{Y}$ that sends a pair object to each of its parts, and a (genuinely) two-place pairing function $\mathit{pr} \colon \mathrm{X},\mathrm{Y} \to \mathrm{O}$. These must satisfy the obvious properties:

1. $\pi_1(\mathit{pr}(x, y)) = x$ and $\pi_2(\mathit{pr}(x, y)) = y$ for all $x$ that are among the $\mathrm{X}$ and all $y$ among the $\mathrm{Y}$.
2. $\mathit{pr}(\pi_1 o, \pi_2 o) = o$ for all $o$ among the $\mathrm{O}$.

Smith then proves that the pairing function is unique given the projections. More precisely, given $\mathrm{O}$, $\pi_1$ and $\pi_2$, if there is *any* pairing function $\mathit{pr}$ that makes these four items into a pairing scheme, then there is a *unique* such $\mathit{pr}$. (He also shows the opposite, that $\pi_1$ and $\pi_2$ are uniquely determined by $\mathit{pr}$.) And this surely makes sense: The projections already tell us the two parts of each pair object, so given $x$ and $y$ there should be a unique $o$ that has $x$ and $y$ as its parts.

Next Smith proves that given $\mathrm{O}$, $\pi_1$ and $\pi_2$, if there is a *unique* $\mathit{pr}$ such that the first property above holds, then that in fact constitutes a pairing scheme. In other words, we require that for each pair of objects $x$ and $y$ there is a unique $o$ among the $\mathrm{O}$ such that $\pi_1 o = x$ and $\pi_2 o = y$. First of all, this is certainly a property of pairing schemes as we notes above: $\mathit{pr}$ is uniquely determined by $\pi_1$ and $\pi_2$.

But notice that this is exactly what we want from a pairing scheme. For each $x$ and $y$ we want at least some $o$ whose parts are $x$ and $y$. But we also want that $o$ to be unique, for the $\mathrm{O}$ are just supposed to be *pairs* of elements among $\mathrm{X}$ and $\mathrm{Y}$, and so each $o$ should have no other properties than its two parts. In other words, it should be uniquely determined by its projections $\pi_1 o$ and $\pi_2 o$.

Smith then lifts this to a definition: $\mathrm{O}$, $\pi_1$ and $\pi_2$ form a *product* of $\mathrm{X}$ with $\mathrm{Y}$ if for each $x$ and $y$ there is a unique $o$ among the $\mathrm{O}$ such that $\pi_1 o = x$ and $\pi_2 o = y$. If we had a pairing scheme for pairing $\mathrm{X}$ with $\mathrm{Y}$, then we would surely have a product. But the above discussion shows that the converse also holds: The projections in the product, given the uniqueness assumption, uniquely determine a pairing function $\mathit{pr}$, and so we end up with a pairing scheme.

The difference between a pairing scheme and a product is then simply that we have substituted the pairing function (and property 2 above) for the uniqueness of pair objects. And these are equivalent.