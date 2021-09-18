# Ensemble SINDy and PDE-FIND
 
This repository contains Matlab code to reproduce the results of the paper:
  
**Ensemble-SINDy: Robust sparse identification of nonlinear dynamics for ordinary- and partial differential equations with uncertainty quantification**

Urban Fasel, J. Nathan Kutz, Bingni W. Brunton, Steven L. Brunton.  



## Ensemble-SINDy

### Comparing different ensemble-SINDy methods 

#### Lorenz system

[SINDy/main_runEnsembleSINDy_heatmap.m](/SINDy/main_runEnsembleSINDy_heatmap.m)  
 * compare different ensemble SINDy methods in terms of model error (error of SINDy coefficients) and success rate (probability to get the correct model structure) over a range of noise levels and data length
 * plot heatmap
    
![ensembleSINDy_heatmap](/SINDY/results/ensembleSINDy_heatmap.png)  

    
[SINDy/main_runEnsembleSINDy_UQ.m](SINDy/main_runEnsembleSINDy_UQ.m)   
 * for one particular noise level and data length, run Enesmble-SINDy and get plots of:
    * SINDy coefficient uncertainties and inclusion probabilities
    * ensemble dynamics reconstruction and forecast 

#### Lotka Volterra Lynx and Hare polpulation data 1900-1920 Hudson Bay Company

[SINDy/main_runLotkaVolterra.m](SINDy/main_runLotkaVolterra.m)  
 * SINDy coefficient uncertainties and inclusion probabilities
 * ensemble dynamics reconstruction


## Ensemble-PDE-FIND

[PDE-FIND/main_weakEnsemblePDE.m](PDE-FIND/main_weakEnsemblePDE.m)  
 * run comparison (model error and success rate) between weak PDE-FIND and weak-ensemble PDE-FIND to identify five different PDEs from very noisy data

[PDE-FIND/main_get_FiguresTable.m](PDE-FIND/main_get_FiguresTable.m)  
 * plot figures shown in table below 


![table_ensemble-PDEFIND](/PDE-FIND/PlotsPaper/table_ensemble-PDEFIND.png)
