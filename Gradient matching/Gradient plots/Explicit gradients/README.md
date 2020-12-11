## Averaged gradients ##

The folder **SimRes_ests_converge_check** contains the results of parameter estimates at 5 different level of measurement errors. 

The .R file **Explicit gradients analysis** generates the spatial/temporal gradients averaged over time and data sets, then record them in the corresponding .txt files. 

The .m file **Gradient_plots** plots the averaged spatial/temporal gradients based on the .txt files generated previously. 

The reference gradients predicted by GAM without measurement errors and the true gradients calculated by the finite difference scheme are stored in **Reference gradients GAM.txt** and **True gradients forward difference scheme.txt**, which were generated in folder **Results with no measurement errors**, check there for more details of these two files. 
