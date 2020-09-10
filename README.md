# us-fatal-police-encounters
## Seattle, where do we go from here? A data driven look at fatal police encounters.

### Motivation:
The death of George Floyd has set-off a chain reaction of anger and frustration across the United States. In watching the officers put their knee on Geroge Floyd I couldn’t help but wonder how often fatal police encounters happen in Seattle. The purpose of this analysis is to answer the following questions related to fatal police encounters in Seattle, and address the current call to defund the police.  The full Medium blog post on the analysis can be found here: https://medium.com/@jacobsworld/seattle-where-do-we-go-from-here-a-data-driven-look-at-fatal-police-encounters-4917adf67a76


### Questions
1. How often do people engage with police and end up dead? I
2. Is this common, and how do we compare to other cities like Chicago, Portland, or Denver? 
3. Is defunding the police the right course of action?

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

### Jupiter notebook files

I separated the code for this project into three notebooks.  If you are only interested in the exploratory analysis then you can jump to Part 3.  Part 1 is the code used to create the clean_city_data_file. Part 2 is the code I used to determine the optimal number of clusters for for the KMeans model.

1. Fatal Police Encounters Part 1 - Data Prep
2. Fatal Police Encounters Part 2 - Train Kmeans model
3. Fatal Police Encounters Part 3 - Exploratory Analysis

### Data

#### Fatal Police Encounters: 
The data on police fatal encounters comes from an independent database made available by fatalecounters.org. The data source includes fatal police encounters since January 1st, 2000, and contains both intentional use of force and unintentional incidents like suicide or vehicle pursuit. 

> File: fatal_encounters.csv
> Reference Link: https://fatalencounters.org

#### 2020 City Population + 2017 Census: 
The data I was looking for by city required me to pull and join data from multiple data sources. The data is a combination of 2020 city population data, 2017 US census data by county, and 2018 stats on the number of police officers active in each city department. 

#### 2017 Census Data
> File: census_data_2017
> Reference Link:https://www.kaggle.com/muonneutrino/us-census-demographic-data

#### Top 200 Cities
> File: city_population.csv
> Reference Link:https://worldpopulationreview.com/us-cities

#### 2018 Full-time Law Enforcement Employees
> File: police_departments_2018.csv
> Reference Link: https://ucr.fbi.gov/crime-in-the-u.s/2018/crime-in-the-u.s.-2018/tables/table-78/table-78.xls/view

#### Output of Part 1 - Data Prep
> File: clean_city_data.csv
