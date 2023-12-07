## My Project

I applied machine learning techniques to investigate relationships between Antarctic Sea-ice Thickness and various Southern Hemispheric Atmospheric Indices. 

Below is my report:

***

## Title 

Understanding relationships between Antarctic sea-ice thickness and the southern hemispheric atmospheric circulations


## Introduction 

Sea-ice distribution in Antarctica is subject to diverse atmospheric and oceanic processes, contributing to non-uniform expansion across the region. Regional disparities are evident, with the Ross Sea experiencing positive (expanding) sea-ice anomalies, while the Amundsen-Bellingshausen Sea witnesses negative (retreating) anomalies (Lefebvre & Goosse, 2008; Matear et al., 2015; Raphael et al., 2016; Zwally et al., 2002). The causative factors for such patterns remain unclear, with proposed influences including atmospheric temperature and wind stress changes (Lefebvre & Goosse, 2005, 2008; Liu et al., 2004) and atmospheric feedback mechanisms (Stammerjohn et al., 2012; Stammerjohn et al., 2008).
This study focuses on Southern Hemisphere atmospheric circulation patterns and their role in explaining interannual variability in Southern Ocean sea-ice trends, with a specific emphasis on Sea-Ice Thickness (SIT). The project aims to elucidate the relationships between Antarctic SIT and five primary large-scale atmospheric circulation indices in the Southern Hemisphere: Southern Annular Mode (SAM), Amundsen Sea Low (ASL), El-Nino Southern Oscillation (ENSO), Meridional Wind Index (MWI), and Zonal Wave-3 Index (ZW3). While these indices are recognized as primary drivers of Antarctic sea-ice changes, their influence varies regionally, and no singular mode has been identified as the predominant factor governing total sea-ice changes in Antarctica. In addition to regional heterogeneity, seasonal variabilities in sea-ice are influenced by atmospheric models. Given the non-linear relationships between sea-ice and atmospheric variables, this study employs supervised Random Forest Regression, a machine learning algorithm, to comprehend and predict these intricate relationships. The objectives of this study include:

I.	Understanding the Significance of Climatic Modes:

a.	Identifying the primary dictating factor for sea-ice distribution in each region.

b.	Assessing the magnitude and direction of the impact.


II.	Assessing effectiveness of selected Machine Learning Algorithm: 

a.	Evaluating the efficacy of supervised machine learning algorithm, specifically Random Forest Regression, in capturing spatio-temporal relationships.

b.	Investigating the seasonal variations in the performance of regional specific-trained Random Forest Regression models.


## Data

My project will utilize gridded NetCDF datasets which are 3-D datasets (longitude, latitude, time) for various sea-ice and atmospheric variables. These will be derived from the historical experiment of the CMIP6’s coupled climate model (i.e. CESM2) for the time-period of 1979-2014. The dataset can be accessed and downloaded from the ESGF website via following: https://esgf-node.llnl.gov/search/cmip6/. Various climatic indices have been calculated using different atmospheric variables obtained from the historical experiment of CESM2 couple climate model. The details can be found in Table 1. 


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

