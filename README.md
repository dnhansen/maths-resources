# maths-resources

This is an attempt to collect notes on mathematics resources I have used and continue to use. It is not meant to be authoritative or exhaustive, but perhaps someone might benefit from my thoughts on the resources below.

## Analysis

## Algebra

## Topology

Point-set (or 'general') topology is relatively self-contained as a discipline, but (for good reason!) it is usually taught after introductory real analysis. Parts of it also depend quite heavily on non-trivial set theory, but most introductory textbooks on topology cover the required amount of set theory quite nicely.

'Nice to know' stuff before learning topology includes some naïve set theory, analysis on Euclidean space, metric space topology, and maybe even a slight bit of category theory (though that is certainly not necessary).

General topology is significantly more abstract than metric space topology, so it may be advantageous to brush up on some of that. Good textbooks include:

1. Rudin, *Principles of Mathematical Analysis*. The classical textbook on introductory real analysis, has a nice chapter on metric space topology.

2. Apostol, *Mathematical Analysis*. Another classic analysis text. I personally prefer it to Rudin, but both cover the material nicely.

3. Folland, *Real Analysis*. Has a more cursory coverage of metric spaces, but the proofs are very nice.

4. Sutherland, *Introduction to Metric and Topological Spaces*. The first part is on metric spaces, and then he repeats himself in his coverage of topological spaces.

Intermediate paragraph for testing.

5. Continuing markdown list numbering test.

I won't say much more about metric spaces. Onto the main recommendations for point-set topology:

1. Munkres, *Topology*. A classic test that covers most of what you need to know. It is a standard undergraduate textbook, so I won't say much about it. You won't go wrong with it, it is very easy to read (more so than the next couple of entries on this list), but it's not my first choice.
2. Engelking, *General Topology*. The 'Baby Rudin' of topology. Also not my first choice, if nothing else then simply because Engelking follows Bourbaki's insistence that compact spaces must be Hausdorff. This is a conceptual annoyance, at least for me, since compactness makes perfect sense and is a useful axiom even without the Hausdorff property. But other than this it is a fine book.
3. Willard, *General Topology*. My favourite point-set topology book at this level. One demerit mark for the restrictive definition of local compactness, though this is a small complaint since most locally compact spaces are Hausdorff, in which case all the usual definitions of local compactness coincide.

    I especially like the coverage of weak/initial and strong/final topologies (though be aware of an error in Exercise 9H.3 as described [here](https://math.stackexchange.com/questions/2370532/can-a-set-be-homeomorphic-to-a-quotient-map-from-itself-making-sense-of-a-probl/)). It could benefit from a more explicit categorical approach; some of the arguments and much of the exposition could have been improved if Willard had been able to assume of his readers a passing familiary with category theory. But if you know what products and coproducts are, you should be in good shape to fill in the gaps yourself.

    To make a couple of benefits of weak topologies explicit: Both subspace topologies and product topologies are weak, the former induced by the inclusion map, the latter by the projections onto each factor. Hence we may e.g. prove a characterisation theorem for weak topologies in general and then specialise to each particular case. Another benefit is that this makes the connection between weak\*- and product topologies explicit.

4. Lee, *Introduction to Topological Manifolds*. Could also have been called 'Introduction to Topology with Applications to Manifolds', since much of the book consists of a double course in point-set and algebraic topology.

    A very good supplement to Willard, it (not surprisingly) has a more geometric flavour, and especially quotient spaces are treated very nicely. If you know a thing or two about weak/strong topologies, for instance from Willard, you will also enjoy Lee's coverage of these topologies from a more structural perspective. Lee does not consider weak topologies in general, but you should have no trouble generalising his claims to general weak topologies.

    If you, like me, have tried to learn algebraic topology from Hatcher and failed, you will also be delighted that this is a book on algebraic topology that you can actually understand!

5. Folland, *Real Analysis*. Not a topology book, but the chapters on point-set topology and functional analysis contain a lot of nice topology with particular interest to analysts. And while the first part of the book focuses on measure and integration theory, this is not strictly necessary to read the above chapters.