## Sensitivity tests results ## 

This folder contains the results of three different sensitivity tests presented in Xiao et al, in each test, a subset of the parameters are constrained at their true values at the optimization step to see if this can improve the accuracy of other parameters. 

Line 41 of **PDE_GradientMatching_FixPar.R** can be adjusted to change the parameters being fixed at the true values. dn & dm; dn & gamma; dn & gamma & rn were fixed at their true values correspondingly in the three different tests, the results were written in folder **SimRes_constrained**, the averaged parameter estimates were written in the corresponding .txt file.   

At the end, the MATLAB file **Parameter_estimations** was used to plot the averaged parameter estimates at different levels of measurement error in different tests.  


