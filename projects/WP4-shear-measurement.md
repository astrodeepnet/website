---
layout: page
title: Project
permalink: projects/wp4-shear/
subtitle: WP4 - Shear measurement
---

## Context

This work package will address the issue of galaxy shape measurement, a central task for weak gravitational lensing. If galaxy orientations are randomly distributed, their ellipticity averages out intrinsically. An observed non-vanishing orientation is a local estimate of shear induced by gravitational lensing of the intervening large-scale structure. Measuring shear gives us unbiased information about the dark-matter distribution in the Universe.

A crucial task of shape measurement is calibration, since generally the estimated shear is biased. The science requirements for LSST/Rubin, Euclid, or WFIRST/Roman are very challenging, demanding calibration at the 0.1% level. A major source of bias are blended objects ([Euclid Collaboration et al. 2019][euclid19]), and one of the main tasks of this WP is to quantify the residual biases as a metric of the deblending techniques developped in WP3.

We will explore the recently introduced metacalibration technique ([Sheldon and Huff 2017][sheldon17]), which allows to calibrate the measured shear from the images directly, without the need of image simulations. We will quantify the performance of this technique in the presence of blended objects at different redshifts. Further, we will develop Bayesian inference techniques that do not require the measurement of individual galaxy shapes like in [Bernstein and Armstrong 2014][bernstein14] and [Bernstein et al. 2016][bernstein16].

Similar methods have been implemented in the field of mining agronomic landscapes where external pressures “shear” the plot mosaic. When a medium size territory encounters external pressures like biodiversity preservation or a contrario gene fluxes, the crop mosaic is distorted by the new farmers decisions ([Schaller et al. 2012][schaller12]). Stochastic models combined with a a priori set of decision rules have given interesting results in this domain.

There has been early attempts at using neural networks to address bias in shear measurements ([Gruen et al. 2010][gruen10]), or on building a low-bias shear estimator on individual galaxies using measured features ([Tewes et al. 2019][tewes19]). Although using deep learning at the pixel level is starting to be used for photo-z (see WP5), or for measuring galaxy features ([Tuccillo et al. 2018][tucillo18]; [Huertas-Company et al. 2018][huertas18]), this is still mostly uncharted territories for weak lensing.

## Lead

This work will be led by DAp with contributions from LORIA and APC.

[gruen10]: https://arxiv.org/abs/1002.0838
[schaller12]: https://link.springer.com/article/10.1007/s10980-011-9691-2
[sheldon17]: https://arxiv.org/abs/1702.02601
[bernstein14]: https://arxiv.org/abs/1304.1843
[bernstein16]: https://arxiv.org/abs/1508.05655
[tucillo18]: https://arxiv.org/abs/1711.03108
[huertas18]: https://arxiv.org/abs/1804.07307
[tewes19]: https://arxiv.org/abs/1807.02120
[euclid19]: https://arxiv.org/abs/1902.00044