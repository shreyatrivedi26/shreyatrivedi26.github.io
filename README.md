**Hi class, welcome to the AOS C111/204 final project!** <img align="right" width="220" height="220" src="/assets/IMG/template_logo.png">

For this project, you will be applying your skills to train a machine learning model using real-world data, then publishing a report on your own website.

* To get data for your project, you could:
  * use **your own data** from a separate research activity
  * **scour the internet** to find something original, then preprocess it yourself - see the Module Overview on BruinLearn for some resources
  * browse an archive of data designed for machine learning problems, such as the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/datasets)

* Your report should be in the region of 2000-2500 words with three to four figures, and written in a scientific language and style. [This template page](/project.md) gives an example structure that you could use, but feel free to make it your own.

Your website will be a great addition to your CV, and a place to host future projects too since it doubles as a GitHub repository. The first step is to set up a project website like this one by following the instructions below. 

## How does this website work?

First, check out the Github repository for this site: [https://github.com/atmosalex/atmosalex.github.io/](https://github.com/atmosalex/atmosalex.github.io/).

Using GitHub pages, you can write a website using markdown syntax - the same syntax we use to write comments in Google Colab notebooks. GitHub pages then takes the markdown file and renders it as a web page using a Jekyll theme. The markdown source code for this page [is shown here](https://github.com/atmosalex/atmosalex.github.io/blob/main/README.md?plain=1).

## Setting up your Project Website

### How to copy this site as a template
1. Create [a GitHub account](https://github.com/)
2.	Create a new GitHub repository with the name **username.github.io**, where **username** is your GitHub username as shown below. Select *public* and do not tick *Add a README file*. [![screenshot][1]][1]
3.	From your new repository, you should see a *Quick setup* guide. Scroll down to the bottom of the page and click *Import code*, as shown: [![screenshot][2]][2]
4.	In the box that says *Your old repository’s clone URL*, copy and paste this URL: `https://github.com/atmosalex/atmosalex.github.io/`, then proceed.
5.	Go to the *Settings* tab, then click *Pages* (under *Code and automation*), and check that the *Build and deployment* section looks like this: [![screenshot][3]][3]
6.	If you can see the *Actions* tab, click it and check that the build and deployment action has finished. Once it has, navigate to **[username].github.io** to see your site, which should be a copy of this one! If you cannot see an *Actions* tab, just wait a few minutes then go to your URL to check it is live.

Now you are ready to customize your site! To add your name to the site, go to your Github page, edit `_config.yml`, and replace the temporary title with your name.

[1]: /assets/IMG/instr_create.png
[2]: /assets/IMG/instr_import.png
[3]: /assets/IMG/instr_bd.png

### How to change the theme (optional)
1.	You can choose any theme [listed on this page](https://pages.github.com/themes/), though some do not work as well on mobile devices.
2.	From GitHub, edit `_config.yml` and replace the `theme:` line with `theme: jekyll-theme-name` where `name` is the name of the theme from the above list. **For the `minima` theme, use a shortened preface like so `theme: minima`**, the others seem to need the whole preface `theme: jekyll-theme-`. You can check the *Actions* tab (as in step 6. above) to make sure the site is building successfully.

### How to change your site logo (optional)
1. Some themes, such as `jekyll-theme-minimal`, show a logo. In your repository, upload a logo or profile picture to the `assets/IMG/` directory
2. Open `_config.yml` and modify the line `logo: /assets/IMG/template_logo.png` to point to your new image

***

## Guide to Adding Content
* Your repository's `README.md` file (the file you are reading now) acts like a home page. Replace its contents with whatever you want the world to see by editing the file on GitHub.
* If you want to turn this page into a CV or blog, etc., it may be useful to refer to a [guide for writing Markdown](https://www.markdownguide.org/basic-syntax/).
* You can create other markdown files (.md) in your repository and navigate to them from this page using links, i.e.: [here is a link to another file, `project.md`](project.md)
* When editing a markdown file on GitHub, it is useful to wrap text by selecting the *Soft wrap* option as shown: ![screenshot](/assets/IMG/instr_wrap.png)
* If you want to get even more technical, you can also write HTML in your .md files, and GitHub Pages will render it. For example, the image below is displayed by writing the following (edit this file to see!): `<img align="right" width="200" height="200" src="/assets/IMG/template_frog.png">`
<img align="right" width="337" height="200" src="/assets/IMG/template_frog.png"> 

***

## Delivering your Project

Your final project has three components: a dataset, a report, and your code.

### Dataset

A link to the dataset you used must be submitted on BruinLearn so that your course instructor can use it to run your code. To do this, it might be easiest to upload the dataset to Google Drive, then share a link (click *Share* then *Copy link*). If your dataset is too big to upload, try to find a way to reduce its size, or speak with your instructor if this is not possible.

### Report

Your report should be **delivered via your website**. Submit a link to your website on BruinLearn so that your instructor can browse it to find your report. 

To make this simple, you can write the report using a word processor or Latex, then export it as a .pdf file and upload it to the `assets` directory. You can then link to it [like so](/assets/project_demo.pdf). However, you can also type the report directly onto the website using another markdown page - [here is](/project.md) a template for that.

### Code

A link to your code must be submitted on BruinLearn, and the course instructor must be able to download and run your code using the dataset. The code could be in a Google Colab notebook (make sure to *share* the notebook so access is set to **Anyone with the link**), or you could upload the code into a separate GitHub repository, or you could upload the code into the `assets` directory of your website and link to it. 


### Report 

AOS C204: Machine Learning in Physical Sciences 
Final Project

Title: Understanding relationships between Antarctic sea-ice thickness and the southern hemispheric atmospheric circulations

Introduction 
Sea-ice distribution in Antarctica is subject to diverse atmospheric and oceanic processes, contributing to non-uniform expansion across the region. Regional disparities are evident, with the Ross Sea experiencing positive (expanding) sea-ice anomalies, while the Amundsen-Bellingshausen Sea witnesses negative (retreating) anomalies (Lefebvre & Goosse, 2008; Matear et al., 2015; Raphael et al., 2016; Zwally et al., 2002). The causative factors for such patterns remain unclear, with proposed influences including atmospheric temperature and wind stress changes (Lefebvre & Goosse, 2005, 2008; Liu et al., 2004) and atmospheric feedback mechanisms (Stammerjohn et al., 2012; Stammerjohn et al., 2008).
This study focuses on Southern Hemisphere atmospheric circulation patterns and their role in explaining interannual variability in Southern Ocean sea-ice trends, with a specific emphasis on Sea-Ice Thickness (SIT). The project aims to elucidate the relationships between Antarctic SIT and five primary large-scale atmospheric circulation indices in the Southern Hemisphere: Southern Annular Mode (SAM), Amundsen Sea Low (ASL), El-Nino Southern Oscillation (ENSO), Meridional Wind Index (MWI), and Zonal Wave-3 Index (ZW3). While these indices are recognized as primary drivers of Antarctic sea-ice changes, their influence varies regionally, and no singular mode has been identified as the predominant factor governing total sea-ice changes in Antarctica. In addition to regional heterogeneity, seasonal variabilities in sea-ice are influenced by atmospheric models. Given the non-linear relationships between sea-ice and atmospheric variables, this study employs supervised Random Forest Regression, a machine learning algorithm, to comprehend and predict these intricate relationships. The objectives of this study include:
I.	Understanding the Significance of Climatic Modes:
a.	Identifying the primary dictating factor for sea-ice distribution in each region.
b.	Assessing the magnitude and direction of the impact.
II.	Assessing effectiveness of selected Machine Learning Algorithm: 
a.	Evaluating the efficacy of supervised machine learning algorithm, specifically Random Forest Regression, in capturing spatio-temporal relationships.
b.	Investigating the seasonal variations in the performance of regional specific-trained Random Forest Regression models.

Datasets
My project will utilize gridded NetCDF datasets which are 3-D datasets (longitude, latitude, time) for various sea-ice and atmospheric variables. These will be derived from the historical experiment of the CMIP6’s coupled climate model (i.e. CESM2) for the time-period of 1979-2014. The dataset can be accessed and downloaded from the ESGF website via following: https://esgf-node.llnl.gov/search/cmip6/. Various climatic indices have been calculated using different atmospheric variables obtained from the historical experiment of CESM2 couple climate model. The details can be found in Table 1. 

Table 1: Southern Hemispheric atmospheric. Circulation indices calculated for this study:
Climatic Mode	Variable Used	References
Southern Annular Mode (SAM)	Sea-level Pressure	(Thompson, Wallace, 2000)

El-Nino Southern Oscillation (ENSO)	Sea-surface Temperature	(Kwok & Comiso, 2002)

Meridional Wind Index (MWI)	Meridional Wind (at 850Hpa)	(Hobbs et al., 2016)

Zonal Wave-3 Index (ZW3)	Geopotential Height (at 500HPa)	(Raphael, 2004)

Amundsen Sea Low (ASL)	Sea-level Pressure	(Hosking et al., 2013)


Methodology
Data Pre-processing in Python:
All variables underwent pre-processing in Python using the “xarray” library. Original datasets, in NetCDF 3-D format, were transformed into time series (Fig. 1a) following methodologies detailed in studies outlined in Table 1. The SIT dataset utilized here represents a time series derived from area-averaging calculations of the spatial dataset. For regional analysis, the circum-Antarctic (Southern Ocean) region was partitioned into five major zones: Amundsen-Bellingshausen Seas (ABS), Ross-Amundsen Seas (RAM), East Antarctic, King Hakon VII, and Weddell Sea (Fig. 1b). Additionally, the time series was segregated into two primary sea-ice seasons: Advance (April-August) and Retreat (October-February). This segmentation aligns with the approach outlined in the study by Raphael & Hobbs, 2014.  
  
Figure 1: a) Time series for the five selected atmospheric circulation indices in the Southern Hemisphere; b) Selected Antarctic regions based on Raphael and Hobbs, 2014.

Supervised Machine Learning Approach:
This project employs a supervised Machine Learning Algorithm, specifically the Random Forest Regression Algorithm. Previous studies have established that the trend in daily total Antarctic sea-ice over time is strongly nonlinear and that the linear estimates are weak and dependent on a positive trend that began in 2011 and ended in 2016 (Handcock & Raphael, 2020). This suggests that the relationship between sea ice extent and other climatic variables could also be nonlinear. In a nonlinear relationship, the changes in one variable are not proportional to changes in the other, and the relationship may exhibit complex patterns or behaviors. If linear estimates are weak and dependent on specific trends within a certain timeframe, it implies that a simple linear model may not capture the true nature of the relationship. Nonlinear relationships could involve threshold effects, interactions, or other complexities that linear models might not adequately represent. Therefore, in this study I have employed the use of sophisticated nonlinear models (i.e. a supervised regression technique of Random Forest Regression Algorithm) to better understand the dynamics between Antarctic sea-ice and other climatic variables. The analysis involves identifying various atmospheric indices as “predictors” (features), with the Antarctic SIT as the predicted (target) variable. This process is executed for each region and across two distinct sea-ice seasons.
Prior studies established these selected indices as significant drivers of Antarctic sea-ice changes. To statistically validate their significance, covariance (Fig.2) among the indices was calculated. This analysis justifies their selection based on correlations, where higher correlations imply similar impact and covariability, thereby reducing the distinct impact of individual predictors.
 
Figure 2: Covariance matrix showing correlations between different atmospheric circulation-based indices. 

The preference is for features that are as “mutually exclusive” as possible. Fig.2 illustrates that most of the chosen predictors exhibit minimal correlations among themselves. An exception is observed for the SAM and ASL, with the highest correlation value recorded at -0.56. However, this correlation, although notable, is not significantly high to compromise its relevance as the crucial predictors.

Modeling:
Following python packages were used in constructing a Machine Learning Model: 
 

I constructed a pipeline with feature scaling and Random Forest Regressor as follows: 
 

Thereafter, I calculated feature importance which gave an estimate of how important a particular feature is in determining the target variable i.e. SIT. These feature importance values are then plotted as bar plots for every region and two distinct seasons:
 

This study also employs the use of SHAP (SHapley Additive exPlanations) plots. SHAP values are a way to explain the output of any machine learning model. It uses a game theoretic approach that measures each feature’s contribution to the final outcome. In machine learning, each feature is assigned an importance value representing its contribution to the model’s output (as seen above). SHAP values show how each feature affects each final prediction, the significance of each feature compared to others, and the model’s reliance on the interaction between features. Similarly, SHAP plots were also produced for every region and the seasons:
 

In the end, I have compared the regional Random Forest Regression Models for every season by using the Regression Error Characteristics (REC) Curves to assess how the models have performed in every region:
 

Results
Feature Importance Plots:
 
Figure 3:  Plot showing the feature importance for all the 5 regions (x-axis) and their corresponding importance in the two seasons.





                 EAST ANTARCTIC	                                        AMUNDSEN-BELLINGSHAUSEN SEA
   


ROSS-AMUNDESN SEAS			KIND HAKON VII
   



WEDDELL SEA
 

Figure 4:  SHAP Plots showing the magnitude and the intensity of the impact of the features on the predicted target value i.e. SIT for the 5 regions for Advance Season.

            EAST ANTARCTIC	                                        AMUNDSEN-BELLINGSHAUSEN SEA
   


ROSS-AMUNDESN SEAS			KIND HAKON VII
   


WEDDELL SEA
 

Figure 5:  SHAP Plots showing the magnitude and the intensity of the impact of the features on the predicted target value i.e. SIT for the 5 regions for Retreat Season.

 
Figure 6:  REC Curves for the regional Random Forest Regression Models for two distinct sea-ice seasons.

Discussion and Conclusions
I.	Feature Importance Analysis highlighted and reaffirmed the regional heterogeneity around the Antarctic in terms of distinct atmospheric circulation-based Indices dictating the regional SIT distributions. 

Figure 3 highlights the distinct nature of sea-ice distribution in each Antarctic region, primarily attributed to unique influencing factors that affect the distribution disparately. Each region exhibits a diverse set of dominant climatic indices that mold SIT during specific seasons. For instance, in the Advance season, Zonal Wave-3 (ZW3) emerges as a prominent climatic variability mode in most regions. However, during the Retreat season, the Amundsen Sea Low (ASL) consistently takes precedence as the foremost climate mode across all regions, exhibiting a substantial magnitude difference whereas, ZW3 remains a dormant mode of climatic variability. This substantiates the hypothesis that despite shared atmospheric, oceanic characteristics, and geographical proximity, Antarctic regions experience distinct impacts from specific climate indices, contributing to the observed regional heterogeneity in Southern Ocean sea-ice. Consequently, this analysis aids in discerning the predominant climate mode in each region.
SHAP Plots (Fig.4 and 5) build upon the results from the Fig.3 by assessing the direction and magnitude of the relationships between the climatic indices and SIT across regions and seasons. For the retreat season, Fig.3 illustrates the predominant influence of the ASL on SIT across all Antarctic regions. This information is further supported by SHAP plots in Fig.4, depicting the magnitude and direction of the ASL’s influence. The plots reveal a consistent strong positive relationship between ASL and SIT across all regions. Specifically, higher magnitudes of ASL (represented by red dots) correspond to a positive impact on SIT (reflected via the positive x-axis). In essence, a stronger ASL tends to increase SIT in each region, while a weaker ASL is associated with a decrease in SIT.

II.	The constructed Regional Random Forest Regression Model performs better for the Ross-Amundsen Seas during the Advance season and the East Antarctic Region during the Retreat season. Overall, the seasonal performance of regional models is better during the Advance Season compared to the Retreat Season. 

My findings demonstrate the effectiveness of the Random Forest Regression Model in establishing relationships between diverse features (in my case, Climate Indices in Southern Hemisphere), whether inclusive or exclusive, and the target variable (i.e. SIT). The model proves to be a valuable tool for identifying key drivers of sea ice changes through its feature importance function and facilitates the assessment of the nature of relationships using SHAP Plots. However, it is noteworthy that the model’s performance exhibits significant variations depending on the season and geographical regions. 

Several factors contribute to these results:
1.	As highlighted in the text and illustrated in figures 3-5, climate indices exhibit heterogeneity in their influence on sea ice thickness, varying with season and region. This diversity in the physical reasons leads to different model performances.
2.	The complex and non-linear relationships that these indices share with sea ice thickness might pose challenges for a straightforward Random Forest Regression model to comprehend and establish.
3.	Additionally, the covariability of different features can appear distinct across regions and vary seasonally, causing models to perform well in some instances and poorly in others.

In conclusion, the Random Forest Regression Model indicates that certain regions and seasons present more challenges for modeling than others.
References:
Handcock, M. S., & Raphael, M. N. (2020). Modeling the annual cycle of daily Antarctic sea ice extent. The Cryosphere, 14(7), 2159–2172. https://doi.org/10.5194/tc-14-2159-2020
Hobbs, W., Massom, R., Stammerjohn, S., Reid, P., Williams, G., & Meier, W. (2016). A review of recent changes in Southern Ocean sea ice, their drivers and forcings. Global and Planetary Change, 143. https://doi.org/10.1016/j.gloplacha.2016.06.008
Hosking, J. S., Orr, A., Marshall, G. J., Turner, J., & Phillips, T. (2013). The Influence of the Amundsen–Bellingshausen Seas Low on the Climate of West Antarctica and Its Representation in Coupled Climate Model Simulations. Journal of Climate, 26(17), 6633–6648. https://doi.org/10.1175/JCLI-D-12-00813.1
Kwok, R., & Comiso, J. C. (2002). Southern Ocean Climate and Sea Ice Anomalies Associated with the Southern Oscillation. Journal of Climate, 15(5), 487–501. https://doi.org/10.1175/1520-0442(2002)015<0487:SOCASI>2.0.CO;2
Raphael, M. N. (2004). A zonal wave 3 index for the Southern Hemisphere: ZONAL WAVE 3 INDEX. Geophysical Research Letters, 31(23). https://doi.org/10.1029/2004GL020365
Raphael, M. N., & Hobbs, W. (2014). The influence of the large-scale atmospheric circulation on Antarctic sea ice during ice advance and retreat seasons. Geophysical Research Letters, 41(14), 5037–5045. https://doi.org/10.1002/2014GL060365
Thompson, D. W. J., & Wallace, J. M. (2000). Annular Modes in the Extratropical Circulation. Part I: Month-to-Month Variability. Journal of Climate, 13(5), 1000–1016. https://doi.org/10.1175/1520-0442(2000)013<1000:AMITEC>2.0.CO;2

![image](https://github.com/shreyatrivedi26/shreyatrivedi26.github.io/assets/59626267/bf3a75d6-27ff-4343-982a-32aaa6d19a87)

