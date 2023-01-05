---
layout: project
type: project
image: images/USairline.jpg
title: "US Commercial Aviation Industry Insight"
# All dates must be YYYY-MM-DD format!
date: 2022.10 - 2022.12
published: true
projecturl: https://github.com/TaikiShuttle/SI618
labels:
  - Data Science
  - Large Scale Data Computation
  - Machine Learning
summary: "A series of projects aiming to give insights to the current US commercial aviation industry. As an aviation lover, I also tried to make my naive suggestions to airline companies."
---

Traveling by airplane is one of the most common modes of transportation for the US dwellers. Compared with countries like Japan and China, which have a high population density, the distribution of the population in the US is quite sparse and thus not suitable for developing a high speed railway network. However, the US also enjoys a huge land area, spanning from the Pacific Ocean to the Atlantic Ocean, which makes long range transportation a necessity for the US citizens. Throughout the history of the US, airplanes have thus been playing the essential role of long distance transportation. 

Due to its popularity, large scale data sets are provided by [the US Department of Transportation](https://data.transportation.gov/) for data scientists to retrieve and analyze. These large scale data sets, which usually contain millions of records, cover a variety of commercial aviation related topics, including: departure records , airfare records, flight delay records, and airline financial reviews. Valuable information can thus be discovered from the data set and transformed into useful suggestions for stakeholders to consider.

Inspired by the motivation mentioned above, this project series use several data sets to answer questions about the US aviation industry. In general, it can be divided into two parts.

## Project Part 1: Recovery of the US Commercial Aviation Industry after COVID: An International View

##### Background

I have been hearing from famous aviation YouTubers like Sam-Chui that the aviation industry is having its toughest years since the COVID pandemic. But I have never looking at the details by myself. Instead of just believing it to be true, I think analyzing it by myself can convince myself better. As a crazy aviation fan, I want to get some insights to the current aviation industry.

##### General Information

In this project, I am trying to analyze the US commerical aviation industry situation after 1990. I am trying to ask myself following questions:
1. What is the impact of COVID on the US commercial aviation industry?
2. Has the US commercial aviation industry recovered completely from the COVID pandemic?
3. Is there any significant structural change made by the COVID pandemic to the US commercial aviation industry?

   a. Is there a significant change in top international destinations considering the flights departed from the US?
   
   b. Is there a significant change in US airports rank considering the flights departed from the US?
   
   c. Is there a significant change in top airline carriers considering the flights departed from the US?

4. What are the current operating conditions of the US commercial aviation industry? Does the accident rate increase?
5. When will the US commercial aviation industry reach the scale before the COVID pandemic?
6. ...

I hope that by answering these questions, I can know the aviation industry better. And if possible, give my naive suggestions to airline carriers to help them go through this tough period.

##### Data Used

The major data set used here is the <a href="https://www.transportation.gov/policy/aviation-policy/us-international-air-passenger-and-freight-statistics-report">International Departures</a> published by the Department of Transportation. There are also some relatively minor data sets including

1. <a href="https://www.kaggle.com/datasets/deepcontractor/aircraft-accidents-failures-hijacks-dataset?resource=download">Aircraft Accidents, Failures & Hijacks Data set</a> provided by Kaggle
2. <a href="https://github.com/mwgg/Airports">Airport codes</a>
3. <a href="https://en.wikipedia.org/wiki/List_of_airlines_of_the_United_States">US Airport codes</a>
4. <a href="https://www.bts.gov/topics/airlines-and-airports/airline-codes">Airline codes</a>
5. <a href="https://gist.github.com/stevewithington/20a69c0b6d2ff846ea5d35e5fc47f26c">Country and Continent Lists</a>

##### Manipulation & Visualization Tools

NumPy, Pandas, PySparkSQL, Seaborn

##### Report

The major analysis code is <a href="https://github.com/TaikiShuttle/SI618/blob/main/Project1/aviation_preprocess.ipynb">this Jupyter Notebook</a>.

The report is <a href="https://github.com/TaikiShuttle/SI618/blob/main/Project1/si618-project-part-1-haoquanz.pdf">here</a>.



## Project Part 2: US Domestic Airline Consumer Airfare: an Inter-City Analysis

##### Background

As mentioned above, traveling by airplane is one of the most common transportation methods used in the US. As a consequence, the airfare problem becomes an important topic widely discussed by the US citizens. How to buy tickets with reasonable prices is important for money-saving. But this is not an easy task. Since the airfare is influenced both by inner factors like distance and outer factors like market situation. In this project, we want to explore which factors influence the airfare significantly, and try to use them to predict the airfare precisely.

##### General Information

In this project, the US domestic airline consumer airfare will be analyzed closely based on an inter-city view. The prices of flights between US major cities will be collected and inspected. In particular, there are three overarching questions covered by this project:

1. What is the overall trend of US domestic airfare after 1990s?
2. What factors determine the airfare between two cities?
3. Can we predict the airfare based on given information?

##### Data Used

The major data set used here is the [Consumer Airfare Report](https://data.transportation.gov/Aviation/Consumer-Airfare-Report-Table-1-Top-1-000-Contiguo/4f3n-jbg2) published by the Department of Transportation.

##### Manipulation & Visualization Tools

Numpy, Pandas, Plotnine, Seaborn, SkLearn

##### Report

The major analysis code is [this Jupyter Notebook](https://github.com/TaikiShuttle/SI618/blob/main/Project2/si618_project2_EDA.ipynb).

The report is [here](https://github.com/TaikiShuttle/SI618/blob/main/Project2/si618-project-2-haoquanz.pdf).
