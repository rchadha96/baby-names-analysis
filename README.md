# Baby Names 
Project Goal: To perform Exploratory Data Analysis on Baby Names in Ireland over a 54-year period using R

* Analysed popularity of baby names trending over time by assigning ranks according to the number of births and deciphered high-ranking names from 1964 to 2018 using packages like ggplot2, plotly and tidyverse.
* Successfully identified a downward trend for gender neutral names like Robin, Ríonach and Dillon, leading to inferring gender specific names as current trend.
* Worked with Regular expressions package ‘stringr’ to find popular baby names by letter and grouping them based on different parameters for further analysis.

## Data Exploration

![residvsfit](/images/residualvsfit.png)

### Hypothesis Testing and checking for normality

We perform t-test for rank of the baby names to check if the mean of the sample from a normal distribution has a specific value i.e. if all the means are same. We consider null hypothesis as all the means of the sample being the same and alternate hypothesis as not all means are equal. As in t-test, it is assumed that the data is normally distributed, we confirmed it with the density- curve which tells us if the graph is bell-shaped or not. Bell-shaped curve represents data is normally distributed. Here, we can safely assume Normal Distribution. Here, we could see that p–value from t-test is than 0.05 which is 2.2*10^(-16) so we reject the null hypothesis and accept the alternate hypothesis which means that sample mean is not equal to the theoretical mean. As per Q-Q plot, we could see that the curve shows the hints of normality. There are few outliers in the plot and it might need transformations to attain ideal Normality.

![DensityPlot](/images/desnity_plot_rank.png)

## Analysis of Girl & Boy Names
### Data Visualisation
What are the top baby girl names over the time period of time? Identifying the top 15 baby girl names according to the rank and number of births.

![top_girlnames](/images/top_girlnames.png)

Trend of Mary, Emma & Sarah over Years by their rank and births

I have used top names, Mary & Sarah (respective to number of births), Emma and Sarah (respective to number of ranks) over the years. We could see the trend of Mary and Emma is decreasing while sarah is nearly constant over years. Could we conclude the most popular names in the early years are not so popular as of now ?

![comparison_girls](/images/comparison_girls.png)

What are the top baby boy names over the time period of time?

Identifying the top 15 baby girl names according to the rank and number of births.

![top_boynames](/images/top_boynames.png)

Trend of James and Michael over Years by their rank and births

I have used top names, James and Michael (respective to number of births and ranks) over the years. We could see the trend of James and Michae is increasing according to number of births while James is nearly constant and Michael is again decresing over years accoriding to rank.

![comparison_boys](/images/comparison_boys.png)

### Trend of Common Names
Robin is the most common name used among babies of both genders. The below trend is the evident that the use of robin for girl babies has increased over time. Where as it has declined for boby babies

![common_babynames](/images/common_babynames.png)

### Popular Baby Names By Letter
Due to popular baby names such as Adam, Ava, Aoife, Aarom and Alan from the dataset, the letter A takes first place. The second place of first letter baby name is C with names such as Conor, Chloe and Catherine.

![names_byletter](/images/names_byletter.png)

## Summary
In the Data Exploration section the mean was suprising low compared to number of births per year and the girls names are more spread than the boys.The analysis of baby names in Irealnd from 1964-2018 tell us that there is an increase in the number of unique names over the years.Also, the names which were popular in 1964 have declined in follwing yeras with respect to rank ( example : baby name MARY).



