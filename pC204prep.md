this file: pC204prep.md

**Hello World** <img align="right" width="220" height="220" src="/assets/IMG/template_logo.png">
good search terms: 
"machine learning streamflow recession forecast"

"machine learning hydrologic signatures"

CAMELS data is needed to run the analysis script created for this project.
Location of files: https://gdex.ucar.edu/dataset/camels/file.html
URLs for specific files uploaded by the script:
1. https://gdex.ucar.edu/dataset/camels/file/camels_clim.txt
2. https://gdex.ucar.edu/dataset/camels/file/camels_topo.txt
3. https://gdex.ucar.edu/dataset/camels/file/camels_geol.txt

Here is the data file I created for this project

my working file folders

1. desk C:\Hydrology\DataResources\CAMELS\
   
2. desk C:\Hydrology\DataResources\CAMELS\BotterillMcMillan2021

I found 27 gages in CAMELS that I have already calibrated.  I have calibrated 35 additional gages in CAMELS.  Potentially there are 18 more gages (two of which I deemed unsuitable)  gages that I can add that meet my selection criteria..

Selection Criteria:  gage in 'WA OR ID MT' and 1950 GAGESII (PRISM) pcp >250 mm

Here are 28 gages in CAMELS that are in CAMELS, meet the selection criteria, but that I have not yet calibrated.

After previewing, and removing two that are glacial meltwater contaminated (Hoh, Thunder Creek),I have 26 candidates. I can add more if necessary and time permits:

[11482500, 11532500, 12010000, 12020000, 12035000, 12040500,  12043000, 12054000, 12056500, 12115500, 12117000, 12143600, 12144000, 12145500, 12147500, 12178100, 12189500, 14138900, 14216500, 14236200, 14305500, 14306340, 14306500, 14309500, 14325000, 14400000]


CA 11482500   718.0 km2  max elev:1619 aspect: 1619 PPT1950_AVG:2503 RUNAVE7100: 1079.5  REDWOOD C A ORICK CA
CA 11532500   1578.0 km2  max elev:1944 aspect: 1944 PPT1950_AVG:3681 RUNAVE7100: 2140.7  SMITH R NR CRESCENT CITY CA
WA 12010000   142.2 km2  max elev:797 aspect: 797 PPT1950_AVG:3967 RUNAVE7100: 1869.9  NASELLE RIVER NEAR NASELLE, WA
WA 12020000   294.2 km2  max elev:948 aspect: 948 PPT1950_AVG:2856 RUNAVE7100: 1109.7  CHEHALIS RIVER NEAR DOTY, WA
WA 12035000   769.9 km2  max elev:1187 aspect: 1187 PPT1950_AVG:3501 RUNAVE7100: 2777.8  SATSOP RIVER NEAR SATSOP, WA
WA 12040500   1153.4 km2  max elev:2211 aspect: 2211 PPT1950_AVG:4619 RUNAVE7100: 3733.1  QUEETS RIVER NEAR CLEARWATER, WA
WA 12041200   655.8 km2  max elev:2389 aspect: 2389 PPT1950_AVG:4646 RUNAVE7100: 3351.0  HOH RIVER AT US HIGHWAY 101 NEAR FORKS, WA
WA 12043000   337.2 km2  max elev:1144 aspect: 1144 PPT1950_AVG:3572 RUNAVE7100: 3354.0  CALAWAH RIVER NEAR FORKS, WA
WA 12054000   171.7 km2  max elev:2080 aspect: 2080 PPT1950_AVG:2757 RUNAVE7100: 1993.7  DUCKABUSH RIVER NEAR BRINNON, WA
WA 12056500   147.0 km2  max elev:1904 aspect: 1904 PPT1950_AVG:5311 RUNAVE7100: 1906.1  NF SKOKOMISH R BL STAIRCASE RPDS NR HOODSPORT, WA
WA 12115500   34.7 km2  max elev:1444 aspect: 1444 PPT1950_AVG:3363 RUNAVE7100: 1233.6  REX RIVER NEAR CEDAR FALLS, WA
WA 12117000   44.9 km2  max elev:1243 aspect: 1243 PPT1950_AVG:3231 RUNAVE7100: 1235.1  TAYLOR CREEK NEAR SELLECK, WA
WA 12143600   165.0 km2  max elev:1903 aspect: 1903 PPT1950_AVG:3544 RUNAVE7100: 2048.3  SF SNOQUALMIE RIVER AT EDGEWICK, WA
WA 12144000   210.1 km2  max elev:1903 aspect: 1903 PPT1950_AVG:3356 RUNAVE7100: 2015.0  SF SNOQUALMIE RIVER AT NORTH BEND, WA
WA 12145500   79.0 km2  max elev:1060 aspect: 1060 PPT1950_AVG:2696 RUNAVE7100: 2066.1  RAGING RIVER NEAR FALL CITY, WA
WA 12147500   102.9 km2  max elev:1800 aspect: 1800 PPT1950_AVG:2957 RUNAVE7100: 2140.4  NORTH FORK TOLT RIVER NEAR CARNATION, WA
WA 12175500   273.8 km2  max elev:2756 aspect: 2756 PPT1950_AVG:2814 RUNAVE7100: 1806.6  THUNDER CREEK NEAR NEWHALEM, WA
WA 12178100   69.7 km2  max elev:2460 aspect: 2460 PPT1950_AVG:2981 RUNAVE7100: 1813.0  NEWHALEM CREEK NEAR NEWHALEM, WA
WA 12189500   1855.3 km2  max elev:3210 aspect: 3210 PPT1950_AVG:3147 RUNAVE7100: 2134.5  SAUK RIVER NEAR SAUK, WA
OR 14138900   21.7 km2  max elev:1195 aspect: 1195 PPT1950_AVG:4427 RUNAVE7100: 1879.0  NORTH FORK BULL RUN RIVER NEAR MULTNOMAH FALLS, OR
WA 14216500   349.5 km2  max elev:2473 aspect: 2473 PPT1950_AVG:3526 RUNAVE7100: 1878.0  MUDDY CREEK BELOW CLEAR CREEK NEAR COUGAR, WA
WA 14236200   361.0 km2  max elev:1434 aspect: 1434 PPT1950_AVG:2818 RUNAVE7100: 1577.7  TILTON RIVER AB BEAR CANYON CREEK NEAR CINEBAR, WA
OR 14305500   526.3 km2  max elev:1082 aspect: 1082 PPT1950_AVG:3876 RUNAVE7100: 2307.3  SILETZ RIVER AT SILETZ, OR
OR 14306340   14.7 km2  max elev:1041 aspect: 1041 PPT1950_AVG:2979 RUNAVE7100: 1503.4  EAST FORK LOBSTER CREEK NEAR ALSEA, OR
OR 14306500   857.2 km2  max elev:1245 aspect: 1245 PPT1950_AVG:2975 RUNAVE7100: 1511.5  ALSEA RIVER NEAR TIDEWATER, OR
OR 14309500   224.9 km2  max elev:1311 aspect: 1311 PPT1950_AVG:3028 RUNAVE7100: 591.0  WEST FORK COW CREEK NEAR GLENDALE, OR
OR 14325000   443.1 km2  max elev:1239 aspect: 1239 PPT1950_AVG:3761 RUNAVE7100: 1583.3  SOUTH FORK COQUILLE RIVER AT POWERS, OR
OR 14400000   702.6 km2  max elev:1535 aspect: 1535 PPT1950_AVG:3911 RUNAVE7100: 2886.5  CHETCO RIVER NEAR BROOKINGS, OR

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/1ab65dda-4241-4526-b6ae-993d7570264e)

Preview plots - checking for sign of gross irregularity in the hydrographs

USGS 11482500 REDWOOD C A ORICK CA

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/8a4c8688-4e08-4c44-8f7b-ffc0e2a8a073)


USGS 11532500 SMITH R NR CRESCENT CITY CA.....USGS 14161500 LOOKOUT CREEK NEAR BLUE RIVER, OR

#https://waterdata.usgs.gov/nwis/dv?period=&begin_date=1900-01-01&end_date=2023-11-11&referred_module=sw&cb_00060=on&site_no=11532500%2C12010000%2C12020000%2C12035000%2C14161500&legacy=&format=gif_mult_sites

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/358df02a-b8c6-4885-9913-5726efffa194)


USGS 12040500 QUEETS RIVER NEAR CLEARWATER, WA
USGS 12041200 HOH RIVER AT US HIGHWAY 101 NEAR FORKS, WA
USGS 12043000 CALAWAH RIVER NEAR FORKS, WA
USGS 12054000 DUCKABUSH RIVER NEAR BRINNON, WA
USGS 12056500 NF SKOKOMISH R BL STAIRCASE RPDS NR HOODSPORT, WA


DROP USGS 12041200 HOH RIVER AT US HIGHWAY 101 NEAR FORKS, WA

because of glacial melt water

https://waterdata.usgs.gov/nwis/dv?referred_module=sw&site_no=14161500%2C12040500%2C12041200%2C12043000%2C12054000%2C12056500%2C121155000&format=gif_mult_sites&PARAmeter_cd=00060&legacy=&begin_date=1900-01-01&end_date=2023-11-11

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/7ccbb505-18e4-4791-8d71-c50cccd6ab03)


USGS 12189500 SAUK RIVER NEAR SAUK, WA ....  USGS 14400000 CHETCO RIVER NEAR BROOKINGS, OR

#https://waterdata.usgs.gov/nwis/dv?referred_module=sw&site_no=14161500%2C12189500%2C14138900%2C14216500%2C14236200%2C14305500%2C14306340%2C14306500%2C14309500%2C14325000%2C14400000&format=gif_mult_sites&PARAmeter_cd=00060&legacy=&begin_date=1900-01-01&end_date=2023-11-11

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/82093131-4a11-4bdc-9d5d-08be3e02d6d5)
![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/ad1ab776-2aa8-4cc2-b9a5-9e59cb1bb432)


USGS 12117000 TAYLOR CREEK NEAR SELLECK, WA...USGS 12178100 NEWHALEM CREEK NEAR NEWHALEM, WA

REJECT: USGS 12175500 THUNDER CREEK NEAR NEWHALEM, WA

https://waterdata.usgs.gov/nwis/dv?referred_module=sw&site_no=14161500%2C12117000%2C12143600%2C12144000%2C12145500%2C12147500%2C12175500%2C12178100&format=gif_mult_sites&PARAmeter_cd=00060&legacy=&begin_date=1900-01-01&end_date=2023-11-11

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/e9a6c6d9-3d5b-451e-b61a-5d669a8aac7e)






![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/cfa47a92-79b0-4454-9a9f-4bbf4640a9b7)

source of above: Wu, Shuyue, et al. "Regional patterns and physical controls of streamflow generation across the conterminous United States." Water Resources Research 57.6 (2021): e2020WR028086.


Botterill, Tom E., and Hilary K. McMillan. "Using Machine Learning to Identify Hydrologic Signatures With an Encoder–Decoder Framework." Water Resources Research 59.3 (2023): e2022WR033091.  https://agupubs.onlinelibrary.wiley.com/doi/pdfdirect/10.1029/2022WR033091

link for TOSSH:  https://github.com/TOSSHtoolbox/TOSSH

list of parameters that they added to the CAMELS set: 

gauge_id	EventRR	RR_seasonality	Recession_a_seasonality	AverageStorage	
RecessionParametersAlpha	RecessionParametersBeta	RecessionParametersT0	BaseflowRecessionK	FirstRecessionSlope
MidRecessionSlope	EventRR_TotalRR_Ratio	VariabilityIndex

link for their github website and their recession parameters: https://github.com/mcmillanhk/HydroML/blob/master/data/extra_sigs/gw_array.csv

see screen shot below of part of the table of auxiliary parameters...

Notes:  they used camels database...add alpha, (median) beta non-linear recession parameters to their classical signatures. They had the machine figure out its own hydrologic signatures (it found 16).  ammong the "classic signatures" the alpha and beta parameters were among those most strongly correlated to ML learned parameters. The ML identified the 16 factors by training on streamflow (the model target was hydrologic time series emulation).  Because of the experimental design, their results show indirectly the importance of alpha, beta recession parameters to hydrologic simulation success. The ML simulation model work about as well as calibrated conceptual models.  these parameters are relevant for accurate simulation of streamflow. The Addor CAMELS does not include alpha.
My idea: I pick camels gages where I can get a good fix on alpha beta, I train a machine on streamflow for two different parameter scenarios: each one using features (camels parameters + RecessionParameters), but differeing in source of RP. One of the sources will be mine, another could be exponential, and a third maybe Botteril and McMillan's parameters?


![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/5bc4d009-3c06-453f-921f-242e662de66c)





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


###===================================================================
###===================================================================

###Addor, Nans, et al. "The CAMELS data set: catchment attributes and meteorology for large-sample studies." Hydrology and Earth System Sciences 21.10 (2017): 5293-5313. cb>400  https://hess.copernicus.org/articles/21/5293/2017/hess-21-5293-2017.pdf

https://gdex.ucar.edu/dataset/camels/file.html

Addor et al 2017=Extension of CAMELS from N15: Newman et al. (2015b).
N=671 minimally impacted by human activities 
20 years of continuous discharge records from 1990 to 2009 and are  we derived climate indices and hydrological signatures using the daily time series 
we added land cover, soil, and geology of each catchment
Climatic indices were derived using the N15 meteorological forcing data.

headers from each of the CAMELS attribute files:
camels_clim.txt headers: gauge_id;p_mean;pet_mean;p_seasonality;frac_snow;aridity;high_prec_freq;high_prec_dur;high_prec_timing;low_prec_freq;low_prec_dur;low_prec_timing
camels_geol.txt headers: gauge_id;geol_1st_class;glim_1st_class_frac;geol_2nd_class;glim_2nd_class_frac;carbonate_rocks_frac;geol_porostiy;geol_permeability
camels_name.txt headers: gauge_id;huc_02;gauge_name
camels_topo.txt headers: gauge_id;gauge_lat;gauge_lon;elev_mean;slope_mean;area_gages2;area_geospa_fabric
camels_vege.txt headers: gauge_id;frac_forest;lai_max;lai_diff;gvf_max;gvf_diff;dom_land_cover_frac;dom_land_cover;root_depth_50;root_depth_99

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/09bb6082-5886-4b06-a9ca-1ef41c3c6218)



![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/fdb941e4-31b9-46fa-aabc-b200e06697d8)


![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/817d7f02-c768-4267-bc5e-0b442b5a0400)
![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/4ab24bdf-cd20-4759-ae60-24e67fa88777)

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/3cb535f1-c3d9-4e50-9286-789bada3b791)

hydrologic signatures

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/c6df94f9-8d60-4587-ba08-6cf4d1d65af4)

![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/793582b0-35c2-4fb1-b81d-c3573cdbca44)


![image](https://github.com/jcsias/jcsias.github.io/assets/149276387/73019226-77ad-4989-8366-5b0ca733dc62)


