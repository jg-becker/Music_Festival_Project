# Music Festival Project 

## Planning

The plan of this project was to aggregate music festival data for music festivals happening around the world in 2020 / 2021. The goal of aggregating this data was to create a structured dataset that could be used for analyzing common metrics about music festivals (location, time of year) in order to see if there were any trends regarding where and when music festivals took place. This project initially started at the beginning of the COVID-19 epidemic, which caused a mass cancellation/postpone of the majority of music festivals in the world. This factor altered the scope of the project, which included adding a music festival status and COVID-19 case component to the dataset. 

## Webscrapping 

The website used for scrapping the data for this project was Jambase.com. This website had a robust catalog of music festival information for 2020 and 2021. Python and the package BeautifulSoup were used to scrape over 2000 music festival entries. For each entry, we got the following data.

* Festival Name
* Status
* Date
* City
* State / Country
* Region

## Data Cleaning


After collecting the music festival data, Pandas was used to structure and clean the data. This processed involved parsing out the location and time data into seperate columns and converting data formats such as acronoyn for state/province location into the full name. The date data was also parsed out into day of the week, month, and year; this structuring would provide more granularity of the analysis. 

## Maintaining Data 

Because the data for the analysis was consistently being updated on the jambase.com website, there needed to be a continual scrape and cleaning of the data. Once this had been completed, the data needed to be merged with prior scrapes of the data and required removing any duplicates from the dataset. 

## COVID-19 Factor

Due to COVID-19 and music festivals being affected, it was decided to incorporate COVID-19 cases by state/province/country into the dataset. This data was acquired using the public World Health Organization data.



