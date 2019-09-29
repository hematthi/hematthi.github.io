# Architectures of the *Kepler* multi-transiting systems

To date, almost 4000 exoplanets have been discovered and confirmed, with an additional couple thousand potential candidates yet to be verified (click [here](https://exoplanetarchive.ipac.caltech.edu/docs/counts_detail.html) to keep up to date with the official numbers). A large majority of these exoplanets were discovered by the Kepler Space Telescope, the instrument central to the wildly successful mission of monitoring over 150 000 stars near continuously for several years in the search for transiting exoplanets. Although the telescope was launched almost a decade ago in 2009, and has since been recently decommissioned, Kepler’s wealth of data remains one of the most informative catalogues to study for advancing exoplanet science.

The Kepler dataset of transiting exoplanets is particularly valuable because it offers both a substantial sample of exoplanet detections, as well as a relatively uniform selection of target stars with well known observational biases that can be modeled. These properties make it ideal for systematically studying exoplanet demographics. This is exactly the focus of a project led by PIs Prof. Eric Ford (my advisor) and Prof. Darin Ragozzine — a framework for simulating catalogs of planetary systems via the Kepler pipeline — and the codebase is available in our [GitHub repository for ExoplanetsSysSim](https://github.com/ExoJulia/ExoplanetsSysSim.jl) (which we call “SysSim” for short).

My research falls within the SysSim framework by taking advantage of its characterization of the Kepler detection pipeline in order to forward model the observed data by generating ensembles of planetary systems in a statistical manner. The Kepler exoplanet catalog includes a rich sample of (over 600!) systems with multi-transiting planets, which offer key insights into their orbital architectures.

You can read more about this work in our [full paper](https://arxiv.org/abs/1907.07773).

You can access our [GitHub repository for Clustered Planetary Systems](https://github.com/ExoJulia/SysSimExClusters) if you wish to download our model catalogs, or even simulate your own catalogs!


<center><img src="figures/Models_cartoon.pdf" alt="Figure 1 in paper"/></center>  
*Figure 1 in He, Ford, & Ragozzine (2019). Cartoon illustration of the three models we explored, from a non-clustered model to a model with clustered periods and planet sizes.*


<center><img src="figures/Clustered_P_R_Model_KS_posterior_corner.pdf" alt="Figure 3 in paper"/></center>  
*Figure 3 in He, Ford, & Ragozzine (2019). Posterior distribution for the parameters of our clustered periods and sizes model.*


<center><img src="figures/Clustered_P_R_observed.gif" alt="Best-fit clustered models"/></center>  
*Animation showing our best-fit clustered models compared to the Kepler data.*


<center><img src="figures/Clustered_P_R_3plus_multis_0.pdf" alt="Gallery of systems with 3+ observed planets"/></center>  
*Gallery of all systems with 3 or more observed planets, in the Kepler data and in a simulation from our clustered model. Can you guess which is which?*
