### Neonatal-connectome-dynamics-predicts-neurocognitive-outcome

This repository provides code and data for data analysis in the article entitled "Development of neonatal connectome dynamics and its prediction for cognitive and language outcomes at age 2" by Xu et al.2023.

___
### Data

#### 1. Basic information of rs-fMRI scans, including age,sex, headmotion parameter and age duration between birth and scan
- infant_info.mat 
- behavior.mat
> Note: the resting-state functional MRI (rs-fMRI) data of all participants are obtained from the Upenn-Chop project.  
> gender, ‘-1’ and ‘1’ denote female and male, respectively; mFD, mean framewise displacement; age, scan age in days; age_diff, age duration time between birth and scan.  
> 

#### 2.  Random parcellation
- ROI_256.nii
> Note: a customized random parcellation, which was obtained by parcellating the gray matter tissue into 256 regions with uniform sizes.

#### 3.  Regional time series of infants
- MTC_256.mat
#### 4.  Regional modular variability of infants
- MV_256.mat
___
### Codes
#### 1. Multilayer community detection
> The time-resolved modular architecture was detected using an open MATLAB code package :[http://netwiki.amath.unc.edu/GenLouvain/GenLouvain](http://netwiki.amath.unc.edu/GenLouvain/GenLouvain)[1] .
#### 2.Modular variability 
-   Scaled_inclusivity_wei.m [2]
-   Ami.m
#### 3. general linear model 
- glm_for_baby.m
#### 4.behavior prediction 

>The behavior prediction analysis was conducted using an open MATLAB code package : https://github.com/ZaixuCui/Pattern_Regression_Matlab/tree/master/SVR [3]
___
### References
1.  Jeub LGS, Bazzi M, Jutla IS, Mucha PJ. A generalized Louvain method for community detection implemented in MATLAB. Version 2.1 [software]. 2012 [updated 2016 Nov; cited 2021 Jan 2]. Available from:  [http://netwiki.amath.unc.edu/GenLouvain](http://netwiki.amath.unc.edu/GenLouvain).
2.  Liao X, Cao M, Xia M, He Y. Individual differences and time-varying features of modular brain architecture. NeuroImage. 2017;152:94-107.
3.  Cui Z, Gong G, The effect of machine learning regression algorithms and sample size on individualized behavioral prediction with functional connectivity features. NeuroImage. 2018; 178: 622-37
