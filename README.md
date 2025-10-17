# Dashboard_Excel_Personal_Rotation_Case_Study

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning / Preparation](#data-cleaning--preparation)
- [Initial Analysis](#initial-analysis)
- [Dashboard – Initial Steps](#dashboard--initial-steps)
- [Slices](#Slices)
- [Further Document Analysis](#further-document-analysis)
- [Results/Findings](#results-findings)

## Project Overview 

### Case Study
You are a newly hired analyst for the human resources department at SelvaCongo.com, a company that sells everything online. They currently have a problem with how information about the hiring and firing of their warehouse staff across the country is displayed. The previous analyst had to prepare PowerPoint reports for more than 100 different managers and department heads, which
took up more than half of their time each month. SelvaCongo.com is also concerned about its staff turnover rates and wants managers to have this information at their fingertips so they can reduce them below the industry average.
The company has decided to invest in a new software solution to automate this process. 

### Task 
To create an interactive dashboard-style report that shows the most important indicators for the company. The dashboard must be useful for all managers and department heads.


At a minimum, the dashboard must show: At a minimum, the dashboard should include:
- Amount of hired staff
- Number of located staff/performance as a percentage of hired staff
- Number of released staff/performance as a percentage of hired staff
- Staff turnover rate (defined as departures over hired staff)
- 2 graphs
- 2 segmenters
- 1 table

## Data Sources

- Contratacion_Almacenes_Mex.xlsx
- Escenario y Documentos.pdf

## Data Cleaning / Preparation
- Gather three dirty tables into one normalized tables
- Fix wrong data dates like typo date errors. Remove possible duplications through a quick dynamic table validation.

## Initial Analysis
- For the four points requested (hired staff, located staff, released staff and turnover) we worked with dynamic tables to get the sum of these employees within each category.
- Then, proceeded to obtain the percentage of each of these staff indicators.

<img width="550" height="548" alt="image" src="https://github.com/user-attachments/assets/8f7543e8-24b6-43da-aae4-33640426b726" />

## Dashboard – Initial Steps
- New worksheet named Dashboard. Here we will work with the Dashboard to show the report requested
- Insert Forms and textboxes.
- Inserting the four indicator names, referencing the numbers and percentages from the Analysis worksheet.
- Modifying color, outline and shadows at will
  
<img width="1044" height="540" alt="image" src="https://github.com/user-attachments/assets/1458351a-6a31-49dc-bdda-e749fff0274e" />

## Slices
- Create two slicers taking reference the Analysis worksheet data; one slicer for Area, and one for Almacén "Warehouse".
- Change color, column quantity, and other specs at will
- Mark "Remove blank data" box, from "Slice Data Configuration" at Slicer ribbon
  <img width="573" height="433" alt="image" src="https://github.com/user-attachments/assets/e9cc0adf-939c-421a-9226-79541483c839" />
- Reference our tables to the slices marking the tables checkboxes on "Report Connections" at Slicer ribbon
  <img width="352" height="270" alt="image" src="https://github.com/user-attachments/assets/698b8dc2-b730-45e3-b2ed-6d4a61521c31" />  

- Cut and copy the tables to our Dashboard
  <img width="1678" height="485" alt="image" src="https://github.com/user-attachments/assets/56dac79e-ee5d-430f-8cd3-4cdc7ba3f102" />

## Further Document Analysis
Exploring the documents, there are two important sections where we are provided extra information to help generate ideas and include if a data is valuable to present. We have found the following: 

  - National Staff Average Turnover. This data is presented as a news arcticle, redacting the increase in criminality inside the country, specially during the night time, where people are afraid to commute during those hours, where the valuable data to extract is the mentioned day and night average turnover reported by a national organism, implying this is the national average staff turnover.
      
  | Shift | Percentage |
  |:-------|-----------:|
  | Night  | 68% |
  | Day  | 23% |
      
  - Hiring Number of Staff from our competition "Manchester Stores". Present as an email coming from a superior providing important insights about the hiring staff that our competition has hired during the first semester of 2017. The messager closes with the importance as our company goal to mantaina  higher number above our competition. Their staff hiring personal is the following:

  | City | Staff Hired |
  |:-------|-----------:|
  | CDMX  | 200 |
  | Ecatepec  | 50 |
  | Guadalajara  | 100 |
  | Zapopan  | 50 |
  | Monterrey  | 200 |
  | Puebla  | 40 |
