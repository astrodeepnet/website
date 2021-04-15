---
layout: page
title: Project
permalink: projects/wp2-noise/
subtitle: WP2 - Uncertainty propagation and noise reduction
---

## Context

This work package will address the general question of noise propagation and reduction through neural networks. Input astronomical images have carefully characterised noise properties (photon noise, CCD readout noise, electronic noise, etc.). Traditional algorithms propagate those uncertainties to the final measurement. This capability is a very strong requirement for any astronomical image processing software. For instance, when deblending overlapping galaxies, the input noise will end up being split between the images of the individual galaxies and a sky background image. Pixels of the output images might have correlated noise, and this noise correlation must also be characterized. It is also well-known that autoencoders can be used for denoising ([Vincent et al. 2008][vincent18]). We will design ways to estimate the noise properties of the final measurements, and will explore the applicability of Bayesian neural networks for this purpose.

The research work in this WP is motivated by the recent developments in machine learning and especially in deep learning where neural networks achieves very good results in image classification, speech recognition and natural language processing. Many methods are developed to analyze and explore these data in a supervised setting, as it should be the case in this WP. However, most of the produced data does not come with metadata and/or labeling. This raises two possible directions of investigation: (i) learning to classify using a few labeled examples, and (ii) transferring what was learned in a given domain into another domain. Actually, active learning (AL) tries to overcome the difficulty of having a few examples available, and may involve interaction. Deep learning poses several difficulties when used in an active learning setting, as, by contrast, active learning methods generally rely on the capability to learn and update learning models from small amounts of data. Accordingly, in this WP, we will study and adapt the idea of “Bayesian Active Learning” based on recent methodologies about an active learning framework for high dimensional complex data combining Bayesian deep learning and active learning ([Gal 2016][gal16a]; [Gal and Ghahramani 2016][gal16b]; [Gal, Islam, and Ghahramani 2017][gal17]). In addition, Bayesian Active Learning is well suited to deal with uncertainty as this is the case for standard Bayesian networks ([Ghahramani 2015][ghahramani15]).

Then, for completing this research direction, we will assess the possibility of using transfer learning. In concrete terms, transfer learning is the process of training a model on a large-scale dataset and then using that pre-trained model to conduct learning within another domain and for another task. Indeed, transfer learning was popularized in the field of pattern recognition and language understanding ([Yang et al. 2018][yang18]). It has also been used recently for transferring galaxy morphology information from one large survey to another ([Domínguez Sánchez et al. 2019][dominguez19]). The idea is to conduct a deep pre-training of entire models with hierarchical representations or graph-based representations. Following this way, we can then try to use graph convolution networks with domain knowledge or knowledge graphs (i.e. DBpedia, YAGO2) to disambiguate or enrich classification models.

A final direction of investigation is related to the combination of classifiers and the production of explanations. Firstly, we will consider a deep learning approach based on special architectures such as convolutional networks and autoencoders ([Badrinarayanan, Kendall, and Cipolla 2017][badrinarayanan17]). Then, we will also consider other classifiers such as random forests for producing explanations. We will extend preceding studies about the combination of classifiers such as in ([Grissa et al. 2019][grissa19]) for understanding the performance of the mining process and gain a better control about recognition and classification. To conclude it should be noticed that, e.g. in ([Biehl et al. 2018][bielh18]; [Kremer et al. 2017][kremer17]), the major role to be played by explanations in mining astronomical data is stressed, especially for _opening black boxes_ such as neural networks and understanding their behaviors.

## Lead

This work will be led by LORIA with contributions from APC.


[ghahramani15]: https://www.nature.com/articles/nature14541
[gal16a]: http://www.cs.ox.ac.uk/people/yarin.gal/website/blog_2248.html
[gal16b]: https://arxiv.org/abs/1506.02142
[gal17]: https://arxiv.org/abs/1703.02910
[kremer17]: https://arxiv.org/abs/1704.04650
[badrinarayanan17]: https://ieeexplore.ieee.org/abstract/document/7803544
[vincent18]: https://dl.acm.org/doi/pdf/10.1145/1390156.1390294
[yang18]: https://research.fb.com/wp-content/uploads/2019/06/GLoMo-Unsupervised-Learning-of-Transferable-Relational-Graphs.pdf
[bielh18]: http://www.cs.rug.nl/~biehl/Preprints/ESANN2018-AstroSession.pdf
[grissa19]: https://www.sciencedirect.com/science/article/pii/S0166218X18306346
[dominguez19]: https://arxiv.org/abs/1807.00807