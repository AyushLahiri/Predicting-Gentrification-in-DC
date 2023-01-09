# Predicting-Gentrification-in-DC
## Washington was nearly half Black by the mid-20th century, and more than 71 percent by 1970, between the 2000 and 2020, accoring to the U.S. Census, the city’s Black population dropped from 59 to 41 percent. Today, D.C. has one of the highest rates of displacement in the country.Low-income residents are being pushed out of neighborhoods at some of the highest rates in the country, according to the Institute on Metropolitan Opportunity. Most of the people pushed out of these economic hot spots are black and low income, according to the data. In lieu of this explosive issue that faces DC, I sort ought to find whether we can predict which areas in DC are getting gentrified and more importanly "will" be gentrified. 

## Execution
 - Obtain a census API key: https://api.census.gov/data/key_signup.html
 - Run notebooks in the following order 
    1. `Data_preparation.ipynb`
    2. `Hierarchical_clustering.ipynb`
    3. `Random_Forest.ipynb`
  
## Gentrification 
Gentrification is a legacy of historical patterns of residential restructuring that trace back to the start of the 20th century. The end of World War II marks a mass exodus of affluent, white households from urban areas to the suburbs. The “white flight” movement was reflective of the preferences, policies, and market conditions throughout the fifties and sixties. Specific factors including systemic racism, redlining, municipal disinvestment, and the construction of the federal highway system helped to systematize the suburban movement (Zuk et al., 2015).Throughout the 1980’s gentrification was referred to as a “localized small scale process…purely temporary and of little long-term significance.” As we are well aware now over the previous fifty years, gentrification is neither temporary nor is it exclusive to the United States. 

While there is much debate on the definition of gentrification, the general patterns from a spacial point view does provide a succint definition: A sustained period of disinvestment, followed by an influx of investment and wealthier residents, in some cases correlated with race,  that results in the displacement of existing residents

## Data 
American community survey's 5-year estimates(2012-2021): https://www.census.gov/data/developers/data-sets/acs-5year.html



## The problem 
Before proceeding with using supervised learning algorithms , to predict gentrification in DC, we face a fundamental problem. i.e. WHAT IS GENTRIFICATION. 
The answer to this complex, frequently disagreed upon and one dimensional. We therefore intend to this problem through unsupervised learning, to generate our own classification of gentrification.

## Methodology 
There primarily exists three definitions in the literature to identify gentrification. Summarized below 
These definitions while rather different from one another, also fail to characterize the socio-economic complexities that exist in the context of gentrification. While neither unimportant, their discreet sensitive values and inability to capture the problem on multiple dimensions makes them sub-optimal methods of classification. 
I therefore use these definitions in tandem with clustering, a type of unsupervised machine learning technique used to distinguish underlying patterns and similarities among multiple features. In the context of urban change, it can be used to distinguish the dominant trajectories of neighborhood change over time. 

Clustering techniques bypass many of the limitations and bias of traditional threshold-based methods. Clustering methods optimize the homogenous subgrouping from the data itself, rather than from a predetermined framework. They also afford the inclusion of additional variables that are able to
capture the multi-dimensionality of neighborhood change. These methods are also less biased than
their prescriptive counterparts. 


