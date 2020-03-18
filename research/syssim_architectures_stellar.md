# Occurrence and architectures of planetary systems as a function of stellar type

In [He, Ford, & Ragozzine (2019)](https://arxiv.org/abs/1907.07773) (which we will refer to as Paper I), we developed several models for the intrinsic architectures of planetary systems by forward modelling the Kepler catalog of planet candidates (see this [page](https://hematthi.github.io/research/syssim_architectures.html) for a summary). For that paper, we used a catalog of FGK dwarf stars and assumed that the distribution of planetary systems was the same across all the stars.

Here, we improve on our best model to explore how the architectures of planetary systems depend on their host stars. The details are in the full paper: [He, Ford, & Ragozzine (2020)](https://arxiv.org/abs/2003.04348).

<center><img src="/research/images/Kepler_planets_variety_NASA_MSFC.jpg" alt="Art: A Variety of Planets" width="800"/></center>  
*Artist's depiction of the many types of planets that exist, similar to those that Kepler discovered. Image credit: NASA MSFC*


### Kepler sensitivity to transiting planets

For this study, we split our sample of FGK dwarfs into two halves using their Gaia b<sub>p</sub>-r<sub>p</sub> colors, which is related to the effective temperatures of the stars (this is how we classify the spectral types of stars): larger values of b<sub>p</sub>-r<sub>p</sub> correspond to redder, cooler stars while smaller values correspond to bluer, hotter stars. We find that Kepler detected a similar number of planets in these two halves.

How likely we are detect a transit depends on its signal to noise ratio (SNR). The signal is the transit depth times the square root of the duration, while the noise is the photometric variability of the light curve. To first approximation, the transit depth of a planet is simply a geometric effect: the planet blocks out a small fraction of the total light coming from the star during its transit. Thus for a given sized planet, it would induce a larger transit depth if it were transiting a smaller, cooler star than a larger, hotter star. However, cooler stars are fainter and thus Kepler's photometric precision of these targets is worse than that of hotter stars (i.e. noisier light curves).

<center><img src="figures/Clustered_P_R_fswp_bprp_fig5.pdf" alt="Figure 5 in paper"/></center>  
*Figure 5 in He, Ford, & Ragozzine (2020). Planets transiting cooler stars (higher values of b<sub>p</sub>-r<sub>p</sub> color) induce a larger transit depth due to the smaller sizes of the stars, but Kepler's photometry of these stars is noisier (quantified by the root-mean-square CDPP values) thus compromising our ability to recover transits.*


### The fraction of stars with planets

As discussed above, by splitting the Kepler stars in our sample into two halves (redder and bluer), we find that the Kepler planet counts are also close to split in equal halves. However, simulating a Kepler mission with a model that assumes the same numbers of planets across all stars (such as the models from Paper I) produces too many detected planets around the bluer stars, since their less noisy light curves make it somewhat easier to recover transits overall.

This implies that planets must be more common around redder (cooler) stars. Indeed, a few previous studies have suggested a similar trend. We introduce a linear dependence for the fraction of stars with planets (f<sub>swpa</sub>) as a function of the stellar (b<sub>p</sub>-r<sub>p</sub>) color, into our clustered models. We fit these two additional parameters (the slope and normalization constant for this linear function) simultaneously with all the other parameters of the model using a similar method as in Paper I.

<center><img src="figures/Clustered_P_R_fswp_bprp_fig3.pdf" alt="Figure 3 in paper"/></center>  
*Figure 3 in He, Ford, & Ragozzine (2020). The fraction of stars with planets (f<sub>swpa</sub>; between 3 and 300 days) increases towards cooler stars.*


We find a significant positive slope for f<sub>swpa</sub>(b<sub>p</sub>-r<sub>p</sub>), indicating that roughly a third of early F dwarfs (left end of the figure above) host a planetary system while this fraction increases to 100% for mid K dwarfs (right end of the figure above). For reference, our Sun is a G2V star with b<sub>p</sub>-r<sub>p</sub> = 0.82. Thus, our results show that roughly half of all Sun-like stars host a planetary system in the range we considered (between 3 and 300 days).

<center><img src="figures/Models_cartoon_stellar.pdf" alt="Cartoon of new models"/></center>  
*Cartoon illustrating the main results of this paper.*
