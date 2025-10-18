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
- [Final Dashboard](#final-dashboard)
- [Results/Findings](#results-findings)

## Project Overview 

- The aim of this practice is to refine key concepts of data analysis such as: Analysing Business Requests, Transforming Data, Cleaning Data, Using Business Logic to bring Value, Storytelling, Dashboard Design, among others.

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
Reading the document "Escenario y Documentos.pdf", there are two key sections from which we receive additional information intended to support idea generation and the inclusion of valuable insights. We have found the following: 

  - National Staff Average Turnover. This data is presented as a news arcticle, redacting the increase in criminality inside the country, emphasizing during the night time, in which people are afraid to commute during night hours; the valuable data to extract is the mentioned day and night average turnover reported by Logistics National Chamber, thus implying this is the National Average Staff Turnover.
      
  | Shift | Percentage |
  |:-------|-----------:|
  | Night  | 68% |
  | Day  | 23% |
      
  - Hiring Number of Staff from our competition "Manchester Stores".This section presents information as if it were an email from a superior providing important insights about the staff hired by our competitor during the first semester of 2017. The message concludes by emphasizing the importance of maintaining a higher number of hires than our competition. Their staff hiring data is at follows:

  | City | Staff Hired |
  |:-------|-----------:|
  | CDMX  | 200 |
  | Ecatepec  | 50 |
  | Guadalajara  | 100 |
  | Zapopan  | 50 |
  | Monterrey  | 200 |
  | Puebla  | 40 |

## Final Dashboard
We got requested to include a two graphs and a table. We decided to use information we have not touched yet. We have choose the following:

- Performance Table versus Manchester Warehouses. We inserted a Pivot of Warehouse Staff Hiring directly into the Dashboard sheet, filtering by the six cities we have Data from our competition and compare with. Adding a Conditional Formatting in Green color if we have above their number, and in Red Color if we were subpar were the final steps.
  
    <img width="435" height="176" alt="image" src="https://github.com/user-attachments/assets/cb8d4cc5-1228-4376-ab5a-eff3807acd95" />
    <img width="162" height="182" alt="image" src="https://github.com/user-attachments/assets/4fa6228c-a0e6-4624-8344-19ccf238d823" />


- Staff Hiring by Position Graph. Before the Graph, a pivot was made in Analysis Sheet; showing the count of people hired by position. Then formatting to match Dashboard colors. We connected this table to the main Slicers at "Filerting Connections".
  
    <img width="277" height="199" alt="image" src="https://github.com/user-attachments/assets/2fa75e50-2681-449b-bea3-ea864c17a693" />
    <img width="508" height="328" alt="image" src="https://github.com/user-attachments/assets/54fb8b62-39f5-4eed-a102-e5e8961003df" />
    

- Staff Hiring Timeline Graph. Similar with previous, we did also inserted a new pivot in Analysis Sheet; this time showing the number of hiring staff during the period of months we have. We connected this table to the main Slicers at "Filerting Connections".
  
    <img width="264" height="185" alt="image" src="https://github.com/user-attachments/assets/235cfc68-4602-4c09-b2e4-c4a30fededad" />
    <img width="463" height="329" alt="image" src="https://github.com/user-attachments/assets/b0762e64-e6af-4239-b734-3b335197ebc2" />
    

- Day & Night Turnover versus the National Average. Since we were given the National Average Turnover, we decided to include this data and compare versus ours. We created two pivots; once for Day Shift and one for Night Shift.We then simply add the numbers directly to the Dashboard, referencing the our Turnover number cells, versus the National Average. We connected this table to the main Slicers at "Filerting Connections".
  
    <img width="378" height="209" alt="image" src="https://github.com/user-attachments/assets/4c0d7fed-2a83-4f6c-af7e-9d4901856498" />
    <img width="271" height="70" alt="image" src="https://github.com/user-attachments/assets/dc39477e-3e5a-48a9-b309-b4d3de87529c" />

      


