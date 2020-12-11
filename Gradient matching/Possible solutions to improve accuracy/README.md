## Possible solutions to improve accuracy ##

This folder records the attempts made in the manuscript Xiao et al. which aims to improve the accuracy of the parameter estimates. 

The reference gradients predicted by GAM without measurement errors and the true gradients calculated by the finite difference scheme are recorded in **Reference gradients GAM.txt** and **True gradients forward difference scheme.txt**, which were generated in folder **Results without measurement errors**.

The .R file **Truncated gradients.R** generates the parameter estimates obtained using the truncated gradient matrices (boundary spatial points and integer timepoints were truncated, the size of each gradient matrix became 5*38) of each perturbed data set in folder **SimRes_ests_converge_check**, the final parameter estimates are stored in **Parameters means truncated.txt**.
