# Mathematics resources

This is an attempt to collect notes on mathematics resources I have used and continue to use. It is not meant to be authoritative or exhaustive, but perhaps someone might benefit from my thoughts on the resources below.

The entries in each main section are listed roughly in 'recommended reading order', insofar as I recommend each resource! Unless otherwise stated, you can assume that I have in fact found each entry worthy of recommendation.

The list is (clearly) far from complete. I will add to it whenever I feel like it!

## Contents

- [Mathematics resources](#mathematics-resources)
  - [Contents](#contents)
  - [Analysis](#analysis)
    - [Introductory real analysis](#introductory-real-analysis)
    - [Complex analysis](#complex-analysis)
    - [Measure and integration theory](#measure-and-integration-theory)
    - [Probability theory](#probability-theory)
    - [Functional and harmonic analysis](#functional-and-harmonic-analysis)
  - [Algebra](#algebra)
    - [Linear algebra](#linear-algebra)
    - [Abstract algebra](#abstract-algebra)
    - [Representation theory](#representation-theory)
    - [Category theory](#category-theory)
  - [Topology and geometry](#topology-and-geometry)
    - [Point-set topology](#point-set-topology)
    - [Algebraic topology](#algebraic-topology)
    - [Topological groups and vector spaces](#topological-groups-and-vector-spaces)
    - [Differential topology and geometry](#differential-topology-and-geometry)
    - [Riemannian geometry](#riemannian-geometry)
  - [Mathematical physics](#mathematical-physics)
  - [Order theory](#order-theory)
  - [Logic](#logic)
    - [Propositional and first-order logic](#propositional-and-first-order-logic)
    - [Second-order logic](#second-order-logic)
    - [Set theory](#set-theory)
    - [Computability theory](#computability-theory)
    - [Model theory](#model-theory)
  - [Linguistics](#linguistics)
  - [Philosophy](#philosophy)
  - [Physics](#physics)
    - [Quantum mechanics](#quantum-mechanics)
  - [Computer science](#computer-science)
    - [Algorithms and data structures](#algorithms-and-data-structures)
    - [Computer architecture](#computer-architecture)
    - [Operating systems](#operating-systems)
    - [Haskell](#haskell)

## Analysis

### Introductory real analysis

By this I mean basically everything that does not require measure theory, and which doesn't fall under more specific headings such as differential equations.

The first order of business is to become familiar with the theory of continuous functions between Euclidean spaces, or better yet metric spaces. This required some knowledge of the topology of the spaces in question, and the books below should cover the necessary material.

Next, on to differentiation and integration, which can be done in varying levels of generality. I personally like the Riemann-Stieltjes integral (see Rudin or especially Apostol below) since it provides an obvious but useful generalisation of the ordinary Riemann (or Darboux) integral, and serves as a first step towards things like like integrals.

Finally, multidimensional analysis, in particular differentiation of functions between general Euclidean spaces (or maybe even infinite-dimensional spaces!), and integration of them as well. The theory of differentiation is very important, but I feel like it is perfectly possible to do without much knowledge of multidimensional Riemann integrals. The Lebesgue integral is just so much nicer, and you will want to become intimately familiar with it down the line anyway.

1. Rudin, *Principles of Mathematical Analysis*. The classic. It is a bit light on content, and certainly the later chapters should be avoided: the material on differential forms and the Lebesgue integral is better found elsewhere.

    Things I especially like: The coverage of the exponential function, first in an 'early transcendentals' fashion, defining it first for integer, then rational and finally real exponents, and later reconciling this with the 'late transcendentals' definitions in terms of integrals and power series (I also cover the exponential function in [my own notes](https://github.com/dnhansen/math-analysis)). The introduction of perfect sets is also interesting and yields a topological proof of the uncountability of the reals.


2. Apostol, *Mathematical Analysis*. Another classic, often compared to Rudin's book. I tend to prefer Apostol's treatment of the basic material, it is more complete and less terse, but they complement each other well.

    Things to like: An excellent coverage of metric space topology, though with a different focus than Rudin. It also treats Riemann-Stieltjes integrals in great generality, and contains basically everything you could ever want to know about Riemann integration (in [my own notes](https://github.com/dnhansen/math-analysis) I give a streamlined presentation of Riemann-Stieltjes integrals, among other things using nets, and correcting a couple of mistakes in Apostol's proofs).

3. Duistermaat, Kolk, *Multivariate Real Analysis*. Assumes knowledge of one-dimensional analysis as covered in one of the books above. Covers multidimensional differential and integral calculus in a very modern fashion, especially the former, and also gets into some basic theory of manifolds (though only submanifolds of Euclidean space). It also covers the antidifferentiation problem in higher dimension, though in a rather unsatisfying fashion by only considering (not even piecewise) continuously differentiable curves and differentiable homotopies. But what it does it does do well.

    The best part of the book is the very large number of excellent exercises! For instance, a sequence of exercises guides the reader through a derivation of (versions of) the Helmholtz-Weyl and Hodge decompositions, Maxwell's equations in covariant form, invariance of the wave equation under Lorentz transformations, and much more. All without assuming, as geometers are want to do, that every manifold and every vector field under the sun is smooth!

4. Zorich, *Mathematical Analysis*.

### Complex analysis

1. Rao, Stetkær, Fournais, Møller, *Complex Analysis: An Invitation*.
2. Ullrich, *Complex Made Simple*.


### Measure and integration theory

I initially learnt measure theory from Steen Thorbjørnsen's *Grundlæggende mål- og integralteori*, so I don't know how good the books below are for beginners. (Thorbjørnsen's book is excellent as an introduction. It is very clearly written with great exercises, and the only prerequisites are first-year analysis and linear algebra.)

1. Bauer, *Measure and Integration Theory*. I haven't read most of this book, but it seems like a perfectly respectable first introduction to measure theory. If the 'sequel' *Probability Theory* (see [below](#probability-theory)) is any indication, this book is certain to be clear and well-motivated.

    The parts that I *have* read are, first of all: The sections on product measures and convolutions of measures. Both of these are excellent, and the latter in particular is a great way to pick up the results about convolutions needed in probability theory. And secondly the section on convergence of Radon measures, in which Bauer introduces vague and weak convergence of measures, both of which are of central importance in probability theory. This is only done in any detail for measures on locally compact Hausdorff spaces, so for the corresponding theory for metric spaces one must go elsewhere (see e.g. Billingsley [below](#probability-theory)).

    Note however that Bauer's Radon measures are *inner* regular instead of *outer* regular. See my notes on Schwartz' *Radon Measures on Arbitrary Topological Spaces and Cylindrical Measures* below.

2. Cohn, *Measure Theory*. As with Bauer above I haven't read much of this book, but it seems a quite popular introduction to the subject. Some highlights:

    - Chapter 4 on signed and complex measures is excellent, much preferrable to e.g. Folland's approach, though I do prefer Folland's treatment of functions of bounded variation.
    - Chapter 8 on Polish spaces is a great introduction to the subject.
    - Section 10.6 on construction of probability measures (including the Kolmogorov consistency theorem) is a good supplement to Folland and Bauer (see [below](#probability-theory) for the latter) who all take different approaches.

3. Folland, *Real Analysis*. Perhaps not the best *introduction* to measure and integration theory, but it is great as a second book on the subject. Some chapters are certainly better than others:

    - Chapter 1, Measures: Skip the results on products of $\sigma$-algebras and see instead [these notes](https://github.com/dnhansen/topology-measure-theory-notes). Many results on e.g. outer measures are fairly obvious geometrically.
    - Chapter 2, Integration: For convergence in measure, see instead [these notes](https://github.com/dnhansen/math-analysis).
    - Chapter 3, Signed Measures and Differentiation: §§3.4-5 on differentiation and functions of bounded variation can be skipped on first reading, though they really are fundamental topics. See [this question](https://math.stackexchange.com/questions/3806610/folland-complex-measures-total-variation-definition) on StackExchange about the total variation of complex measures, though as mentioned above I prefer Cohn's treatment.
    - Chapter 4, Point Set Topology: For nets (and filters) and Tychonoff's theorem, see instead [these notes](https://github.com/dnhansen/topology-nets-filters). Arzelà-Ascoli can be skipped on first reading, and so can §4.8 about embeddings in cubes.
    - Chapter 5, Elements of Functional Analysis: For more on topological vector spaces, see [these notes](https://github.com/dnhansen/topological-groups).
    - Chapter 6, $L^p$ Spaces: For completeness, see [these notes](https://github.com/dnhansen/math-analysis). §6.2 on duality can be skipped if the proof of Minkowski's inequality for integrals is replaced by the proof I give in [these notes](https://github.com/dnhansen/folland-real-analysis) (this proof mimics the usual proof of Minkowski's inequality). Apart from this inequality, §§6.3-5 can be skipped on a first reading, though ideally take note of the Riesz-Thorin interpolation theorem since it is an important tool in e.g. Fourier analysis (the [Wikipedia page](https://en.wikipedia.org/wiki/Riesz%E2%80%93Thorin_theorem) has a nice geometric interpretation of part of the theorem).
    - Chapter 7, Radon Measures: §7.4 on products of Radon measures can be skipped on a first reading, though note that they are used in e.g. harmonic analysis.
    - Chapter 8, Elements of Fourier Analysis: See [these notes](https://github.com/dnhansen/folland-real-analysis) for a proof of the Plancherel theorem that does not use the Schwartz space. While §8.4 is fairly technical and can be skipped, §8.5 is central and uses only the basic results on functions of bounded variation. The material in §8.6 is probably covered better elsewhere (e.g. in Bauer).
    - Chapter 9, Elements of Distribution Theory: See [these notes](https://github.com/dnhansen/folland-real-analysis) for a proof of the fundamental lemma of the calculus of variations that does not use the theory of differentiation.

    Some issues I have with the book: Folland doesn't assume any knowledge of topological spaces, so many theorems in the first half of the book are stated for metric spaces even though they generalise immediately. Some of the proofs are also less than clear for this reason. A few theorems are also proven in less than full generality, even though they would be no less difficult to state or prove more generally. So keep your eye out, and if it seems like something can be generalised, it probably can.

4. Schwartz, *Radon Measures on Arbitrary Topological Spaces and Cylindrical Measures*. By the master himself. Reading e.g. Bauer and Folland above, one realises that there are (at least) two different ways of construing Radon measures: Bauer requires a Radon measure to be locally finite and inner regular, while Folland requires it to be outer regular, inner regular on open sets, and finite on compact sets. Bauer actually considers these Folland-type Radon measures as well, but the bulk of his discussion concerns the former kind.

    If one, like I do, prefers Folland's treatment of Radon measures, including e.g. his proof of the Riesz representation theorem (which uses the full force of Urysohn's lemma and Carathéodory's theorem), then how does one get to understand the connection to Bauer's Radon measures? Schwartz presents the connection between them very explicitly, though not always very *clearly*. It is also a quite old book, the typography is lacking and it is difficult to see the forest for the trees. I also have a [note](https://github.com/dnhansen/radon-measures) (work in progress) that explains Radon measures in more detail.

5. Rudin, *Real and Complex Analysis*. A much loved textbook, though I am not a huge fan. At least the approach to measure theory is a bit annoying, since Rudin only considers measurable functions with values in a topological space, which is just not sufficient.

    The rest of the first part of the book is *fine*, though I think it shows its age. The words 'Radon measure' appear a single time the whole book, namely in the end notes. The proof of the Riesz representation theorem is also stereotypically Rudin: six plus pages of exhausting mathematics without much motivation.

    I haven't read the second part on complex analysis, so I won't comment on it.


### Probability theory

1. Bauer, *Probability Theory*.

2. Billingsley, *Convergence of Probability Measures*.

3. Kallenberg, *Foundations of Modern Probability*. A massive tome which I can't claim to have read. From perusing it it does seem a bit terse and perhaps not great to learn from. One specific issue I have with it is Kallenberg's focus on *second-countable* locally compact Hausdorff spaces, which is just not necessary for e.g. the Riesz representation theorem.

### Functional and harmonic analysis

1. Folland, *Real Analysis*.

2. Rudin, *Functional Analysis*. The classic text on functional analysis. Covers: topological vector spaces and related topics, distribution theory and the Fourier transform, Banach and C*-algebras, bounded and unbounded operators on Hilbert space.

    The coverage of topological vector spaces is quite nice and elementary, if a bit old-fashioned. I would have liked a more explicit mention of the topological properties of TVSs, for instance that a not necessarily T1 TVS is regular, and that T0 is sufficient for a TVS is T1, and hence T3 (perhaps even a mention of the T0 identification). But it is easy enough to fill in these details if you know the topology, which can be glanced from e.g. Willard's book (see [below](#point-set-topology)). I also have a [set of notes](https://github.com/dnhansen/topological-groups) which contains most of the elementary material on topological vector spaces that Rudin uses, as well as an introduction to topological groups.

3. Conway, *A Course in Functional Analysis*.
4. Folland, *A Course in Abstract Harmonic Analysis*.
5. Helemskii, *Lectures and Exercises on Functional Analysis*.

## Algebra

### Groups

1. Aluffi: Chapters II and IV. Can skip §II.10, §IV.2.5, Proposition IV.3.5 and §IV.3.3, and §IV.4.4 (though note the statement of Theorem 4.20 as well as Corollary 4.21). Finally, §IV.5 can be postponed until after chapter III has been read.
2. Rotman part I: The definition of normal series on p. 192 through Theorem A-5.30, except Lemma A-5.21. Skip the proofs of Propositions A-5.22 through A-5.25
3. Rotman part II: TODO anything interesting?
4. Rotman groups: Chapter 5 from p. 102, also Krull-Schmidt in chapter 6 from p. 144. Also stuff in chapter 7, also postpone until Aluffi chapter III.
5. Grove
6. Broué: §§5.1-2

### Rings

1. Aluffi: Chapters III and V. Also covers basics of modules needed to understand rings.
2. Rotman A-3? B-1/2?
3. Broué: Chapters 2, 3, 6

### Fields

1. Aluffi: Chapter VII
2. Rotman A-5?
3. Leinster?

### Modules

1. Aluffi: Chapters VI and VIII
2. Rotman B-1/2/3/4/5?
3. Broué?

### Homological algebra

1. Aluffi: Chapter IX
2. Rotman C-3/4?

### Commutative algebra

1. Rotman B-6, C-5?
2. Altman, Kleiman


### Lie algebras? Or under rep theory?

1. Rotman?
2. Jacobson

### Representation theory

1. Steinberg
2. Rotman?
3. Weintraub?
4. Quivers
5. Broué: §§5.3-4, part IV?

### Misc

1. Marsh Cluster algebras?
2. Springer Linear algebraic groups? (more like alg geo)



### Linear algebra

1. Hoffman, Kunze, *Linear Algebra*. I don't know if this might be too ambitious for beginners, but if you know a thing or two about matrices it's a very good second look at linear algebra

    I particularly like the section on determinants. Hoffman and Kunze first prove the existence of determinant functions through the Laplace expansion, and then later shows that a determinant function must have a certain form (which is just the Leibniz definition of the determinant). The uniqueness is then used to e.g. prove the multiplicativity of determinants. I do something similar in [my own linear algebra notes](https://github.com/dnhansen/linear-algebra-notes), which I (for obvious reasons!) prefer.

    At least the later chapters do assume a certain level of mathematical maturity, but the exposition is clear and pleasantly succinct.

2. Roman, *Advanced Linear Algebra*. Assumes some knowledge of basic linear algebra, in particular matrices and determinants, and some abstract algebra. The exposition is very modern, and matrices and systems of equations are used only sparingly in proofs (as they should!).

    Those results that explicitly concern matrices are also handled pleasingly abstractly without unnecessary calculations that hide the structure behind each proof. For instance, Roman proves that the row rank and column rank of a matrix coincide by proving that both ranks are preserved under both elementary row and column operations, and that every matrix can be reduced through these operations to a diagonal matrix with ones and zeros on the diagonal. (This can also be proved using the theory of operator adjoints (not to be confused with *Hermitian* adjoints), avoiding the use of matrices as far as possible. I take this approach in [my notes](https://github.com/dnhansen/linear-algebra-notes).)

    The first part of the book covers both vector spaces and modules before moving on to eigenvalues/-vectors, inner product spaces and normal/self-adjoint operators, though most of this latter material can be appreciated without reading the chapters on modules.

    The second part is then a collection of (with one exception) independent chapters on a wide selection of topics, including bilinear forms, Hilbert spaces, tensor products, and affine geometry.


### Abstract algebra

1. Aluffi, *Algebra: Chapter 0*. 'Chapter 0' is perhaps putting it a bit strongly, but Aluffi only presupposes mathematical maturity and knowledge of the basic properties of the natural through the complex numbers. Some familiarity with linear algebra is also useful for some of the exercises, in particular matrix groups.

    The book starts with a chapter on set theory, functions and relations, and most importantly *category theory*. The latter is covered throughout the book as it becomes more and more important. The first section on category theory covers (locally small) categories, products and coproducts, universal properties, but that's it.

    Other than the categorical focus it is a very standard textbook. It covers groups, rings, modules, fields, and some homological algebra. The exposition is mostly excellent. The treatment of quotient groups is the best I have seen (Aluffi starts with the simple assumption that the natural map from the group to the quotient be a group homomorphism, and the requirement that the subgroup be normal arises naturally from this), and I am left wondering why I haven't seen any other authors take this approach. (I hope this is simply my lack of experience!) This is not to say that there isn't room for improvement, and I try to cover the conceptual holes in [my notes](https://github.com/dnhansen/aluffi-algebra).

    One thing that annoys me: The categorical approach could have been a bit more explicit, and I think some of the results would be more transparent with a slightly stronger background in category theory. For instance, group kernels are given by equalisers, but Aluffi doesn't use this word but simply describes the universal property.

    Also, be aware that the book contains quite a few errors. Luckily the author maintains a list of errata ([first printing](https://www.math.fsu.edu/~aluffi/algebraerrata.2009/Errata.html), [second printing](https://www.math.fsu.edu/~aluffi/algebraerrata.2016/Errata.html)), and it might be wise to keep this close when reading it.

2. Dummit, Foote, *Abstract Algebra*. Two comments:

    First compare Dummit and Foote's treatment of quotient groups to that of Aluffi. There are at least three (elementary) ways of introducing quotient groups:

    1. Quotients by other groups, i.e. objects in the same category. This approach is not applicable to other categories, since e.g. ideals are not rings, hence not objects in the category of rings. But it is a natural approach, and we quickly find that to define an operation on the resulting quotient we require that we divide out by a *normal* subgroup. This seems to be the strategy employed by most modern algebra texts. On the other hand, there is the danger of leaving open the question of whether all relevant equivalence relations are captured by this notion of quotient.
    
    2. Quotients by general equivalence relations. This is the path chosen by Aluffi, and I think it is the most natural. In **Set** we cannot hope to capture the general notion of a quotient by dividing a set *A* by subsets of *A*, so while this is of course possible in **Grp**, it seems natural to take the same approach as in **Set** and then *discover* the notion of quotienting by a normal subgroup.

    3. Quotients by kernels. This is of course equivalent to the first approach, but one only realises this *after* one has developed the theory of quotient groups, and it seems very unnatural if you don't already know why kernels are important in capturing the structure of algebraic objects.

    Secondly, the book includes a *lot* of exercises, many of them very good.


### Representation theory

1. Steinberg, *Representation Theory of Finite Groups*.
2. Weintraub, *Representation Theory of Finite Groups: Algebra and Arithmetic*.


### Category theory

1. Awodey, *Category Theory*. This one carries a big fat 'do not recommend'! At least for beginners. A lot of people seem to like it, and I don't get it. It's sloppy, imprecise and difficult to follow compared to so many other books on category theory.

    For instance, in section 1.4 he introduces the category **Cat** of all categories and functors, but in section 1.8 he apparently retracts this definition and lets **Cat** denote the category of *small* categories. Nevertheless he, for instance in exercise 2 of the first chapter, still wants to talk about isomorphisms of *large* categories despite not having defined what this means.
    
    For another example, in section 2.8 he introduces hom-functors and calls them *the* representable functors. In exercise 18 of the same chapter he asks the reader to show that the forgetful functor from monoids to sets is representable. But what is that supposed to mean? He only introduces natural transformations in chapter 7! See also [this](https://math.stackexchange.com/questions/3299671/why-is-the-forgetful-functor-representable) discussion on StackExchange.

    To its credit, the book does contain a lot of material of particular interest to computer scientists and logicians. But I don't understand why people use it as an introductory text.

2. Smith, *Introducing Category Theory*. This is probably my favourite introduction to category theory. Smith is a logician and philosopher, and as such he is *very* careful when it makes sense to be. While some might find this annoying, I do think it has its place in an introduction to category theory since foundational questions arise almost immediately: Is set theory the only possible foundation for mathematics, and how do we motivate using set theory? What do we even mean by such a foundation? What kinds of properties must we take (or do we want) sets to have, and how do they affect the relationship between set theory and category theory?

    The coverage is fairly standard. The level of abstraction increases very gradually: Smith starts with a survey of groups, mostly to serve as motivation and to highlight some foundational questions, before he defines categories. After a brief detour into subcategories, products and quotients, he stays *inside* a single category while covering all the basic material. Different types of arrows (or morphisms), concrete examples of limits and colimits before meeting the (or a) general definition, and exponentials.

    After an interlude into basic topos theory (which can be skipped), he introduces functors, natural transformations, the Yoneda lemma and representables, and finally adjunctions. I particularly appreciate the presentation of the Yoneda lemma, which is especially well-motivated: The first natural question is what natural transformations between hom-functors look like, and only after these does Smith consider what can be generalised.

    The writing is very clear, though I do think it is a bit light on examples; but this is to be expected since it has only minimal prerequisites. I don't think the absense of exercises is a huge detriment since every proof is basically an exercise. In the same vein, I do think the most profitable way to read the book (as with most mathematics textbooks, but especially in category theory) is to only glance at the provided proofs and attempt to reconstruct them.

    It is freely available on Smith's website [here](https://www.logicmatters.net/categories/).

3. Perrone, *Starting Category Theory*. A very nice new addition to the literature. Its coverage is a bit strange and should probably be supplemented with a book like Smith. Its main selling points are a great number of examples, and the slightly unorthodox inclusion of monads and monoidal categories in an introductory text.

4. Goldblatt, *Topoi: The Categorical Analysis of Logic*.

5. Leinster, *Basic Category Theory*. Ostesibly an introductory text, I think it would be difficult to follow without prior experience with category theory. But if you have read some of Smith's notes or Goldblatt's book, then it is a very nice book.

    Contrary to the above resources it is written with the mathematics (graduate) student in mind: examples are furnished by standard undergraduate algebra and topology in particular, though it is not necessary to understand every single example to get through the book. This also means that he expects a certain mathematical maturity from his readers, and thus he can be considerably more brisk in his presentation.

    For instance, while Smith only introduces natural transformations after more than 200 pages, Leinster already reaches this level of abstraction on page 27, immediately following a discussion on functors. The coverage of equivalence of categories is clear and well-motivated.

    Freely available [from arXiv](https://arxiv.org/abs/1612.09375).

6. Riehl, *Category Theory in Context*.
7. Fong, Spivak, *Seven Sketches in Compositionality*.


## Topology and geometry

### Point-set topology

Point-set (or 'general') topology is relatively self-contained as a discipline, but (for good reason!) it is usually taught after introductory real analysis. Parts of it also depend quite heavily on non-trivial set theory, but most introductory textbooks on topology cover the required amount of set theory quite nicely.

'Nice to know' stuff before learning topology includes some naïve set theory, analysis on Euclidean space, metric space topology, and maybe even a slight bit of category theory (though that is certainly not necessary).

General topology is significantly more abstract than metric space topology, so it may be advantageous to brush up on some of that. Good textbooks include:

1. Rudin, *Principles of Mathematical Analysis*. The classical textbook on introductory real analysis, has a nice chapter on metric space topology.

2. Apostol, *Mathematical Analysis*. Another classic analysis text. I personally prefer it to Rudin, but both cover the material nicely.

3. Folland, *Real Analysis*. Has a more cursory coverage of metric spaces, but the proofs are very nice.

4. Sutherland, *Introduction to Metric and Topological Spaces*. The first part is on metric spaces, and then he repeats himself in his coverage of topological spaces.

I won't say much more about metric spaces. Onto the main recommendations for point-set topology:

1. Munkres, *Topology*. A classic text that covers most of what you need to know. The first chapter in particular is a great introduction to naïve set theory (though why not go all out and read a book on [set theory](#logic), e.g. Goldrei's very approachable *Classic Set Theory*?). You won't go wrong with it, it is very easy to read (more so than the next couple of entries on this list), but it's not my first choice.

2. Engelking, *General Topology*. Some call it the 'Baby Rudin' of topology, it is particularly well-regarded for its wide coverage of topics. Also not my first choice, if nothing else then simply because Engelking follows Bourbaki's insistence that compact spaces must be Hausdorff. This is a conceptual annoyance, at least for me, since compactness makes perfect sense and is a useful axiom even without the Hausdorff property. But other than this it is a fine book.

3. Willard, *General Topology*. My favourite point-set topology book at this level. One demerit mark for the restrictive definition of local compactness, though this is a small complaint since most locally compact spaces are Hausdorff, in which case all the usual definitions of local compactness coincide.

    I especially like the coverage of weak/initial and strong/final topologies (though be aware of an error in Exercise 9H.3 as described [here](https://math.stackexchange.com/questions/2370532/can-a-set-be-homeomorphic-to-a-quotient-map-from-itself-making-sense-of-a-probl/)). It could benefit from a more explicit categorical approach; some of the arguments and much of the exposition could have been improved if Willard had been able to assume of his readers a passing familiarity with category theory. But if you know what products and coproducts are, you should be in good shape to fill in the gaps yourself.

    To make a couple of benefits of considering general weak topologies explicit: Both subspace topologies and product topologies are weak, the former induced by the inclusion map, the latter by the projections onto each factor. Hence we may e.g. prove a characterisation theorem for weak topologies in general and then specialise to each particular case. Another benefit is that this makes the connection between weak\*- and product topologies explicit.

    I'm not a fan of his coverage of nets, especially subnets. For that I prefer the treatment in [my own notes](https://github.com/dnhansen/topology-nets-filters) on the topic.

4. Lee, *Introduction to Topological Manifolds*. Could also have been called 'Introduction to Topology with Applications to Manifolds', since much of the book consists of a double course in point-set and algebraic topology.

    A very good supplement to Willard, it (not surprisingly) has a more geometric flavour, and especially quotient spaces are treated very nicely. If you know a thing or two about weak/strong topologies, for instance from Willard, you will also enjoy Lee's coverage of these topologies from a more structural perspective. Lee does not consider weak topologies in general, but you should have no trouble generalising his claims to general weak topologies. Every time he states a theorem on some particular weak topology, try to generalise it to an arbitrary weak topology. For instance, any product of Hausdorff spaces is Hausdorff. But any weak topology generated by maps into Hausdorff spaces is Hausdorff, at least if this collection of maps separates points in the given space.

    Categories are also not used in any substantial way in the discussion of point-set topology. Every time you see something that seems like it would benefit from the categorical view point, try to put things in categorical terms. For example, in problem 3-13 the reader is asked to show that if a continuous map *f* has a continuous left inverse, then *f* is a topological embedding. In fact, an arrow in **Top** is a topological embedding if and only if it is a regular monomorphism, i.e. if it is an equaliser. (This fact is quite natural, since equalisers in **Top** are subspaces.) So in particular a split monomorphism is an embedding.

    It also serves nicely as a self-contained introduction to point-set topology. However, analysts will find it lacking since it doesn't cover things like the product topology and Tychonoff's theorem, the Stone-Weierstrass theorem, and so on. For this there is e.g. Willard or Folland (see below).

    If you, like me, have tried and failed to learn algebraic topology from Hatcher, you will also be delighted that this is a book on algebraic topology that you can actually understand! In one sentence one might say that Lee has *respect* for point-set topology, something which Hatcher seemingly lacks. But more on algebraic topology [below](#algebraic-topology).

5. Folland, *Real Analysis*. Not a topology book, but the chapters on point-set topology and functional analysis contain a lot of nice topology with particular interest to analysts. As an example, take his self-contained (assuming some knowledge of Taylor series) proof of the Stone-Weierstrass theorem for compact spaces, as well as the analogous theorem for non-compact locally compact spaces using one-point compactification. And while the first part of the book focuses on measure and integration theory, this is not strictly necessary to read the above chapters.

6. Bradley, Bryson, Terilla, *Topology: A Categorical Approach*.

7. Naranong, 'Translating Between Nets and Filters' (archived [here](http://web.archive.org/web/20130308175220/http://www.math.tamu.edu/~saichu/netsfilters.pdf)). A nice exposition on the properties of nets and filters, using the (superior) definition of subnets following Aarnes and Andenaes. Be aware that the notes do contain some inaccuracies: for instance, the collection of tails of a net need not be nonempty if the domain of the net is empty, but a filterbase is required to be nonempty. Hence Definition 4.6 is slightly wrong. As far as I can tell we may repair this by simply requiring the domain of a net to be nonempty, for instance by requiring that directed sets be nonempty (following e.g. Kelley, but not Folland or Willard).

    There are also plenty of typos. Furthermore, many of the basic definitions work for general sets and not only topological spaces. There are no exercises, but most (all?) of the proofs are very easy once you have digested the concepts, so these may serve as exercises. Of course, any textbook covering nets (e.g. Folland, Willard) also contain exercises that may be of interest.

    I have also written [notes](https://github.com/dnhansen/topology-nets-filters) on nets and filters, which I obviously prefer.

### Algebraic topology

1. Lee, *Introduction to Topological Manifolds*. Contains first of all a very nice and standard introduction to the fundamental group. I particularly like Lee's very clear coverage of homotopy, especially the difference between free and relative homotopy, and why we need relative homotopy to make sense of path homotopy. For loops we might as well take the circle to be the domain of each path, and path homotopy of loops then amounts to *free* homotopy of the circle representatives of the loops in question.

    Lee also has a very nice *and understandable* chapter on cell complexes, in particular CW complexes and simplicial complexes. Since he has already covered quotients, disjoint unions and adjunction spaces, he can leverage this in his discussion of cell complexes upfront instead of sticking it in an appendix like some authors do... The upshot is that you walk away with more than just an intuitive understanding of complexes.

    While someone like Hatcher uses the language of manifolds sparingly (at least in the chapters on the fundamental group and homology), Lee has no trouble framing his results in this language. For example, he uses the Lebesgue number lemma (another plus) to show that any path in an at least two-dimensional manifold can be modified to avoid a given point. This is then used to calculate the fundamental group of spheres. The conceptual clarity that arises from his use of the Lebesgue number lemma and the language of manifolds is very helpful.

2. Rotman, *An Introduction to Algebraic Topology*.
3. tom Dieck, *Algebraic Topology*.

### Topological groups and vector spaces

1. McCarty, *Topology: An Introduction with Applications to Topological Groups*. As the title suggests, this is an introduction to topology with a special focus on topological groups. Each topic is first covered for general topological spaces and then specialised to topological groups, so I suppose it could serve as a general introduction to point-set (and a little bit of algebraic) topology, though I would prefer the books mentioned [above](#point-set-topology).

    There is both good and bad here. It is fairly elementary with good exercises, and it has good coverage of the elementary theory. The structure of the book is a bit odd, very few results are singled out as 'theorems', so it probably doesn't work very well as a reference. Some of the proofs are also a bit awkward, so one might instead use it as a guide to *results* of which the reader might themselves supply the *proofs*.

    If one is interested specifically in topological groups (and vector spaces), then I prefer [my own notes](https://github.com/dnhansen/topological-groups).

2. Folland, *A Course in Abstract Harmonic Analysis*. This is not a book on topological groups as such, but it might serve as a second reference for the very basic topology of groups.

3. Narici, Beckenstein, *Topological Vector Spaces*.

### Differential topology and geometry

1. Lee, *Introduction to Smooth Manifolds*.

### Riemannian geometry

1. Do Carmo, *Differential Geometry of Curves and Surfaces*. A bit fat 'stay away'! Some of my problems with the book:

    Do Carmo writes in a footnote: 'In italic context, letter symbols will not be italicized so they will be clearly distinguished from the surrounding text.' First of all, this is horrendous to read, and it is not exactly aesthetically pleasing. Secondly, he seemingly misses the point that we do not italicise letters to make them stand out, but for semantic reasons. A roman letter and and italic letter are semantically distinct; otherwise there would be no distinction between e.g. 'sin' (the sine function) and '*sin*' (the product of *s*, *i* and *n*). The second edition was completed in 2016, he does not get a free pass because the book is old. Furthermore, he apparently finds this practice odd himself, seeing as he found it necessary to remark on it all the way on page 138!

    Already in the first chapter does he abuse notation, for instance writing '*dβ*/*d*(-*s*)'. He also distinguishes between the derivatives *dα*/*dt* and *dα*/*ds*, the latter referring to the derivative with respect to arc length, without defining what this means. Ironically, in chapter 2 he admits to a *different* abuse of notation, apparently forgetting that he had been guilty of it from the start!

    But enough petty comments, here are a few things he just gets wrong:

    - He explicitly considers regular surfaces as subsets of **R**³ and only defines diffeomorphisms between surfaces, yet he claims that surfaces are locally diffeomorphic to (open subsets of) **R**².

    - After defining differentiability of maps between surfaces he apparently forgets that this is different from differentiability of maps between (open subsets of) Euclidean spaces. For instance, in Proposition 1 in Section 2-4 he considers a parametrisation **x**: *U* -> *S* of a surface *S* and a curve *α*: (–*ε*, *ε*) -> **x**(*U*). Now *α* is differentiable as a map between Euclidean spaces, but **x⁻¹** is differentiable as a function on a surface, so the composition is not obviously differentiable. However, this is exactly what he claims, apparently not noticing that this is not trivial.

        The solution is to solve Exercise 13 (which is starred!) of section 2-3, but he never refers to this exercise. In fact, in a footnote on page 82 he encourages one to skip this exercise if one has skipped the proofs in section 2-3. And this he claims could be done on a first reading, but *not so* for section 2-4.

        When taking undergraduate differential geometry using Do Carmo's book, I asked my TA (who was a PhD student in geometry) how this worked, and he simply remarked that the composition above being differentiable was obvious. In fact, even the lecturer got it wrong! But in a different way, by claiming that the differential of **x**⁻¹ is the inverse of the differential of **x** *as a map between Euclidean spaces*.
    
    I could go on. I have no idea why people like the book so much. Furthermore, I do not see the use in doing differential geometry only on submanifolds of Euclidean spaces. One has to learn about abstract manifolds at some point, might as well do so from the beginning.

2. Lee, *Introduction to Riemannian Manifolds*.
3. O'Neill, *Semi-Riemannian Geometry: With Applications to Relativity*.
4. Petersen, *Riemannian Geometry*.


## Mathematical physics

1. Hall, *Quantum Mechanics for Mathematicians*.
2. Moretti, *Fundamental Mathematical Structures of Quantum Mechanics*.
3. Reed, Simon, *Methods of Modern Mathematical Physics*.
4. Abraham, Marsden, *Foundations of Mechanics*.
5. Arnold, *Mathematical Methods of Classical Mechanics*.


## Order theory

1. Davey, Priestley, *Introduction to Lattices and Order*. A very good elementary introduction to order and lattice theory. Assumes basically nothing from the reader and goes quite slowly through the material. From a strictly mathematical point of view, I don't find order or lattice theory particularly interesting, but they are very useful at clarifying conceptual issues. Highlights of this nature in my reading so far are:

    - The Knaster-Tarski fixpoint theorem is used to prove Banach's decomposition theorem, and this in turn gives an easy proof of the Schröder-Bernstein theorem. (Cf. Theorem 2.35 and Exercise 2.32.)
    
    - The authors make a throwaway comment that the extent and intent of a concept appear asymmetrically in the definition of the ordering on the set of concepts of a given context, and that this asymmetry is 'illusory'. In fact, the extent and intent do not appear asymmetrically, but rather *antisymmetrically*. This distinction between asymmetry and antisymmetry is of course an important one, I suppose culminating in the idea of contravariant functors. (Cf. §3.2.)

    - It is well-known that many types of structures are preserved under intersection but not union: For instance, any intersection of subgroups is a subgroup, but a union of subgroups is usually not a subgroup. However, a union of an *increasing sequence* of subgroups is a subgroup. In other words, the union of a *chain* of subgroups is a subgroup. The authors note that it suffices that a collection of subgroups is *directed* for its union to be a subgroup. (Cf. Definition 7.10 and the following discussion.)

        I am reminded of the fact from topology that the union of a finite collection of closed sets is closed, but it actually suffices that the collection is *locally* finite (cf. e.g. Lee's *Introduction to Topological Manifolds*, Lemma 4.75).
    
    - The book is also an excellent introduction to fixpoint theory, though note that their CPO Fixpoint Theorem III (proved in Exercise 8.20) contains an error, in that the function $F$ does not need to have a *minimal* fixpoint.

2. Fong, Spivak, *Seven Sketches in Compositionality*.

## Logic

The definitive guide to self-studying formal logic for both mathematicians and philosophers is certainly Peter Smith's [*Beginning Mathematical Logic: A Study Guide*](https://www.logicmatters.net/tyl/), and most of the resources below are found therein. However, I disagree somewhat with some of Smith's advice, so below I outline a slightly different path through the material.

### Propositional and first-order logic

When beginning one's study of formal logic, the first thing one should do is obtain some familiarity with central notions such as the distinction between syntax, semantics and proof systems. This includes the distinction between the formal languages that we study in formal logic, and the metalanguage (here some augmented version of English) we use to study those formal languages. The best place to start, in my opinion, is

1. Smith, *An Introduction to Formal Logic*. I will comment on the first edition, since this is the one I have read. Smith starts by spending 50 pages on *informal* logic, slowly introducing the reader to the central concepts of logical inference. He then develops first propositional logic without conditionals, introduces conditionals, and then moves on to first-order logic. The deductive system employed for both propositional and first-order logic is that of logical tableaux (the second edition has been rewritten to use natural deduction), and he eventually proves, in an admittedly very informal fashion, both soundness and completeness of his deductive system for first-order logic.

    The writing is clear, and Smith is, as usual, very sensitive to more conceptual or philosophical issues, and highlights these when they occur.

    One doesn't need to study this book very closely. Most of the material will be repeated in some form or another in the recommendations below, but do take note of the more philosophical or conceptual asides. Those are always worth coming back to.

Next, Smith recommends Chiswell and Hodges' *Mathematical Logic*, and this is certainly a good book, but after reading the introduction above my sense is that it is just too slow. C&H's proof system of choice is natural deduction, so if one has read the second edition of Smith's own introduction, then one is already familiar with the general ideas and probably don't need a repeat. Instead, I recommend moving straight onto Smith's next recommendation:

2. Leary, Kristiansen, *A Friendly Introduction to Mathematical Logic*. Instead of starting with propositional logic and building up to first-order logic, L&K introduce their version of first-order logic from the get-go. A version of propositional logic features in their proof system (essentially allowing one to 'ignore' quantifiers and make deductions that would be valid in a propositional logic), but one doesn't have to slog through another long exposition.

    L&K use a Hilbert-style axiomatic system as their proof system. This has the disadvantage of being less natural than natural deduction (which I guess is quite natural), but it has the major advantage that it is very easy to reason about.

    At this point, one could begin by reading through §3.2 on completeness, as well as Theorem 3.3.1 and Corollary 3.3.2 from §3.3. The material in the rest of chapter 3 will be covered in the readings on model theory below, and they are not important at this stage. However, jumping ahead and reading §4.1 could be very useful in fixing some ideas about axiomatisation before moving on to Gödel's theorems and computability theory.

    Also see [my notes](https://github.com/dnhansen/leary-kristiansen-logic) on L&K.

At this point the groundwork has been laid, and there are multiple different directions one could go in: The most important are set theory, computability theory, and model theory. Mathematicians should cope readily with the technical aspects of set theory, though they may struggle slightly with the more philosophical or conceptual parts (unless they have been brought up right). Computability theory is of central importance in computer science, and we also collect the more CS-oriented recommendations here. Finally, model theory is probably the most technically (if not conceptually) difficult of the three.


### Second-order logic

At this point I believe it is useful to study briefly second-order logic. First of all to contrast this with first-order logic in order to better see what makes FOL special, and secondly because for mathematicians second-order logic is very natural, and one might even argue that it is more natural than FOL.

1. Shapiro, 'Higher-order Logic', in Shapiro, ed., *The Oxford Handbook of the Philosophy of Mathematics and Logic*.
2. Button, Walsh, *Philosophy and Model Theory*, chapter 1.


### Set theory

Mathematicians should have a good understanding of naïve set theory.

1. Moschovakis, *Notes on Set Theory*. A very conceptually sound introduction. Moschovakis (rightly, in my view) studies not *formal* set theory but rather *axiomatic* set theory. That is, he studies those properties of sets that are captured by the axioms, he doesn't study the properties of a formalisation of set theory. This means that he can unproblematically talk about the empty set, or the union of two sets, and so on. This is not the case in the study of *formal* set theory, in which one cannot even refer to the empty set since the only terms in the language are variables.

    For things like recursion and lattice theory, see also [my CS bachelor project](https://github.com/dnhansen/cs-bachelor-project).

2. Goldrei, *Classic Set Theory*.
3. Potter, *Set Theory and Its Philosophy*.

### Computability theory

1. Chiswell, *A Course in Formal Languages, Automata and Groups*. For mathematicians a great introduction to grammars, the Chomsky hierarchy, and automata. The final chapter is on applications to group theory, e.g. the word problem. Chiswell takes a grammars-first approach, and only later proves that different classes of languages are accepted by certain classes of automata, or that the regular languages constitute the smallest rationally closed (i.e., which contains the finite languages, and which is closed under the Kleene star operation, unions and concatenation).
   
   The book is naturally light on applications, but these can readily be learnt from the computer science literature, which can now be perused very easily since the foundations have been laid.

   If one is not interested in applications to group theory, the final chapter can easily be skipped (or saved for another day).

2. Kozen, *Automata and Computability*. Written as a series of somewhat mutually independent lectures, much of the material is familiar to anyone having studied CS-oriented computability theory. If one has already read Chiswell (or learnt the material elsewhere), of particular interest are the following sections:

    - Lectures 7-9 and supplementary lecture A on regular expressions, pattern matching and Kleene algebras.
    - Lecture 10 on homomorphisms, with applications to regular languages.
    - Lecture 12 on applications of the pumping lemma for regular languages (in case one is interested in seeing more examples).
    - Lectures 13-16 (in particular 14) and supplementary lecture B on minimisation of finite automata.
    - [TODO C,D]
    - Lecture 26 on parsing.
    - Lecture 27 on the CKY algorithm.
    - Supplementary lecture G on the Chomsky-Schützenberger theorem, which characterises the context-free languages as the homomorphic images of intersections of regular languages and certain 'parenthesis languages' (also called Dyck languages).
    - Supplementary lecture H on Parikh's theorem, whose statement is more technical.

    The final part of the book concerns Turing machines, but they will be covered in greater detail in the recommendations below.

3. Smith, *An Introduction to Gödel's Theorems*.

4. Cooper, *Computability Theory*.

### Model theory

3. Goldrei, *Propositional and Predicate Calculus*.
4. Manzano, *Model Theory*.


## Linguistics

Linguistics is of course not mathematics! I should probably rename this list...

1. Fromkin, Rodman, Hyams, *An Introduction to Language*.
2. Fromkin, ed., *Linguistics: An Introduction to Linguistic Theory*.
3. Comrie, *Aspect*.
4. Comrie, *Tense*.
5. Dahl, *Tense and Aspect Systems*.
6. Palmer, *Mood and Modality*.
7. Blake, *Case*.


## Philosophy

Philosophy isn't mathematics either.

1. Benson, ed., *A Companion to Plato*.
   - Dancy, 'Platonic Definitions and Forms'.
   - Ferejohn, 'Knowledge and the Forms in Plato'.
   - Miller, 'The Platonic Soul'.
   - Kahn, 'Plato on Recollection'.
   - Gill, 'Problems for Forms'.
2. Meinwald, *Plato*.
3. Shields, *Aristotle*.
4.  Beebee, *Hume on Causation*.
5.  Millican, introduction to David Hume's *Enquiry concerning Human Understanding* (Oxford World Classics).
6.  Audi, *Epistemology*.
7.  Loux, Crisp, *Metaphysics*.
8.  Miller, *Philosophy of Language*.
9.  Kim, *Philosophy of Mind*.
10. Ladyman, *Understanding Philosophy of Science*.
11. Kagan, *Normative Ethics*.
12. Fisher, *Metaethics*.
13. George, Velleman, *Philosophies of Mathematics*.
14. Shapiro, *Thinking about Mathematics*.
15. Psillos, *Causation and Explanation*.
16. Melia, *Modality*.
17. Brock, Mares, *Realism and Anti-Realism*.
18. Mares, *A Priori*.
19. Ladyman, Ross, *Every Thing Must Go*.


## Physics

### Quantum mechanics

1. Griffiths, *Introduction to Quantum Mechanics*. Obviously a popular introductory text, and I do think it's one of the best ones out there. That doesn't say much since the literature is rather lacking. Let me highlight some of the obvious flaws of the book.

    The author claims that a wave function (in one dimension) must go to zero as $x$ goes to plus or minus infinity, otherwise it "would not be normalizable" (2nd ed., p. 14). By this he means $L^2$ (p. 13). But as any sophomore mathematics student fresh out their first measure theory course can tell you, this is emphatically wrong. It is easy to find counterexamples that are discontinuous on a countable nowhere dense subset of $\mathbb{R}$, and it is only slightly harder to find counterexamples that are *smooth*. In a footnote (p. 14) Griffiths claims that counterexamples to this claim are "pathological" and that "for us the wave function *always* goes to zero at infinity". (Only in physics could *smooth* functions be pathological... I suppose anything that is not analytic is the work of the devil?) The author also spends no effort explaining to the reader why in the world we should expect (and even postulate!) wave functions to vanish at infinity.
    
    In any case, if the problem with functions not going to zero at infinity is that they are so-called "pathological", then why claim that they are not $L^2$, only to retract this claim in a footnote? There are many functions that do and no not have this property, many of whom are $L^2$ and many of whom are not. It simply has nothing to do with them being $L^2$. Even a physicist should be able to see that. Evidently the author does as well, though he apparently also thinks that it would take a "good" mathematician to come up with counterexamples...

    Another conceptually quite egregious flaw is the front-loading of the Schrödinger equation. This is introduced on page 1 with no explanation. No hint at how to think about it, no history, nothing. This is followed by a bunch of uninspiring, actually quite difficult for this level, calculations that tell you precisely nothing about quantum mechanics.

    Maybe even worse, the word "vector" appears for the first time in the book *on page 93* in a chapter so uninspiringly called "Formalism". Of course it is impossible to grasp quantum mechanics without a solid understanding of linear algebra, so why wait almost a hundred pages before introducing it?

    Thankfully (or miraculously?) the second half of the book, titled "Applications", is actually quite good. It contains probably the best exposition of perturbation theory I have seen at this level.

2. Schumacher, Westmoreland, *Quantum Processes, Systems, and Information*. A joint introduction to quantum mechanics and quantum information theory. Probably my favourite introduction to quantum mechanics (for physicists at least!). Westmoreland is a mathematician, so even if the book is far from rigorous -- and it certainly shouldn't be as an introductory book aimed at physicists -- it is written quite carefully.

    The book starts very elementary, discussing bits and qubits, distinguishability and information, and linear algebra upfront. Unitary dynamics and the Schrödinger equation are only introduced after more than 100 pages.

    They are also remarkably careful when discussing questions of dimensionality of vector spaces: they don't enter into a thorough discussion of these matters, but even acknowledging that there are thorny mathematical issues puts the book above many other introductory textbooks.

    One thing to keep in mind, as with most physics books, is that vector spaces are assumed finite-dimensional when this is useful. For instance, the otherwise obscure notion of time-dependence of operators becomes trivial if the operator is just a matrix. But I wish this had been made more explicit, since we surely do *not* wish to interpret operators as matrices. (Of course, all norms on a finite-dimensional vector space are equivalent so this is not necessary. But this fact is certainly not trivial, so it would seem unreasonable to assume this kind of knowledge of the reader.)


## Computer science

### Algorithms and data structures

1. Cormen, Leiserson, Rivest, Stein, *Introduction to Algorithms*.
2. Kleinberg, Tardos, *Algorithm Design*.
3. Okasaki, *Purely Functional Data Structures*.


### Computer architecture

1. Tanenbaum, Austin, *Structured Computer Organization*. A classic, covering Tanenbaum's Mic microarchitecture and IJVM. Some of this book is very good, but then some of it is borderline unreadable. Obviously the many chapters on concrete architectures or other technologies are only of interest to practitioners. Apart from this, chapters 1 and 3-5 are quite good.

    Chapter 3 covers the basics of digital logic (though I prefer Mano and Ciletti's coverage, see below), focusing on the types of circuits that are of interest in computer architecture. Most of this is perfectly fine.

    Chapter 4 then covers the Mic microarchitecture, a very simple processor that is supposed to implement IJVM, which is a subset of the JVM instruction set only containing integer instructions. And it is indeed simple and very useful as a reference microarchitecture, though the exposition could be (much) better. For instance, the authors discuss issues of timing at least three times, when it really should be enough to cover this once. Furthermore, the explanation of branching is also rather hard to follow.

    Chapter 5 covers general instruction sets, and this discussion is fairly good.

    The IJVM instruction set is strange in that its virtual machine is stack-based, in contrast with e.g. the x86 or ARM instruction sets. In particular, none of the registers of the Mic are visible at the ISA level, so one gets basically no experience with proper assembly programming by programming in IJVM. Hence it is most useful as a conceptual model, as an example of how one might implement a fairly high level assembly language in a concrete microarchitecture.

    While the introduction of chapter 6 helps one place operating systems in the machine hierarchy, this is followed by a more or less incomprehensible discussion of virtual memory. For (much) better introductions to virtual memory, see the recommendations [below](#operating-systems).

    The introduction of chapter 7 on assembly is similarly useful, especially since the relationship between the ISA, OS and assembly levels can be hard to understand. The rest of this chapter seems like a bunch of fluff, to be honest.

2. Comer, *Essentials of Computer Architecture*.
3. Mano, Ciletti, *Digital Design: With an Introduction to the Verilog HDL, VHDL, and SystemVerilog*.


### Operating systems

1. Arpaci-Dusseau, Arpaci-Dusseau, *Operating Systems: Three Easy Pieces*. Also known as simply "OSTEP".
2. Hailperin, *Operating Systems and Middleware*.


### Haskell

1. Allen, Moronuki, *Haskell Programming from First Principles*.
2. Bird, *Thinking Functionally with Haskell*.
3. Bird, Gibbons, *Algorithm Design with Haskell*.
4. Hutton, *Programming in Haskell*.