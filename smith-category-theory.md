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


## 14. Quotients, pre-categorially

### Equialence relations in general, and equivalence kernels

First notice that if $R$ and $E$ are relations defined over some objects $\mathrm{Y}$, where $E$ is an equivalence relation, then for the reflexive, symmetric, transitive closure $\overline{\overline{R}}$ of $R$ to be contained in $E$, it suffices that $R$ is contained in $E$. This follows since $\overline{\overline{R}}$ by definition is the smallest equivalence relation that contains $R$. The existence of such an equivalence relation follows in one of two ways:

1. If we have access to intersections of arbitrary collections of relations, we can simply take the intersection of all equivalence relations that contain $R$, of which there is at least one, namely the trivial relation on $\mathrm{Y}$ identifying all objects. This is e.g. possible if $Y$ is a set, since then there is only a set's worth of equivalence relations on $Y$, and so we can take their intersection.
2. If not, then we may proceed as follows: First extend $R$ by making all instances of the form $yRy$ true, which makes $R$ reflexive. Next add instances of the form $y'Ry$ whenever $yRy'$ is already true. This makes $R$ symmetric, and it preserves reflexivity. Finally if $yRy'$ and $y'Ry''$ are already true, then add $yRy''$, making $R$ transitive. This again obviously preserves reflexivity, and notice that it also preserves symmetry: For if $yRy''$ is now true, then either it already was before making $R$ transitive, or else there is some $y'$ such that $yRy'$ and $y'Ry''$ were true before. But $R$ was symmetric before making it transitive, so in the first case we also had $y''Ry$. In the latter case we would then also have $y'Ry$ and $y''Ry'$, but then taking the transitive closure we would get $y''Ry$. Hence $R$ is still symmetric.

Then notice that if some function $k \colon \mathrm{Y} \to \mathrm{Z}$ respects $R$, then $R$ is contained in the equivalence kernel $E_k$. But then $\overline{\overline{R}}$ is also contained in $E_k$.


### Equivalence projections

As far as I know, the term 'equivalence projection' was introduced by Smith and is not common terminology. It is not immediately clear why equivalence projections are interesting.

Given a function $k \colon \mathrm{Y} \to \mathrm{Z}$, is there some natural (equivalence) relation on $\mathrm{Y}$ determined by $k$? Indeed, the equivalence kernel $E_k$ of $k$: Say that $y E_k y'$ if there is some $z$ such that $k(y) = z$ and $k(y') = z$. But given a function $f \colon \mathrm{X} \to \mathrm{Y}$, is there now a natural relation on $\mathrm{Y}$ determined by $f$? By analogy with equivalence kernels, we might try to define a relation $R_f$ on $\mathrm{Y}$ by saying that $y R_f y'$ if there is an $x$ such that $f(x) = y$ and $f(x) = y'$. But this is not very useful, since then $R_f$ would simply be equality on the image of $f$.

Instead, consider a more general kind of relation: If $h \colon \mathrm{Y} \to \mathrm{Z}$ is another function, say that $y E_{kh} y'$ if $k(y) = h(y')$, i.e. if there is some $z$ such that $k(y) = z$ and $h(y') = z$. This is clearly not an equivalence relation in general, since for it to be reflexive we must have $k = h$. Why this should be interesting to consider is also not quite clear, but it seems an obvious generalisation of equivalence kernels. In fact, given $n$ functions we may analogously define an $n$-place relation on $\mathrm{Y}$.

If we then have another function $g \colon \mathrm{X} \to \mathrm{Y}$, say that $y R_{fg} y'$ if there is some $x$ with $f(x) = y$ and $g(x) = y'$. Taking the reflexive, symmetric and transitive closure we obtain the equivalence projection $\overline{\overline{R_{fg}}}$.