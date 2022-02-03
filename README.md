# synthetic_population_dev


This repository contains the following jupyter notebooks:

SPENSER_notebook_1: 
- Merges all persons and households of the study area in two dataframes (df_persons_NE and df_households_NE), 
- Generates a unique primary key for each table (persons (PID_AreaMSOA) and households (HID_AreaOA)) 
- Removes unnecessary persons (those that were not assigned to any households (HIP = (-1)) and those that are assigned to buildings that are not residential (QS420_CELL = -2) or education (QS420_CELL = 26). 
- Removes unnecessary households (those buildings that are not residential (QS420_CELL = -2) or education (QS420_CELL = 26).


SPENSER_notebook_2:
-	Calculates the following columns:
-- Total people in household: count the number of persons in each household
-- Total children in household: count the number of children in each household
-- Same ethnic: check if there are people with the same ethnicity
-- Adult similar age: check if there are people within +- 10 years
-- Children_dependency: Boolean value that tells if a person has a children dependency
-- Marital_status: classifies each individual in married, couple or single based on their socio-demographic characteristics


SPENSER_notebook_3:
- Calculates the attribute: driving licence (True / False)


SPENSER_notebook_4:
- Calculates the column: Economic activity (Employed, Unemployed, Inactive) based on age, gender and OA area. Census 2011 data is projected to 2019 using Regional labour market statistics: HI01 Headline indicators for the North East 


SPENSER_notebook_5:
- Calculates the column: Occupation for employed and unemployed people only. This column classifies these people in 9 categories



Additionally, there is a word file documenting each of the notebooks (e.g., what it does, dependencies and explanation of the main cells).
