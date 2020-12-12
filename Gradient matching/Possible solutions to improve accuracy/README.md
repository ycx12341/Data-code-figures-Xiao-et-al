## Possible solutions to improve accuracy ##

This folder records the attempts made in the manuscript Xiao et al. which aims to improve the accuracy of the parameter estimates. 

The reference gradients predicted by GAM without measurement errors and the true gradients calculated by the finite difference scheme are recorded in **Reference gradients GAM.txt** and **True gradients forward difference scheme.txt**, which were generated in folder **Results without measurement errors**.

The .R file **Truncated gradients.R** generates the parameter estimates obtained using the truncated gradient matrices (boundary spatial points and integer timepoints were truncated, the size of each gradient matrix became 5*38) of each perturbed data set in folder **SimRes_ests_converge_check**, the final parameter estimates are stored in **Parameters means truncated.txt**.

The .R file **Replaced TC gradients except gamma.R** generates the parameter estimates obtained using the updated gradient matrices, where all the tumour cells related gradients except the haptotaxis term related to gamma were replaced by the corresponding true gradients in **True gradients forward difference scheme.txt**. The updated gradient matrices are presented in folder **SimRes_ests_tc_except_gamma_ests_fds_grads**, the final parameter estimates are given in **Parameters means tc gradients except gamma replaced by FDS grads**.

The .R file **Replaced TC gradients.R** generates the parameter estimates obtained using the updated gradient matrices, where all the tumour cells related gradients were replaced by the corresponding true gradients in **True gradients forward difference scheme.txt**. The updated gradient matrices are presented in folder **SimRes_replaceall_tc_ests_fds_grads**, the final parameter estimates are given in **Parameters means tc gradients replaced by FDS grads**.

The .R file **Replaced TC and dm gradients.R** generates the parameter estimates obtained using the updated gradient matrices, where all the tumour cells related gradients and the second order spatial gradients related to parameter dm were replaced by the corresponding true gradients in **True gradients forward difference scheme.txt**. The updated gradient matrices are presented in folder **SimRes_replace_tc_and_dm_ests_fds_grads**, the final parameter estimates are given in **Parameters means tc dm gradients replaced by FDS grads**.

The .R file **Replaced TC dm dmdt gradients.R** generates the parameter estimates obtained using the updated gradient matrices, where all the tumour cells related gradients, the temporal gradients of MDE and the second order spatial gradients related to parameter dm were replaced by the corresponding true gradients in **True gradients forward difference scheme.txt**. The updated gradient matrices are presented in folder **SimRes_replace_tc_and_dm_dmdt_ests_fds_grads**, the final parameter estimates are given in **Parameters means tc dm dmdt gradients replaced by FDS grads**.

The folder **MATLAB plots** contains the plots of parameter estimates of each attempt mentioned above at different levels of measurement errors.

