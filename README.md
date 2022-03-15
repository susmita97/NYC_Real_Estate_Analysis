# NYC_Real_Estate_Analysis

ABSTRACT

There is no denying that New York is one of the most expensive places to
own or rent a place. The ever-blooming economy and a cultural epicenter of
the world make it one of the most competitive cities in the world. In this
context, our project aims to perform some descriptive analysis on the real
estate data from New York and utilize machine learning models to predict
future prices. In addition to this, we also have attempted to determine the
average income of millennials to afford those properties. We hope our work
helps readers who aspire to own a place in New York to make informed
decisions.

DATA ACQUISITION AND CLEANING

NYC Real Estate has always been a popular topic of discussion, with prices
rising high at a rate of a minimum of 10% every year. Hence, moving
forward, we acquired publicly available data to analyze the reasons for the
percentage increase every year. We obtained a dataset called Rolling Sales
from NYC Open Data for 2016-2020, which consisted of the following
columns and information.

We firstly went through each of the 25 data files and explored the data. We
quickly realized that while the order of the information contained in each
column remained the same, the column names differed a little in the files year
by year. The data was available separately for each of the boroughs for every
year, and as that proved to be useful for us for analysis of some of the tasks,
we still had to combine and clean the data a lot for the rest of our study. We
firstly went through each of the 25 data files and explored the data. We
quickly realized that while the order of the information contained in each
column remained the same, the column names differed a little in the files year
by year. This method, however, was causing a problem while concatenating
all the data in one dataframe and giving us an inconsistent dataframe.
After we merged all the data, as the next step, we checked for NaN and null
values, especially on the ‘SALE PRICE’ column, as we had to build a
predictive model for predicting future prices. We used the dropna() and
isnull() functions for this purpose. Furthermore, when we checked the unique
values for each column, it consisted of ‘-’ values for most of the rows that
indicated missing data. There were a lot of missing and invalid data types
present in the data, which we took care of during data preparation.
We were curious about how much the property’s surroundings affected its
price, and this data was not present in the rolling sales dataset. Therefore, we
used the publicly available Real Estate Investment Trust (REIT) data.
Fortunately, this dataset’s data preparation was not as time-consuming for the
rolling sales dataset as most data was already preprocessed.

ANALYSIS

1. Which are the most popular and highly-priced neighborhoods in all
the five boroughs of NYC?
To get started with this analysis, we began by exploring which neighborhoods
were the most expensive in all the boroughs yearly, as it can be seen below.
When we checked the number of sales, the areas in Midtown Manhattan and
Upper East and the West dominate the majority of all property sales, with the
Upper East Side(59-79) having the most number of sales for the years 2017,
2018, 2019 and the Midtown West in 2016 and Upper West Side in 2020.
However, Midtown West has consistently had expensive property rates with a
positive increase in percentage rate over the five years which can be seen in
the last graph where we combined the data for all the five years. The graphs
show all the sales for all the neighborhoods and the prices are shown in
millions of dollars. A recently published article by TimeOut says that Tribeca
and Hudson Yards are two of the five most expensive neighborhoods in
Manhattan in 2021, which are in Midtown West. This is consistent with our
analysis that Midtown West has most of the expensive properties in
Manhattan alongside the Upper East and West Sides.

![alt text](https://github.com/susmita97/NYC_Real_Estate_Analysis/tree/main/images/q1/Manhattan Prices Comparision 2016))

![alt text](https://github.com/susmita97/NYC_Real_Estate_Analysis/tree/main/images/q1/Manhattan Prices Comparision 2017))

![alt text](https://github.com/susmita97/NYC_Real_Estate_Analysis/tree/main/images/q1/Manhattan Prices Comparision 2018))

![alt text](https://github.com/susmita97/NYC_Real_Estate_Analysis/tree/main/images/q1/Manhattan Prices Comparision 2019))

![alt text](https://github.com/susmita97/NYC_Real_Estate_Analysis/tree/main/images/q1/Manhattan Prices Comparision (2016-2020))

