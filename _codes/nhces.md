---
title: "Aiyagari Model with Non-homothetic CES Preferences and Multiple Sectors: Steady State and Transition"
collection: codes
permalink: /codes/NhCES
excerpt: "How to robustly solve for the steady state and transition paths of an Aiyagari model in continuous-time with non-homothetic CES preferences (as in Lashkari-et-al (2021)) and three sectors? The Matlab code below proposes an algorithm based on a predefined approximation of inverse of marginal utility of expenditure using the so-called 'Chebyshev technology'. Transition path in response to one or several series of MIT shocks can be efficiently solved for, using a first-order perturbation of the approximant of the inverse of marginal utility and perturbed relative prices along the transition path. The code is written for three sectors, but the code remain as efficient for large number of sectors (as long as the production functions are static and relative prices can be solved for as it is with the current model). The implementation below uses the excellent 'Chebfun' package of Matlab, but a similar implementation is available in Julia (upon request)."
date: 2022-07-30
repourl: 'https://github.com/SSabet/Aiyagari-nhces.m'
---
