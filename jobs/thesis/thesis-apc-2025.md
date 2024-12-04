---
layout: page
title: Thesis at APC
permalink: jobs/thesis-apc-2025/
subtitle: At the crossroad of large galaxy surveys : developing cosmic shear analysis with Bayesian neural networks for Dark Energy studies with the Vera Rubin Observatory LSST
---

- 3-year PhD thesis starting with a 3-month internship.
- supervisors: [Cécile Roucelle](mailto:jobs@astrodeep.net), Eric Aubourg

At the crossroad of large galaxy surveys : developing cosmic shear analysis with Bayesian neural networks for Dark Energy studies with the Vera Rubin Observatory LSST.


During the last decade, cosmology has entered a precision era, leading to the prevalence of the standard cosmological model, ΛCDM. Nevertheless, the main ingredient of this model, the so-called dark energy, remains mysterious while dominating the energy budget of the Universe. Its comprehension is therefore one of the main goals in this domain. The starting generation of cosmological surveys, among which the one of the Euclid satellite launched last year and the Legacy Survey of Space and Time (LSST) of the Vera Rubin Observatory (on the ground) which will see its first light mid-2025 (commissioning is already going on !). 

These surveys, when combined, will map thousands of square degrees of sky in a multiwavelength manner with sub-arcsec resolution. This will result in the detection of several tens of billions of sources, enabling a wide range of astrophysical investigations and providing unprecedented constraints on the nature of dark energy and dark matter. The scope of the PhD topic, based in the LSST dark energy science collaboration context, will aim to bring new developments at the intersection of the two surveys. More precisely, the PhD topic discussed here (and the preceding internship) will focus on developing analyses for weak gravitational lensing and will aim at being able to combine the data of LSST and Euclid. We will use machine learning approaches that we want to build into Bayesian pipelines which is the context of our “AstroDeep” ANR funding, and the direction taken by our research team for the past few years. 
 
The gravitational lensing corresponds to the deflection of light from distant sources (background galaxies) due to the bending of space-time by matter along the line of sight, resulting in  distortions and displacements of their image. The statistical study of weak gravitational lensing distortions at large scales provides a “mapping” of the matter (dark or visible) between the observer and source (well, more accurately, the effect we want to study is the one of the small and coherent deformation of background galaxies following the principle described here and which is called cosmic shear). The measurement of cosmic shear (and its combination with other probes) gives a window on the properties and the evolution of cosmic structures as well as the geometry of the Universe. Its study can therefore bring higher constraints on the origin of the current accelerated expansion of the Universe that led to the notion of dark energy. In the absence of systematic errors, weak lensing is even recognised as the single most constraining probe of dark energy. As such, its analysis is one of the main science drivers for both LSST and Euclid. 

Two main requirements are essential for using cosmic shear: accurately measuring galaxy shapes and their redshifts. Given the wealth and volume of forthcoming data, these aspects present a set of new challenges, for which machine learning techniques are particularly well suited.
For example, the sheer volume of produced data requires the development of new types of analyses that allow more efficient processing. Plus novel complexities arise. To address these challenges, our group has started to develop an approach based on Bayesian neural networks (BNNs, see for example [1]). The BNNs offer a formalism to quantify and propagate uncertainties associated with deep neural networks models and also with the data itself, which are both key for cosmological analyses. 
To give an idea, as more and more galaxies and stars populate the images in deep surveys, the local density increases and the projected objects naturally overlap. This phenomenon, referred to as blending, impedes the ability to properly measure the shapes and photometry of individual objects and  will affect more than 60% of the galaxies in LSST. To address this issue, deep learning brings a possible solution, with an efficient use of the joint multi-band processing of LSST and Euclid images. The images are fed to a BNN to separate overlapping galaxies before measuring their shape and this approach brings an improvement to the use of one of the surveys alone (as it brings the complexity but also the power of a multi-resolution and multiwavelength approach to the problem). We have demonstrated the feasibility of this approach in a configuration with several simulated galaxies per image ([2]) and developed several architectures aiming at the deblending of images in our group ([2], [3]).  

The goal of this PhD project is to advance beyond these established applications by exploring new avenues for using combined data from different observational modalities. As suggested by Parker et al. [4], training networks on both imaging and spectroscopic data can produce informative embeddings that encode physical information. This training can be self-supervised on non-labeled data (as long as imaging and spectroscopy data have been matched) and then utilized with zero-shot or few-shot training. Alternatively, the training can be supervised using simulated data with subsequent transfer to real data.

During the course of this PhD, both realistic simulations and public data from the spectroscopic survey DESI, matched with either LSST and Euclid data, will be used to train original architectures. The research will have two main goals:

- Validate the approach.
- Apply the method to new on-sky data from the best surveys of the decade.

This will yield improved performance in deblending, photometric redshift (photo-z) and shape measurements, and ultimately in the characterization of dark energy.
During the pre-thesis internship, the main topic to pursue would be to enter the topic, familiarize with the existing architectures that have been developed in the group and to test further this new approach of multimodal training of neural networks with galaxy imaging and spectroscopy on simplified mock data.  

### Context : 

From a local environment perspective, this PhD will occur in the scope of the AstroDeep project started in October 2019 at APC and that has started a follow up ANR funding in 2024. This project intends to build a collaboration between cosmologists, statisticians and computer scientists, focused on the quantification of uncertainties in cosmological analyses with Bayesian neural networks. The student joining our group will beneficiate from such collaboration to build knowledge in an emergent field, working on the comprehension, characterization and use of the BNNs, and also apply these exciting techniques to astrophysical images to perform a multi-instrument and multi-wavelength joint analysis of galaxy fields. 

AstroDeep has been a pioneer in Bayesian deep learning techniques, with applications for handling blending in deep surveys, and simulation-based inference. The group has strong ties with the Rubin/LSST Dark Energy Science Collaboration (LSST-DESC) and the LSST Informatics & Statistics Science Collaboration (ISCC). The research will be conducted in connection with working groups from these collaborations.
If successful, the implications of this work could drastically reduce the bias on cosmic shear measurements and release an essential tool for observational cosmology to the community. Not to mention that LSST and Euclid data will become available for science in 2026 , during the PhD thesis, making these studies all the more interesting as the scientific environment will be extremely dynamic.

### Proposed research activities :

The research will utilize both realistic simulated data, developed within relevant scientific collaborations like DESC, and data from recent surveys such as DESI, Rubin/LSST, and Euclid. A significant part of the work will involve comparing, selecting, adapting, and improving existing machine learning techniques, or developing new ones, to build neural networks capable of learning physical information about galaxies from multi-modal data (including spectra, visible imaging, and infrared imaging).

Bayesian deep learning techniques will be employed to account for uncertainties in the data and models. In addition to classical network architectures like convolutional networks and their Bayesian extensions, the student will explore variational autoencoders, transformers and attention mechanisms, physics-informed networks, and self-supervised training techniques like contrastive learning.

The student will also gain knowledge in cosmology, weak gravitational lensing, and massive astronomical data processing. The research is expected to produce production-grade software for combined cosmological analysis of multi-modal datasets. The skills and knowledge acquired during the PhD will enable the pursuit of a career in academia, focusing on cosmology or software engineering, as well as opportunities in the private sector.


[1] Tom Charnock, Laurence Perreault-Levasseur, François Lanusse, Bayesian Neural Networks, arXiv:2006.01490
[2] Bastien Arcelin, Cyrille Doux, Eric Aubourg, Cécile Roucelle, Deblending galaxies with Variational Autoencoders: a joint multi-band, multi-instrument approach, Monthly Notices of the Royal Astronomical Society, staa3062, https://doi.org/10.1093/mnras/staa3062 arXiv:2005.12039v1
[3] MADNESS Deblender Maximum A posteriori with Deep NEural networks for Source Separation, B. Biswas, E. Aubourg, A. Boucaud, A. Guinot, J. Lao, C. Roucelle, and the LSST Dark Energy Science Collaboration, under review by A&A https://hal.science/hal-04680436v1 see also B. Biswas PhD thesis 
[4] AstroCLIP: A Cross-Modal Foundation Model for Galaxies, L. Parker, F. Lanusse et al. arXiv:2310.034



