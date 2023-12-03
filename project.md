## My Project

I applied machine learning techniques to investigate... Below is my report.

***

## Introduction 

Here is a summary description of the topic. Here is the problem. This is why the problem is important.

There is some dataset that we can use to help solve this problem. This allows a machine learning approach. This is how I will solve the problem using supervised/unsupervised/reinforcement/etc. machine learning.

We did this to solve the problem. We concluded that...

An important theme in hydrologic research is regionalization of streamflow model parameters. To regionalize a hydrologic model parameter, one looks for significant regressions between empirical watershed attributes one the one hand, and – on the other - hydrologic model parameters determined for gaged locations through model calibration.  If a strong relationship is found, then the possibility exists for successful parameterization of a hydrologic model for an ungaged watershed based on the regression model.  Botterill and McMillan 2022 (hereafter, BM22) use a connected neural network model to “learn” streamflow simulation model parameters from a combination of geophysical data and hydro-meteorological  time series data. They performed this training for watersheds in the CAMELs dataset (Addor et al. 2017).  They produced 16 machine-learned (“ML”) parameters for each of 670 watersheds in the continental United States.  Using a new subjective procedure (Sias, unpublished) I have - for twenty-seven of these watersheds - independently estimated a characteristic recession parameter that I will call beta. In principle beta should depend only on geology. This parameter beta is interesting to me because of its potential usefulness as a hydrologic simulation model parameter. BM22 estimated beta for each watershed in CAMELS and included their beta as a feature variable. Using the same geophysical feature variables that BM22 used in their model training (but omitting their beta values), I will train a new ML model to predict beta. I will perform this training/testing twice, using using my beta as the target in one training and the BM22 beta in the second training.  For reasons that I will not elaborate on here, I  hypothesize that the ML model trained on my beta values will produce better test performance than that of a ML model trained on the BM22 beta values.  In Figure 1  I show that the Sias and BM22 estimates of beta for these twenty-seven watersheds are discrepant, causing me to  expect significantly different global minimum cost function values for the different target data. 

The main outcomes of this proposed work are expected to be as follows.

1.	The comparison of the global minimum cost function values provides a basis for judging which method for estimating beta is likely to lead to more success in a hydrologic model parameter regionalization scheme.
   
2.	The results of this project will provide a preliminary assessment of whether a machine learning approach can replace my subjective procedure for estimating beta.
3.	
References.

Addor, Nans, et al. "The CAMELS data set: catchment attributes and meteorology for large-sample studies." Hydrology and Earth System Sciences 21.10 (2017): 5293-5313.

Botterill, T. E., & McMillan, H. K. (2023). Using machine learning to identify hydrologic signatures with an encoder–decoder framework. Water Resources Research, 59, e2022WR033091. https://doi. org/10.1029/2022WR033091

## Data

Here is an overview of the dataset, how it was obtained and the preprocessing steps taken, with some plots!

![](assets/IMG/datapenguin.png){: width="500" }

*Figure 1: Here is a caption for my diagram. This one shows a pengiun [1].*

## Modelling

Here are some more details about the machine learning approach, and why this was deemed appropriate for the dataset. 

The model might involve optimizing some quantity. You can include snippets of code if it is helpful to explain things.

```python
from sklearn.ensemble import ExtraTreesClassifier
from sklearn.datasets import make_classification
X, y = make_classification(n_features=4, random_state=0)
clf = ExtraTreesClassifier(n_estimators=100, random_state=0)
clf.fit(X, y)
clf.predict([[0, 0, 0, 0]])
```

This is how the method was developed.

## Results

Figure X shows... [description of Figure X].

## Discussion

From Figure X, one can see that... [interpretation of Figure X].

## Conclusion

Here is a brief summary. From this work, the following conclusions can be made:
* first conclusion
* second conclusion

Here is how this work could be developed further in a future project.

## References
[1] DALL-E 3

[back](./)

