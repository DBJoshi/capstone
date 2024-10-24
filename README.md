# Adverse effects of Covid-19 Vaccination in United States #

## Table of Contents

 1. [Motivation](#1motivation)
 2. [Questions](#2questions)
 3. [Data Sources](#3datasources)
 4. [Data Limitation](#4datalimitation)
 5. [Data Considerations](#5dataconsiderations)
 6. [Challenges](#6challenges)
 7. [Technologies Used](#7technologiesused)
 8. [Conclusion](#8conclusion)
 9. [Future Roadmap](#9futureroadmap)
 10. [Tableau Dashboard](#10tableaudashboard)

## <a name="1motivation"></a> Motivation:

The COVID-19 pandemic has changed the lives of everyone all over the world and placed a strain on science and technology to provide rapid solutions. Vaccination was a pivotal point of pandemic. However, there were many concerns about vaccination which included vaccination mandate, rushed vaccine development, emergency vaccine approval and so on. Being a physical therapist, I was asked many questions by my patients, co-workers and family members. Most of the questions and concerns were about “What could be the Adverse Effects of Vaccination?”. Those who were hesitant to get vaccinated thought, vaccine might have serious adverse effects. There was no data at the time to answer what the adverse effects of covid- 19 vaccination could be. However, after 3 years of vaccine availability, there is enough data to analyze the adverse effects and get some answers.


## <a name="2questions"></a> Questions:

1.	What were these adverse effects seeking medical attention? Which category reported maximum adverse effects? What is the general vaccination adverse effect trend looks like?
2.	Which states reported more cases of adverse effects? Which states reported highest deaths, disabilities, ER visits, Life- threatening events and office visits?
3.	Is there any difference in number of cases reported (adverse effects) by vaccine manufacturer? 
4.	What is the gender distribution of adverse effect cases? Is there any difference in symptoms for females and males?
5.	Which age group reported the most cases in each category? 

## <a name="3datasources"></a> Data Sources:

To answer the above questions, I used the following sources to collect datasets for my analysis:
1.	Vaccine adverse events reporting system:
https://vaers.hhs.gov/data/datasets.html

2.	COVID-19 Vaccinations in the United States, Jurisdiction:
https://data.cdc.gov/Vaccinations/COVID-19-Vaccinations-in-the-United-States-Jurisdi/unsk-b7fc/data

## <a name="4datalimitation"></a> Data Limitations:

According to VAERS website:
* VAERS data are from a passive surveillance system and represent unverified reports of adverse events temporally associated with one or more vaccines. Such data are subject to limitations of under-reporting, simultaneous administration of multiple vaccine antigens, reporting bias, and lack of incidence rates in unvaccinated comparison groups.

* When reporting and evaluating data from VAERS, it is important to note that for any reported event, no cause-and-effect relationship has been established. The event may have been related to an underlying disease or condition, to drugs being taken concurrently, or may have occurred by chance shortly after a vaccine was administered.

## <a name="5dataconsiderations"></a> Data Considerations:

* Data sources were updated on 12/07/2022 and have data till that date. 
* Analysis for gender distribution and quarterly timeline studies, vaccination administration data was not available hence it is showing general pattern across the nation. 
*	Adverse effect cases requiring medical attention were taken in to consideration.

## <a name="6challenges"></a>Challenges:

*	Data normalization was the biggest challenge where the values reported were exceedingly small. To normalize the data, data-frames were divided by total    doses administered and then multiplied by 100,000 and showing the reports per 100,000 doses administered.
*	Analysis and visualization of symptoms containing text was a challenge.

## <a name="7technologiesused"></a>Technologies Used:

*	Python / Pandas - for exploration, normalizing and aggregation of the dataset
*	Tableau - for creating charts and maps
*	Tableau Story - for Presentation 
*	Git – for version control

## <a name="8conclusion"></a>Conclusion:

This analysis of adverse events shows:
*	General vaccination adverse effects trend shows very less numbers of reports for adverse effect cases.
*	Maximum cases were reported in the year 2021 in the first and second quarters and the very few cases in year 2022.
* Maximum cases were reported for office visits, which could be very mild to moderate fever, dizziness, arm- pain, fatigue, headaches; common symptoms and least cases were reported for deaths per 100,000 doses administered.
*	The top five states reporting maximum cases for adverse events were: Kentucky, Michigan, Minnesota, Montana, and Alaska.
*	Among three vaccine manufacturer Janssen reported most adverse effect cases in all six categories and Pfizer reported least cases.
*	Gender study showed that female patients reported more adverse effects compared to males, and symptoms for adverse effects were also more in females.
*	Age group study shows that death, disability, life threatening events and hospitalizations were reported more in the 65+ age group whereas ER visits and office visits were reported more in 18-64 age group.
*	Age group 5-12 and 12-18 reported the least numbers of cases per 100,000 doses administered.

## <a name="9futureroadmap"></a>Future Roadmap:

*	State specific analysis (Michigan and Kentucky): Michigan and Kentucky showed the highest number of adverse effects in 4 subcategories, and it would be interesting to find and analyze this further.
*	Pre-existing medical conditions: Adverse effects might be correlated to pre-existing medical conditions, medications, or allergies and that would be an interesting angle to analyze further.
*	Adverse effects based on Manufacture: It would be interesting to see if there are any specific adverse effects reported more times with a specific vaccine manufacturer.

 ## <a name="10tableaudashboard"></a>Tableau Dashboard:
 https://public.tableau.com/views/Covid-19VaccinationAdverseEffectsinUnitedStates/Presentation?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link




