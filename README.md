# Mathematics resources

This is an attempt to collect notes on mathematics resources I have used and continue to use. It is not meant to be authoritative or exhaustive, but perhaps someone might benefit from my thoughts on the resources below.

The list is (clearly) far from complete. I will add to it whenever I feel like it!

## Contents

- [Analysis](#analysis)
  - [Introductory real analysis](#introductory-real-analysis)
  - [Complex analysis](#complex-analysis)
  - [Measure theory and probability theory](#measure-theory-and-probability-theory)
  - [Functional and harmonic analysis](#functional-and-harmonic-analysis)
- [Algebra](#algebra)
- [Topology and geometry](#topology-and-geometry)
  - [Point-set topology](#point-set-topology)
  - [Algebraic topology](#algebraic-topology)
  - [Differential topology](#differential-topology)
  - [Riemannian geometry](#riemannian-geometry)

## Analysis

### Introductory real analysis

### Complex analysis

1. Rao, Stetkær, Fournais, Møller, *Complex Analysis: An Invitation*.
2. Ullrich, *Complex Made Simple*.


### Measure theory and probability theory

1. Bauer, *Measure and Integration Theory*.
2. Bauer, *Probability Theory*.
3. Cohn, *Measure Theory*.
4. Folland, *Real Analysis*.
5. Billingsley, *Convergence of Probability Measures*.

### Functional and harmonic analysis

1. Folland, *Real Analysis*.
1. Rudin, *Functional Analysis*.
3. Conway, *A Course in Functional Analysis*.
4. Folland, *Abstract Harmonic Analysis*.
5. Helemskii, *Lectures and Exercises on Functional Analysis*.

## Algebra

1. Aluffi, *Algebra: Chapter 0*.

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

    If you, like me, have tried and failed to learn algebraic topology from Hatcher, you will also be delighted that this is a book on algebraic topology that you can actually understand!

5. Folland, *Real Analysis*. Not a topology book, but the chapters on point-set topology and functional analysis contain a lot of nice topology with particular interest to analysts. As an example, take his self-contained (assuming some knowledge of Taylor series) proof of the Stone-Weierstrass theorem for compact spaces, as well as the analogous theorem for non-compact locally compact spaces using one-point compactification. And while the first part of the book focuses on measure and integration theory, this is not strictly necessary to read the above chapters.

6. Bradley, Bryson, Terilla, *Topology: A Categorical Approach*.

### Algebraic topology

1. Rotman, *An Introduction to Algebraic Topology*.
2. tom Dieck, *Algebraic Topology*.

### Differential topology and geometry

1. Lee, *Introduction to Smooth Manifolds*.

### Riemannian geometry

1. Lee, *Introduction to Riemannian Manifolds*.
2. O'Neill, *Semi-Riemannian Geometry: With Applications to Relativity*.
3. Petersen, *Riemannian Geometry*.