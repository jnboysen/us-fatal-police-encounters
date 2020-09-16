# us-fatal-police-encounters
## Seattle, where do we go from here? A data driven look at fatal police encounters.

### Motivation:
The death of George Floyd has set-off a chain reaction of anger and frustration across the United States. In watching the officers put their knee on Geroge Floyd I couldn’t help but wonder how often fatal police encounters happen in Seattle. The purpose of this analysis is to answer the following questions related to fatal police encounters in Seattle, and address the current call to defund the police.  

The full Medium blog post on the analysis can be found here: https://medium.com/@jacobsworld/seattle-where-do-we-go-from-here-a-data-driven-look-at-fatal-police-encounters-4917adf67a76


### Questions
1. How many fatal police encounters occur in Seattle annually?
2. How does Seattle compare to other cities?
3. Is defunding the police the right solution?

### Required libraries

1. numpy
2. pandas
3. matplotlib.pyplot
4. matplotlib.style
5. seaborn
6. sklearn.cluster
7. scipy.spatial.distance
8. pingouin
9. sys

### Jupyter notebook files

I separated the code for this project into three notebooks.  If you are only interested in the exploratory analysis then you can jump to Part 3.  Part 1 is the code used to create the clean_city_data_file. Part 2 is the code I used to determine the optimal number of clusters for for the KMeans model.

1. Fatal Police Encounters Part 1 - Motivation and Data Understanding
2. Fatal Police Encounters Part 2 - Data Prep
2. Fatal Police Encounters Part 3 - Train K-Means model
3. Fatal Police Encounters Part 4 - Exploratory Data Analysis

### Data

#### Fatal Police Encounters: 
The data on police fatal encounters comes from an independent database made available by fatalecounters.org. The data source includes fatal police encounters since January 1st, 2000, and contains both intentional use of force and unintentional incidents like suicide or vehicle pursuit. 

1. File: fatal_encounters.csv
2.  Reference Link: https://fatalencounters.org

#### 2020 City Population + 2017 Census: 
The variables required for this analysis required me to pull data together from multiple sources. The data is a combination of 2020 city population data, 2017 US census data by county, and 2018 stats on the number of police officers active in each city department. 

#### 2017 Census Data
1. File: census_data_2017
2. Reference Link:https://www.kaggle.com/muonneutrino/us-census-demographic-data

#### Top 200 Cities
1. File: city_population.csv
2. Reference Link:https://worldpopulationreview.com/us-cities

#### 2018 Full-time Law Enforcement Employees
1. File: police_departments_2018.csv
2. Reference Link: https://ucr.fbi.gov/crime-in-the-u.s/2018/crime-in-the-u.s.-2018/tables/table-78/table-78.xls/view

#### Output of Part 1 - Data Prep
1. File: clean_city_data.csv

## Summary of Finding

Policing in the United States is a complex topic that needs to be addressed. Data can be a powerful mechanism for change; a way to shine a light what’s working, and what’s not working.

This exploratory analysis provides us some insight into the long-term trends of encounters with Seattle police that turn fatal. With an average of 2.7 fatalities per year, Seattle ranks 2nd out of 6 similar cities across the U.S. That rate is 2x the rate of Nashville but 70% less than the Denver. While positive, we can also see that Seattle’s average rate hasn’t change significantly in the last 20 years.

Is defunding the police the right decision? An answer to this question requires a more robust analysis, however the low correlation between the two variables and the dispursion of fatalities should give us pause. There appears to be little evidence that defunding the police will significantly change the fatality rate of encounters with police.


## Acknolwedgment
A special thank you to fataleoncounters.org for collecting ad making the data on fatal police encounters available. The insight gained from this analysis would not be possible without your the data you've made available. Also, thank you to Udacity.com, Simon Storey, and Jess Estrada for providing feedback on both the technical elements and summary of findings.
