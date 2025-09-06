---
title: "The Nested-Drift Algorithm"
collection: publications
category: wp
permalink: /publication/Nested
excerpt: <p style="font-size:0.85rem;">with <a href="https://www.patrickmschneider.com/">Patrick Schneider</a></p><p style="font-size:0.85rem;">Efficient and robust method of implementing finite difference algorithms for solving heterogeneous agent models in continuous time with multiple endogenous state variables, using the two-asset HANK model of Kaplan-Moll-Violante (2018) as lead example. </p>
date: 2025-09-05
paperurl: 'http://ssabet.github.io/files/Nested.pdf'
repourl: 'https://github.com/SSabet/NestedDrift'
---
We introduce a new algorithm for solving continuous time problems
with multiple endogenous state variables in a finite–difference scheme.
The algorithm extends the logic of up–winding to its logical extreme in
a way that meets the necessary conditions for local convergence (Barles
and Souganidis, 1991). It is consistent because the directions of state–
drift are never in conflict, and constraints are applied non–linearly. It is
efficient because it nests the search for these state–drifts in a way that
ensures costly root–finding is only performed after other alternatives
are exhausted. The algorithm improves on the existing ‘split–drift’
approach from (Kaplan et al., 2018; Achdou et al., 2022), which can
fail under some parameter settings because it is not guaranteed to be
consistent.

<img src='/images/nested.png'>
