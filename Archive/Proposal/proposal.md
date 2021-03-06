Optimal control of neglected tropical diseases using a simple dynamic model
================
Chris Hoover
April 2, 2018

Background:
-----------

Neglected tropical diseases (NTDs) tend to be diseases of poverty that thrive in tropical, disadvantaged communities that often lack access to basic amenities such as clean water, sanitation, and healthcare. They are generally environmentally mediated meaning that some component of their transmission cycle depends on the environment (e.g. a vector, intermediate host, or free-living environmental stage). Control of NTDs generally relies on the administration of drugs that cure individuals from the disease and may confer short-term immunity. However, following drug administration, people are often reinfected by the environmental stage(s) of the pathogen that persist through mass drug administration (MDA) campaigns. Additional interventions that target these environmental reservoirs are often available, but underutilized due to their indirect effects on improving individuals' health.

Description:
------------

Using a simple, generalizable model of NTD transmission presented in [Garchitorena et al](http://rstb.royalsocietypublishing.org/content/372/1722/20160128) I will investigate the ability of different interventions to effectively eliminate the disease from the human population. In this generalizable model, two interventions will be considered: 1) drug administration, implemented as a pulse reduction in the state variable, *I*, that reduces the prevalence of the disease in the population and 2) environmental remediation (e.g. improvement in sanitation, vector control), implemented as a permanent alteration of a model parameter, that reduces the transmission of the disease.

Data:
-----

This project will be mostly simulation based but the model and parameters used for initial simulations/explorations will be drawn from [Garchitorena et al](http://rstb.royalsocietypublishing.org/content/372/1722/20160128)

Analyses:
---------

1.  Explore model dynamics resulting from implementing proposed interventions alone and in combination. Replicate Fig 3c from [Garchitorena et al](http://rstb.royalsocietypublishing.org/content/372/1722/20160128)
2.  Translate the model into a Markov decision process (MDP) solvable with stochastic dynamic programming (SDP) by following the "Six steps of stochastic dynamic programming" in [Marescot et al](https://besjournals.onlinelibrary.wiley.com/doi/full/10.1111/2041-210X.12082)
3.  Find the optimal intervention stretagey for this simple disease model using SDP implemented with the R package MDPtoolbox
