---
layout: page
title: Project
permalink: projects/wp3-blending/
subtitle: WP3 - Galaxy deblending
---

## Context

This work package will focus on detecting and deblending objects, and separating stars from galaxies (using colors and shapes). At the depth of LSST about half of the galaxies overlap with another galaxy. In order to measure the shape of the galaxies, a requirement for any weak lensing analysis, the objects have to be separated. Our team has already gained experience on neural-net-based deblending ([Boucaud et al. 2019][boucaud20]; [Arcelin et al. 2020][arcelin20]). In A[rcelin et al. 2020][arcelin20] we have used networks derived from variational autoencoders. The decoder part is simply trained on centered, isolated galaxies (and can be used in the context of WP2). The encoder part is fed with images containing several galaxies, and trained to reproduce only the centered galaxy and delete the other ones. 

The final software will comprise a mix of algorithms and neural networks, in order to iteratively select, isolate and subtract identified galaxies. Several paths will be explored, including dense networks, convolutional networks, Bayesian networks, with various divergences, or combinations of those. A metric relevant to the end problem (measuring the shear of galaxies) will be defined to benchmark the different techniques.

## Lead

This work will be led by APC with contributions from LORIA and DAp.

[boucaud20]: https://academic.oup.com/mnras/article/491/2/2481/5650521
[arcelin20]: https://arxiv.org/abs/2005.12039