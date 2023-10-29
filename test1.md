
**Hello World** <img align="right" width="220" height="220" src="/assets/IMG/template_logo.png">
good search terms: 
"machine learning streamflow recession forecast"

"machine learning hydrologic signatures"



![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/cfa47a92-79b0-4454-9a9f-4bbf4640a9b7)

source of above: Wu, Shuyue, et al. "Regional patterns and physical controls of streamflow generation across the conterminous United States." Water Resources Research 57.6 (2021): e2020WR028086.

google search term "machine learning hydrologic signatures"
Botterill, Tom E., and Hilary K. McMillan. "Using Machine Learning to Identify Hydrologic Signatures With an Encoder–Decoder Framework." Water Resources Research 59.3 (2023): e2022WR033091.  https://agupubs.onlinelibrary.wiley.com/doi/pdfdirect/10.1029/2022WR033091

they used camels database...add alpha, (median) beta non-linear recession parameters to their classical signatures. They had the machine figure out its own hydrologic signatures (if foudn 16).  ammong the "classic signatures" the alpha and beta parameters were among those most strongly correlated to ML learned parameters. The ML identified the 16 factors by training on streamflow (the model target was hydrologic time series emulation).  Their results underscore the importance of alpha beta as string flow signatures. The experimental design shows these parameters are relevant for accurate simulation of streamflow . The Addor CAMELS does not include alpha
My idea: I pick camels gages where I can get a good fix on aplpha beta, I train a machine on streamflow for two different parameter scenarios: each one using features (camels parameters + RecessionParameters), but differeing in source of RP. One of the sources will be mine, another could be exponential, and a third maybe Botteril and McMillan's parameters?

cb 1
cites Gnann et al 2021

Eng, Ken, David M. Wolock, and Michael Wieczorek. "Predicting baseflow recession characteristics at ungauged stream locations using a physical and machine learning approach." Advances in Water Resources 175 (2023): 104440.  

**Problem is their target values for the recession constansts are dependend on the method of estimation, and which from my research I have rejected as a valid method for estimating recession parameters.  Under the hypothesis that watershed do indeed possess characteristic recession parameters, then true parameter values exist.  The closer that a database of estimated parameters are to the truth, the more highly these should correlate to geophysical parameters, in so far as the parameters are determined by fundamentally and primarily by geology.  These target values may or may not be biased or uncorrelated with the "true" values.   I would like to test whether my estimates of characgteristic watershed b-values are found through machine learning to be more predictable than estimates prepared by other sources...basically I want to comduct a competition between different estimates of b-values for the same set of watersheds, preferablly limiting the competition for now to watersheds in winter-wet temperatute and mediterranean climate zones.**

Gnann, Sebastian J., et al. "TOSSH: A toolbox for streamflow signatures in hydrology." Environmental Modelling & Software 138 (2021): 104983.
cb 30

Istalkar, Prashant, Akshay Kadu, and Basudev Biswal. "Value of process understanding in the era of machine learning: A case for recession flow prediction." Journal of Hydrology (2023): 130350.

Prieto, C., Vine, N. L., Kavetski, D., García, E., & Medina, R. (2019). Flow prediction in ungauged catchments using probabilistic random forests regionalization and new statistical adequacy tests. Water Resources Research, 55(5), 4364–4392. https://doi.org/10.1029/2018WR023254
Note 1: Basically, the ML-Bayesien parameter inference procedure did NOT work out. Two steps to go from watershed xteristics to inferred model parameters:  1) fit RF model to predict flow index PC for prognostic watershed. *2) Then use the trained Bayesism scheme to infer the hydrosimmodle parameter.  Then run to the model on the prognostic watershed. 3) estimate the hydro params for the prognostic watershed with a conventional approach. (4)  Compare the model performed based on the source of parameters (ML-Bayesian vs conventional).  They got pretty good results on the RF testing data (i.e., did good job estimating the "true" flow index PCS on the testing watersheds, but when these used to estimate simulation model parameters, GOT POOR hydrograph simulation RESULTS using the inferred hydrosim parameters!! 

Note 3:  how would conventionally calibrated model on a training gage do against the model using parameters estimated by the ML-Scheme? This should jdefine the upper level of how well we could hope to on the testing data. This is the calibration assessment.  If the calibration assessment is highly unfavorable for the ML-B pareters, then expect to have no better and probably worse results in the validation (the results with the test data).

Note 2: cited by Botter et al: "Signatures can be used to calibrate hydrologic models in ungauged basins, by regionalizing the signatures (estimating signature values based on watershed attributes) and then calibrating the model against the regionalized signatures (Prieto et al., 2019)"

ABSTRACT:  This study attacks the prediction in ungauged catchment problem by ... First, [formed] orthogonal set of “flow index PCs.” These  are regionalized using random forests regression [I wonder what they used as their feature variables?] and  used to condition hydrological model parameters using a Bayesian scheme. Second, “adequacy” tests are proposed to evaluate a priori the hydrological and regionalization model performance in the space of flow index PCs. The proposed regionalization approach is applied to 92 northern Spain catchments, with 16 catchments treated as ungauged. It is shown that (1) a small number of PCs capture approximately 87% of variability in the flow indices and (2) adequacy tests with respect to regionalized information are indicative of (but do not guarantee) the ability of a hydrological model to predict flow time series and are hence proposed as a prerequisite for flow prediction in ungauged catchments. The adequacy tests identify the regionalization of flow index PCs as adequate in 12 of 16 catchments but **the hydrological model as adequate in only 1 of 16 catchments.** Hence, a focus on improving hydrological model structure and input data (the effects of which are not disaggregated in this work) is recommended.

Tyralis, Hristos, et al. "Explanation and probabilistic prediction of hydrological signatures with statistical boosting algorithms." Remote Sensing 13.3 (2021): 333. 

Singh, Shailesh Kumar, and George A. Griffiths. "Prediction of streamflow recession curves in gauged and ungauged basins." Water Resources Research 57.11 (2021): e2021WR030618.  " Both Euclidean Distance and Random Forest methods were employed to determine degree of similarity between a reference basin and an ungauged site. Results are shown in Table 5 which shows a much superior performance as assessed by MAE and RMSE for the Random Forest method."

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/3232d841-4ac5-4d77-9430-a2d7d26737a0)

Figure above from the Sing et al paper.  Maybe I can train RF to estimate recession parameters for a handful of CAMELS gages; I can train a model on different "truth" data, each truth being z different researcher's estimates of  b-values  Then the distance between RF model and Truth I expect will be smallest if trained on my b-value than when trained on someone else's.  So basically I run a contest that I also enter.

Štravs, L., & Brilly, M. (2007). Development of a low-flow forecasting model using the M5 machine learning method. Hydrological sciences journal, 52(3), 466-477.

Addor, Nans, et al. "The CAMELS data set: catchment attributes and meteorology for large-sample studies." Hydrology and Earth System Sciences 21.10 (2017): 5293-5313. cb>400  https://hess.copernicus.org/articles/21/5293/2017/hess-21-5293-2017.pdf

Addor et al 2017=Extension of CAMELS from N15: Newman et al. (2015b).
N=671 minimally impacted by human activities 
20 years of continuous discharge records from 1990 to 2009 and are 
we derived climate indices and hydrological signatures using the daily time series 
we added land cover, soil, and geology of each catchment
Climatic indices were derived using the N15 meteorological forcing data.
![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/09bb6082-5886-4b06-a9ca-1ef41c3c6218)



![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/fdb941e4-31b9-46fa-aabc-b200e06697d8)


![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/817d7f02-c768-4267-bc5e-0b442b5a0400)
![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/4ab24bdf-cd20-4759-ae60-24e67fa88777)

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/3cb535f1-c3d9-4e50-9286-789bada3b791)

hydrologic signatures

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/c6df94f9-8d60-4587-ba08-6cf4d1d65af4)

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/793582b0-35c2-4fb1-b81d-c3573cdbca44)


![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/73019226-77ad-4989-8366-5b0ca733dc62)

