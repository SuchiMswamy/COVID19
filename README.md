# About COVID19 Analysis (beta)
Packages used:
*1. covid19.analytics: The "covid19.analytics" R package allows users to obtain live worldwide data from the novel CoronaVirus Disease
*2. devtools


**Data Accessibility**
The covid19.data() function allows users to obtain realtime data about the CoViD19 reported cases from the JHU's CCSE repository, in the following modalities:

1. "aggregated" data for the latest day, with a great 'granularity' of geographical regions (ie. cities, provinces, states, countries)

2. "time series" data for larger accumulated geographical regions (provinces/countries)

3. "deprecated": we also include the original data style in which these datasets were reported initially.

The datasets also include information about the different categories (status) "confirmed"/"deaths"/"recovered" of the cases reported daily per country/region/city.

This data-acquisition function, will first attempt to retrieve the data directly from the JHU repository with the latest updates. If for what ever reason this fails (eg. problems with the connection) the package will load a preserved "image" of the data which is not the latest one but it will still allow the user to explore this older dataset. In this way, the package offers a more robust and resilient approach to the quite dynamical situation with respect to data availability and integrity.


|Argument                   | Description                                                   |
|:-------------------------:|:-------------------------------------------------------------:|
|aggregated                 | last number of cases by country                               |
|ts-confirmed               | data of confirmed cases                                       |
|ts-deaths                  | data of fatal cases                                           |
|ts-recovered               | time series data of recovered cases                           |
|ts-ALL                     | all time series data combined                                 |
|ts-dep-confirmed           | time series data of confirmed cases as originally reported    |
|ts-dep-deaths              | time series data of deaths as originally reported             |
|ts-dep-recovered           | time series data of recovered cases as originally reported    |
|ALL                        | all of the above                                              |
|Eg: ts-Germany             | time series data of confirmed cases for the city or country   |

