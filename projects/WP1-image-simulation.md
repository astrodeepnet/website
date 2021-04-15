---
layout: page
title: Project
permalink: projects/wp1-sims/
subtitle: WP1 - Realistic image simulation
---

#### Context

This work package will deal with simulating realistic images, using traditional techniques or generative networks. We will use software tools like GalSim ([Rowe et al. 2015][rowe15]) and PhoSim ([Peterson et al. 2015][peterson15]) to generate images of galaxies with typical observation conditions, and instrumental effects. The Dark Energy Science Collaboration (DESC collaboration) is also producing simulated LSST/Rubin images (the latest set is the Data Challenge 2) that we will use as test images. In order to generate more efficiently the large amount of images needed to train the networks used in other workpackages, we plan to use generative networks, like Generative Adversarial Networks (GAN, [Goodfellow et al. 2014][goodfellow14]) or Variational Autoencoders (VAE, [Kingma and Welling 2013][kingma13]), which, once trained, are much faster than codes like GalSim (see for instance [Ravanbakhsh et al. 2016][ravanbakhsh16]). We have already tested using VAE as galaxy images generators with promising results ([Arcelin et al. 2020][arcelin20], Figure 1). 

This work will probably iterate with the deblending work package (WP3) since some networks useable for deblending have common parts with generators (like the decoder part of an autoencoder), or more generally both problems require the notion of what a typical galaxy looks like.
Other work packages (WP3-5) will use the output of this one, although we will also use the data simulated in LSST DESC Data Challenges, and precursor surveys real data. Our generators could be used in future data challenges image simulation, if relevant.

#### Lead

This work will be led by APC, with contributions from LORIA.



[kingma13]: https://arxiv.org/abs/1312.6114
[goodfellow14]: https://arxiv.org/abs/1406.2661
[rowe15]: https://arxiv.org/abs/1407.7676
[peterson15]: https://arxiv.org/abs/1504.06570
[ravanbakhsh16]: https://arxiv.org/abs/1609.05796
[arcelin20]: https://arxiv.org/abs/2005.12039