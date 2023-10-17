### Prenatal development of brain connectome dynamics

This repository provides code and data for data analysis in the article entitled "Early development of functional connectome dynamics and neurodevelopment outcomes prediction in the preterm human brain" by Xu et al.2023.

___
### Data

#### 1. Basic information of rs-fMRI scans, including age,sex, headmotion parameter and age duration between birth and scan
- infant_info.mat 
- behavior.mat
- covariates.mat
> The resting-state functional MRI (rs-fMRI) data of all participants are obtained from the Upenn-Chop developmental connectome project (http://brainmrimap.org/penn-chop-developmental-connectome-data-preterm-and-term.html). The behavior data includes cognitive and language scores that are obtained with the Bayley Scales of Infant and Toddler Development Ⅲ [1].
>gender, ‘-1’ and ‘1’ denote female and male, respectively; mFD, mean framewise displacement; age, scan age in days; age_diff, age duration time between birth and scan.  
> 

#### 2.  Random parcellation
- ROI_256.nii
> The customized random parcellation, which was obtained by parcellating the gray matter tissue into 256 regions with uniform sizes.

#### 3.  Regional time series of infants
- MTC.mat
#### 4.  Regional modular variability of infants
- MV.mat
___
### Codes
#### 1. Multilayer community detection
> The time-resolved modular architecture was detected using an open MATLAB code package (http://netwiki.amath.unc.edu/GenLouvain/GenLouvain) [2] .
#### 2.Modular variability 
-   Scaled_inclusivity_wei.m
-   Scaled_inclusivity.m
-   Ami.m
#### 3. general linear model 
- glm_for_baby.m
#### 4.behavior prediction 
> cui ; SVR
- SVR_LOOCV.m 
___
### References
1. Bayley 
2.  Jeub LGS, Bazzi M, Jutla IS, Mucha PJ. A generalized Louvain method for community detection implemented in MATLAB. Version 2.1 [software]. 2012 [updated 2016 Nov; cited 2021 Jan 2]. Available from:  [http://netwiki.amath.unc.edu/GenLouvain](http://netwiki.amath.unc.edu/GenLouvain).
3.  Liao X, Cao M, Xia M, He Y. Individual differences and time-varying features of modular brain architecture. Neuroimage. 2017;152:94-107.
4.  Wang J, Wang X, Xia M, Liao X, Evans A, He Y. GRETNA: a graph theoretical network analysis toolbox for imaging connectomics. Front Hum Neurosci. 2015;9:386.
