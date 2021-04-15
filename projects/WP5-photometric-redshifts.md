---
layout: page
title: Project
permalink: projects/wp5-photoz/
subtitle: WP5 - Photometric redshifts
---

## Context

This work package will be devoted to Bayesian measurement of photo-z from multi-band images, extracting for each galaxy a p(z) distribution, directly from the blended images (see [Jones and Heavens 2019][jones19]). Compared to the state of the art, which uses template fitting or neural networks applied to _colors_ (difference between the measured magnitudes in two bandpass) to derive a value of the redshift with a (Gaussian) uncertainty, and is prone to _catastrophic errors_ where degeneracies yield to selecting a bad solution, we plan to work directly at the pixel level, on multiband image cubes, and output a p(z) probability distribution, using Bayesian networks.

Some work has already been done on that topic, within LSST-France ([Pasquet et al. 2019][pasquet19]), but using deep convolutional networks that output probability distribution functions, considering the problem as a classification problem, rather than Bayesian networks. We plan to use Bayesian techniques on multicolor image cubes, using both LSST 6-band images, and LSST+Euclid 10-band images.

## Lead

This work will be led by APC with contributions from LORIA

[jones19]: https://arxiv.org/abs/1808.02846
[pasquet19]: https://arxiv.org/abs/1806.06607