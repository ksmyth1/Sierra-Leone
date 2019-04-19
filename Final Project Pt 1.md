# Sierre Leone

Final Project - GA Part-Time Data Science Course 2018 

# Background & Research

---

Sierra Leone is a small country on the coast of West Africa.

![](ScreenShot2018-10-11at6-585ac592-90a5-4366-acdb-8067cd1f80cd.21.26pm.png)

I went to Africa in 2017 and saw first hand the incredible potential of the countries and the people  there, as well as many of the challenges. I found a dataset online about AID spending on projects in Sierra Leone between 1992 and 2014. By analysing the relationship between this data, and other freely available data regarding the countries performance on human development indicators in those years, I may be able to find some relationship between certain sectors and years of AID, and outcomes in human development. 

Dataset 1:

![](34B33DC2-0D25-4BD2-ACA9-5B5EFD357640-60ebb799-2693-447c-ac45-1976e4bf3945.png)

Source:

[AidData | Sierra Leone AIMS Geocoded Research Release, Version 1.0](https://www.aiddata.org/data/sierra-leone-aims-geocoded-research-release-level-1-v1-0)

Summary:

Geocoded projects from the Development Assistance Database (DAD) Aid Information Management System (AIMS) managed for Sierra Leone. This dataset tracks 856 projects across 2314 locations, $3,340,138,954.00 in geocoded commitments, and $2,785,175,978.00 in geocoded disbursements between 1992 and 2014.

Dataset 2: 

Pending, HDI data between 1992 and 2014 for Sierre Leone. 

# Questions?

---

1. What proportion of disbursed AID dollars were given to various sectors of the country overall?
2. Which years contain the most amount of disbursed AID dollars?
3. What are the trends over time, by sector? 
4. How has Sierra Leone been tracking in various human development indicators throughout those years, what are the trends over time, by area? 

# Hypotheses

- Null hypothesis: There is no relationship between amount spent on projects by year, per sector, and the countries performance on related HDI indicators
- Alternative hypothesis: There is some relationship between amount spent on projects by year, and sector, and the relevant countries performance on related HDI indicators
- Does AID go to the areas that Sierre Leone is ranked weakest on in HDI indicators? Does more money to certain sectors have a correlation to scores in relevant indicators?
- Confounder 1: Time Lag. There may be a negative relationship due to the time lag involved, i.e. more project money may go into an area as it’s getting ‘worse’ in order to try an improve it, making it look like there is a negative relationship between the money and the indicator. Alternatively if there’s not as much time lag, the money may have a positive relationship with indicators, showing that it is helping immediately.
- Confounder 2: Correlation vs Causation. If, for example, Sierre Leone's HDI indicators improved over the time period, and the project funding also increased over the time period, it may not mean that the project funding caused the HDI improvement. Both aspects could have been influenced by a third factor, such as improvements in the global economy and technology.

# How?

---

1. Import packages
2. Import Sierre Leone project data
3. EDA on project data
4. Import HDI data
5. EDA on HDI data
6. Sum the Sierre Leone project data by year across the sectors (i.e. pivot table) 
7. Combine the summarised project dataframe with the HDI indicator dataframe
8. Perform 2D linear regressions across sectors to determine positive, neutral or negative relationships
9. If time permits, build in ’time lags’ to the year column, to see if adding 1 or 2 years between the projects and the indicators results in more positive relationships
10. Establish conclusions

# Requirements

---

- [x]  Acquire Sierre Leone project data 1992-2014
- [x]  Acquire HDI data for Sierre Leone 1992-2014