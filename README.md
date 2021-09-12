# Mathematics resources

This is an attempt to collect notes on mathematics resources I have used and continue to use. It is not meant to be authoritative or exhaustive, but perhaps someone might benefit from my thoughts on the resources below.

The entries in each main section are listed roughly in 'recommended reading order', insofar as I recommend each resource! Unless otherwise stated, you can assume that I have in fact found each entry worthy of recommendation.

The list is (clearly) far from complete. I will add to it whenever I feel like it!

## Contents

- [Analysis](#analysis)
    - [Introductory real analysis](#introductory-real-analysis)
    - [Complex analysis](#complex-analysis)
    - [Measure and integration theory](#measure-and-integration-theory)
    - [Probability theory](#probability-theory)
    - [Functional and harmonic analysis](#functional-and-harmonic-analysis)
- [Algebra](#algebra)
    - [Linear algebra](#linear-algebra)
    - [Abstract algebra](#abstract-algebra)
    - [Category theory](#category-theory)
- [Topology and geometry](#topology-and-geometry)
    - [Point-set topology](#point-set-topology)
    - [Algebraic topology](#algebraic-topology)
    - [Differential topology](#differential-topology-and-geometry)
    - [Riemannian geometry](#riemannian-geometry)
- [Mathematical physics](#mathematical-physics)

## Analysis

### Introductory real analysis

By this I mean basically everything that does not require measure theory, and which doesn't fall under more specific headings such as differential equations.

The first order of business is to become familiar with the theory of continuous functions between Euclidean spaces, or better yet metric spaces. This required some knowledge of the topology of the spaces in question, and the books below should cover the necessary material.

Next, on to differentiation and integration, which can be done in varying levels of generality. I personally like the Riemann-Stieltjes integral (see Rudin or especially Apostol below) since it provides an obvious but useful generalisation of the ordinary Riemann (or Darboux) integral, and serves as a first step towards things like like integrals.

Finally, multidimensional analysis, in particular differentiation of functions between general Euclidean spaces (or maybe even infinite-dimensional spaces!), and integration of them as well. The theory of differentiation is very important, but I feel like it is perfectly possible to do without much knowledge of multidimensional Riemann integrals. The Lebesgue integral is just so much nicer, and you will want to become intimately familiar with it down the line anyway.

1. Rudin, *Principles of Mathematical Analysis*. The classic. It is a bit light on content, and certainly the later chapters should be avoided: the material on differential forms and the Lebesgue integral is better found elsewhere.

    Things I especially like: The coverage of the exponential function, first in an 'early transcendentals' fashion, defining it first for integer, then rational and finally real exponents, and later reconciling this with the 'late transcendentals' definitions in terms of integrals and power series. The introduction of perfect sets is also interesting and yields a topological proof of the uncountability of the reals.


2. Apostol, *Mathematical Analysis*. Another classic, often compared to Rudin's book. I tend to prefer Apostol's treatment of the basic material, it is more complete and less terse, but they complement each other well.

    Things to like: An excellent coverage of metric space topology, though with a different focus than Rudin. It also treats Riemann-Stieltjes integrals in great generality, and contains basically everything you could ever want to know about Riemann integration.

3. Duistermaat, Kolk, *Multivariate Real Analysis*. Assumes knowledge of one-dimensional analysis as covered in one of the books above. Covers multidimensional differential and integral calculus in a very modern fashion, especially the former, and also gets into some basic theory of manifolds (though only submanifolds of Euclidean space). It also covers the antidifferentiation problem in higher dimension, though in a rather unsatisfying fashion by only considering (not even piecewise) continuously differentiable curves and differentiable homotopies. But what it does it does do well.

    The best part of the book is the very large number of excellent exercises! For instance, a sequence of exercises guides the reader through a derivation of (versions of) the Helmholtz-Weyl and Hodge decompositions, Maxwell's equations in covariant form, invariance of the wave equation under Lorentz transformations, and much more. All without assuming, as geometers are want to do, that every manifold and every vector field under the sun is smooth!

4. Zorich, *Mathematical Analysis*.

### Complex analysis

1. Rao, Stetkær, Fournais, Møller, *Complex Analysis: An Invitation*.
2. Ullrich, *Complex Made Simple*.


### Measure and integration theory

I initially learnt measure theory from Steen Thorbjørnsen's *Grundlæggende mål- og integralteori*, so I don't know how good the books below are for beginners. (Thorbjørnsen's book is excellent as an introduction. It is very clearly written with great exercises, and the only prerequisite is first-year analysis and linear algebra.)

1. Bauer, *Measure and Integration Theory*. I haven't read most of this book, but it seems like a perfectly respectable first introduction to measure theory. If the 'sequel' *Probability Theory* (see [below](#probability-theory)) is any indication, this book is certain to be clear and well-motivated.

    The parts that I *have* read are, first of all: The sections on product measures and convolutions of measures. Both of these are excellent, and the latter in particular is a great way to pick up the results about convolutions needed in probability theory. And secondly the section on convergence of Radon measures, in which Bauer introduces vague and weak convergence of measures, both of which are of central importance in probability theory.

2. Cohn, *Measure Theory*. As with Bauer above I haven't read much of this book, but it seems a quite popular introduction to the subject. The chapter on Polish spaces is particularly nice.

3. Folland, *Real Analysis*. Perhaps not the best *introduction* to measure and integration theory, but it is great as a second book on the subject. Of particular interest are the following sections:

    - Outer measures and Borel measures on the real line
    - Modes of convergence and the *n*-dimensional Lebesgue integral
    - The chapter on signed measures (skip the last couple of sections if you feel like it)
    - The chapters on point-set topology and functional analysis (see also [below](#point-set-topology))
    - The first couple of sections on *L^p*-spaces
    - The chapter on Radon measures (you can skip the last section)
    - The chapters on Fourier analysis and distributions

    Some issues I have with the book: Folland doesn't assume any knowledge of topological spaces, so many theorems in the first half of the book are stated for metric spaces even though they generalise immediately. Some of the proofs are also less than clear for this reason. A few theorems are also proven in less than full generality, even though they would be no less difficult to state or prove more generally. So keep your eye out, and if it seems like something can be generalised, it probably can.


### Probability theory

1. Bauer, *Probability Theory*.

2. Billingsley, *Convergence of Probability Measures*.

3. Kallenberg, *Foundations of Modern Probability*. A massive tome which I can't claim to have read. From perusing it it does seem a bit terse and perhaps not great to learn from. One specific issue I have with it is Kallenberg's focus on *second-countable* locally compact Hausdorff spaces, which is just not necessary for e.g. the Riesz representation theorem.

### Functional and harmonic analysis

1. Folland, *Real Analysis*.
1. Rudin, *Functional Analysis*.
3. Conway, *A Course in Functional Analysis*.
4. Folland, *A Course in Abstract Harmonic Analysis*.
5. Helemskii, *Lectures and Exercises on Functional Analysis*.

## Algebra

### Linear algebra

1. Hoffman, Kunze, *Linear Algebra*.
2. Roman, *Advanced Linear Algebra*.

### Abstract algebra

1. Aluffi, *Algebra: Chapter 0*.

### Category theory

1. Awodey, *Category Theory*. This one carries a big fat 'do not recommend'! At least for beginners. A lot of people seem to like it, and I don't get it. It's sloppy, imprecise and difficult to follow compared to so many other books on category theory.

    For instance, in section 1.4 he introduces the category **Cat** of all categories and functors, but in section 1.8 he apparently retracts this definition and lets **Cat** denote the category of *small* categories. Nevertheless he, for instance in exercise 2 of the first chapter, still wants to talk about isomorphisms of *large* categories despite not having defined what this means.
    
    For another example, in section 2.8 he introduces hom-functors and calls them *the* representable functors. In exercise 18 of the same chapter he asks the reader to show that the forgetful functor from monoids to sets is representable. But what is that supposed to mean? He only introduces natural transformations in chapter 7! See also [this](https://math.stackexchange.com/questions/3299671/why-is-the-forgetful-functor-representable) discussion on StackExchange.

    To its credit, the book does contain a lot of material of particular interest to computer scientists and logicians. But I don't understand why people use it as an introductory text.

2. Leinster, *Basic Category Theory*.
3. Riehl, *Category Theory in Context*.


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

1. Munkres, *Topology*. A classic test that covers most of what you need to know. The first chapter in particular is a great introduction to naïve set theory. You won't go wrong with it, it is very easy to read (more so than the next couple of entries on this list), but it's not my first choice.

2. Engelking, *General Topology*. Some call it the 'Baby Rudin' of topology, it is particularly well-regarded for its wide coverage of topics. Also not my first choice, if nothing else then simply because Engelking follows Bourbaki's insistence that compact spaces must be Hausdorff. This is a conceptual annoyance, at least for me, since compactness makes perfect sense and is a useful axiom even without the Hausdorff property. But other than this it is a fine book.

3. Willard, *General Topology*. My favourite point-set topology book at this level. One demerit mark for the restrictive definition of local compactness, though this is a small complaint since most locally compact spaces are Hausdorff, in which case all the usual definitions of local compactness coincide.

    I especially like the coverage of weak/initial and strong/final topologies (though be aware of an error in Exercise 9H.3 as described [here](https://math.stackexchange.com/questions/2370532/can-a-set-be-homeomorphic-to-a-quotient-map-from-itself-making-sense-of-a-probl/)). It could benefit from a more explicit categorical approach; some of the arguments and much of the exposition could have been improved if Willard had been able to assume of his readers a passing familiarity with category theory. But if you know what products and coproducts are, you should be in good shape to fill in the gaps yourself.

    To make a couple of benefits of considering general weak topologies explicit: Both subspace topologies and product topologies are weak, the former induced by the inclusion map, the latter by the projections onto each factor. Hence we may e.g. prove a characterisation theorem for weak topologies in general and then specialise to each particular case. Another benefit is that this makes the connection between weak\*- and product topologies explicit.

4. Lee, *Introduction to Topological Manifolds*. Could also have been called 'Introduction to Topology with Applications to Manifolds', since much of the book consists of a double course in point-set and algebraic topology.

    A very good supplement to Willard, it (not surprisingly) has a more geometric flavour, and especially quotient spaces are treated very nicely. If you know a thing or two about weak/strong topologies, for instance from Willard, you will also enjoy Lee's coverage of these topologies from a more structural perspective. Lee does not consider weak topologies in general, but you should have no trouble generalising his claims to general weak topologies. Every time he states a theorem on some particular weak topology, try to generalise it to an arbitrary weak topology. For instance, any product of Hausdorff spaces is Hausdorff. But any weak topology generated by maps into Hausdorff spaces is Hausdorff, at least if this collection of maps separates points in the given space.

    If you, like me, have tried and failed to learn algebraic topology from Hatcher, you will also be delighted that this is a book on algebraic topology that you can actually understand! But more on algebraic topology [below](#algebraic-topology).

5. Folland, *Real Analysis*. Not a topology book, but the chapters on point-set topology and functional analysis contain a lot of nice topology with particular interest to analysts. As an example, take his self-contained (assuming some knowledge of Taylor series) proof of the Stone-Weierstrass theorem for compact spaces, as well as the analogous theorem for non-compact locally compact spaces using one-point compactification. And while the first part of the book focuses on measure and integration theory, this is not strictly necessary to read the above chapters.

6. Bradley, Bryson, Terilla, *Topology: A Categorical Approach*.

### Algebraic topology

1. Lee, *Introduction to Topological Manifolds*.
2. Rotman, *An Introduction to Algebraic Topology*.
3. tom Dieck, *Algebraic Topology*.

### Differential topology and geometry

1. Lee, *Introduction to Smooth Manifolds*.

### Riemannian geometry

1. Do Carmo, *Differential Geometry of Curves and Surfaces*. I'll get back to the details on this one, but until then: Do not recommend!
2. Lee, *Introduction to Riemannian Manifolds*.
3. O'Neill, *Semi-Riemannian Geometry: With Applications to Relativity*.
4. Petersen, *Riemannian Geometry*.


## Mathematical physics

1. Hall, *Quantum Mechanics for Mathematicians*.
2. Moretti, *Fundamental Mathematical Structures of Quantum Mechanics*.
3. Reed, Simon, *Methods of Modern Mathematical Physics*.
4. Abraham, Marsden, *Foundations of Mechanics*.
5. Arnold, *Mathematical Methods of Classical Mechanics*.