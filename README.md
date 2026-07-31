# Course-2-Data-Analytics-Using-Python
In ‘Data Analytics Using Python’, we learned an extensive scope of Python, applying code across the Pandas, Numpy, Seaborn and Matplotlib libraries. 
Foundational theory included Python data structures, core functions, control flow expressions and the DateTime module. By the end of the course we had attained a skillbase in Data Wrangling, Data Visualisation, Scraping and even Sentiment Analysis.
This course was a far greater application of visualisation and trend analysis, using python.

Please find the <a href='https://github.com/jameshparmenter/Course-2-Data-Analytics-Using-Python/blob/main/Parmenter_James_DA201_Assignment_Report%20(1).pdf'> full report above.</a>

<b>Grade: 64% *</b>
'* Grade impacted significantly by a family bereavement

## The Assignment:

For the assignment, we used trend analysis to make recommendations to the NHS regarding the strategy, feasibility and costs associated with expanding services.

## Building Context

First, it was necessary to define the importance of the task and problem statement: 
<ul>
<li><i>‘The National Health Service (NHS) is the UKs public healthcare provider and is both essential to the welfare of UK citizens and part of the fabric of the UK’s identity.’</i></li>
<li><i>‘This analysis utilises the provided datasets to suggest actions in response to the questions posed by the NHS regarding adequate staffing, capacity and resource utilisation.’</i></li>
  </ul>
Very early in the NHS report, I question the usefulness of the data collection, important for building informed business recommendations.
<i>‘As analysts, we also ask our own questions and challenge the usefulness of the data.’</i>

## Analytical Approach
The three datasets were of medium size consisting of X variables and X observations. The first step was to import pandas and numpy, alongside the datasets, so we can explore the data and perform descriptive statistics. We found:
<ul>
<li>Missing values: There were no missing values</li>
<li>Mapping: We decide to not map ‘Other’ or ‘Unmapped’ as this will assist in our assessment as to the quality of the dataset</li>
<li>Timeframe: The datasets only shared data over a period of 18 months. </li>
<li>We then completed transformations to aid in analysis and visualisation:
‘...dividing appointment count by 1000 to make the Y axis of visualisations legible and we transform ‘Appointment_Status’ into a percentage to measure the percentage of appointments attended. Lastly, research found that on average a missed NHS appointment costs the NHS £30, thus we use this to monetise missed appointments.’</li>
  </ul>

## Timeseries Analysis
Our time series analysis produced visualisations to give time context and prove trends in data. We installed seaborn and matplotlib, completed final groupings and then visualised the month on month capacity trends.


<img width="400" alt="NHS1" src="https://github.com/user-attachments/assets/4d74edac-3cf1-41e5-9ecc-3a58749cd701" />

<img width="400" alt="NHS2" src="https://github.com/user-attachments/assets/8f57d4ba-882e-466d-b58f-703e99ec8ffb" />

<img width="400" alt="NHS3" src="https://github.com/user-attachments/assets/0677c349-ba5f-4f71-a745-34596b6d2783" />


We find the observations are dominated by a few categories: ‘General Consultation’ (Service Settings), ‘Care Related Encounters’ (Context Types) and ‘General Practice’ (Grouped National Categories), all peaking at the same time - October and November 2021.
Sentiment Analysis

We performed sentiment analysis, installing the XXX libraries and and twitter dataset to collect supporting qualitative feedback on the NHS. 

Here, we preprocessed the data, lowercasing, removing noise, tokenising and removing stop words. We grouped certain words by health themes to reduce the noise in the analysis and then presented a count of the most frequent hashtags / their themed groupings. Here we found ‘Covid’ related hashtags to be the most significant.

We dropped ‘retweet’ and ‘favourited’ tweet analysis as this was mainly advertising and entertainment content.

## Capacity & Utilisation Analysis

For the core of the analysis , we produced several visualisations, ranging from stacked bar chats, linegraphs and boxplots.

<img width="400" alt="NHS4" src="https://github.com/user-attachments/assets/4e484d3b-2ea5-47b1-8e6f-1d0e4ac88ed7" />

<img width="400" alt="NHS5" src="https://github.com/user-attachments/assets/8000bf2f-7b90-4a86-91cc-e6a2a97feb1b" />

<img width="400" alt="NHS7" src="https://github.com/user-attachments/assets/41fb619e-9dea-4444-937a-018d74e26f15" />
<img width="400" alt="NHS6" src="https://github.com/user-attachments/assets/6f2459c8-e9ac-4699-8b26-0e168decec9f" />

<ul>
<li><i>‘Lineplots present findings on staff level utilisations where it peaks at 85% in October and November’</i></li>
<li><i>‘The appointment type split remains proportionate across the busiest months’</i></li>
<li><i>‘General Practice has the widest range and highest level of outliers’</i></li>
<li><i>‘The Appointment Type with the highest Attended Rate was ‘Telephone’ (~95%) and the lowest was ‘Home Visit’ (~75%)’</i></li>
</ul>

## Notable Patterns, Trends and Recomendations
In recommendations, we mainly challenge the usefulness of data covering only one full calendar cycle, and one that is applied in a pandemic. 
<ul>
<li><i>‘...there is a consistent increase in appointments in the months of October, November which we hypothesise to be from the natural downturn in weather’</i></li>
<li><i>‘ [A backlog of appointments in] …March, due to a backlog of appointments from the Omicron Covid-19 variant.’</i></li>
<li><i>‘the next step would be to mimic this analysis across several years of data to account for a period where the data is not influenced by a worldwide pandemic’</i></li>
<li><i>‘We also recommend improving data collection to reduce the number of ‘Unknown’ data records.’</i></li>
<li><i>‘Our core recommendation is to move more appointments to video / online to help save the NHS money in missed appointments’</i></li>
</ul>
