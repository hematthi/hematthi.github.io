# Stability and collisions of triple stellar systems

I had the opportunity to do research in the summer immediately after graduation from the University of Toronto (U of T), under the supervision of Dr. Cristobal Petrovich at the Canadian Institute for Theoretical Astrophysics (CITA). Our goal was to test previously proposed analytical criteria for the long-term stability of triple systems based on their initial configurations. These stability criteria are of particular interest to dynamicists who wish to study various outcomes of systems with three stars. We used [REBOUND](https://github.com/hannorein/rebound), an N-body integrator developed by astrophysicists at U of T, to perform numerical simulations of the dynamical evolution of triple systems over Gyr timescales. In addition to confirming that the two commonly used criteria in the literature for predicting stability are quite reliable for a wide range of parameters, we also used our simulations to compute the collision rates for systems involving various stellar objects (e.g. between main sequence and white dwarf stars) by tracking close encounters. The rates of stellar collisions have direct implications for the likelihood of observing astrophysical transients such as Type Ia supernovae, which are the signatures of white-dwarf white-dwarf collisions.

The details of our simulations and results can be found in our published paper, [He & Petrovich (2017)](https://arxiv.org/pdf/1710.04698.pdf).

![Figure 1 in paper](/figures/Triples_paper_fig1.png)
*Figure 1 in He & Petrovich (2017). The two panels show the performance of each of the two popular stability criteria in the literature. A value of 0 (i.e. the vertical dashed line) denotes the boundary of the stability criteria, and the red and blue curves denote the fraction of unstable and stable systems, respectively.*

![Figure 4 in paper](/figures/Triples_paper_fig4.png)
*Figure 4 in He & Petrovich (2017). Evolution of a triple stellar system initially close to the stability boundary, that ended in an unstable outcome (ejection of a body).*
