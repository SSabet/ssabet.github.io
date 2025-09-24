---
title: "Model with Two Assets and Kinked Adjustment Costs (HANK)"
collection: codes
permalink: /codes/nested
excerpt: "We introduce a new algorithm for solving continuous time problems with multiple endogenous state variables in a finite–difference scheme. The algorithm extends the logic of up–winding to its logical extreme in a way that meets the necessary conditions for local convergence (Barles and Souganidis, 1991). It is consistent because the directions of state–drift  are never in conflict, and constraints are applied non–linearly. It is efficient because it nests the search for these state–drifts in a way that ensures costly root–finding is only performed after other alternatives are exhausted. The algorithm improves on the existing ‘split–drift’ approach from (Kaplan et al., 2018; Achdou et al., 2022), which can fail under some parameter settings because it is not guaranteed to be consistent."
date: 2024-03-30
paperurl: 'http://ssabet.github.io/files/Nested.pdf'
repourl: 'https://github.com/SSabet/NestedDrift'
---
