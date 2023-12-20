# 17-The-determinants-of-cyberattack-costs-An-event-study

## Goal
This study aims to compute the impact of different types of cyber attacks on firms' stock prices.
------
## Abstract
Along with the increasing frequency and severity of cyber incidents, understanding their economic implications is paramount. In this context, listed firms' reactions to cyber incidents are compelling to study since they (i) are a good proxy to estimate the costs borne by other organizations, (ii) have a critical position in the economy, and (iii) have their financial information publicly available. We extract listed firms' cyber incident dates and characteristics from newswire headlines. We use an event study over 2012--2022, using a three-day window around events and standard benchmarks. We find that the magnitude of abnormal returns around cyber incidents is on par with previous studies using newswire or alternative data to identify cyber incidents. Conversely, as we adjust the standard errors accounting for event-induced variance and residual cross-correlation, we find that the previously claimed significance of abnormal returns vanishes. Given these results, we run a horse race of specifications, in which we test for the marginal effects of type of cyber incidents, target firm sector, periods, and their interactions. Data breaches are the most detrimental incident type with an average loss of -1.3\% or (USD -1.9 billion) over the last decade. The health sector is the most sensitive to cyber incidents, with an average loss of -5.21\% (or USD -1.2 billion), and even more so when these are data breaches. Instead, we cannot show any time-varying effect of cyber incidents or a specific effect of the type of news as had previously been advocated.

------
## Documents
For more information please refer to:


------
## Code

The code is a mix of notebooks and a `py` file: 
- the _py file_ contains the functions needed in the notebooks;
- the _notebooks_ explain all the steps.


**Data**:


Stock information from [WRDS](https://wrds-www.wharton.upenn.edu/).


------
## Files description:

Short description of the files:

| File name        | Short Description  |  
| ------------- |:-------------:| 
| function_definitions.py | defines of all the functions used in the other files |
| event_study_prc.py | analyses and processes the cyber breach dataset from [Privacy Rights Clearinghouse](https://privacyrights.org/data-breaches) |
| event_study_refinitiv.py | merges of the Refinitiv news data with the stock information data |
| event_study_CAR_OLS.py | estimates CARs with OLS and the associated t-test statistics |
| event_study_CAR_SURE.py | estimates CARs with SURE and the associated t-test statistics |
| event_study_analysis.py | presents regressions of CARs on firm and breach characteristics and computes descriptive statistics on the price of cyber incidents |

Each file contains more details and comments. 



------
## Hints of bibliography:

Please find the complete list on the bibliography of [the master thesis](Cyber_risk_thesis.pdf). 

