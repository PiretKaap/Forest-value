# Introduction
This is the final project for the **ValiIT! Data Analyst** course. The project demonstrates our ability to apply core data analysis principles—including **data cleaning, analysis, and visualization**—to solve a complex, real-world business challenge.
### Technical Tools Used:
*Data Manipulation & Analysis:* **SQL, Python (Pandas, NumPy)**

*Data Visualization:* **Power BI**

*Version Control:* **Git**

## ⭐Project Team⭐
#### Product Owner **Piret Kääp**, 
LinkedIn: https://www.linkedin.com/in/piretsaartok/, Portfolio: https://github.com/PiretKaap/Portfolio

#### Product Tester **Triin Pent**,
LinkedIn:, Portfolio: 

#### Product Tester **Vahur Täht**, 
LinkedIn:, Portfolio: 

# Research Problem:  
Company X operates in the fields of forestry, real estate, and the wood industry. It uses an in-house, time-consuming program to calculate the values of forest and agricultural land. The company wants a tool to make the valuation process smoother and more efficient.

# Research Plan 
The main question is how to determine a property's true value. For this, we will create a model that calculates a data-supported estimate based on a number of key variables. 

# Business Glossary
Return a valuation software or model used to calculate the value of forest and agricultural land by integrating multiple factors.

# Data Model

# Data Dictionary
| Field Name | Data Type | Definition | Unit| Source |
|:---:|:---:|:---:|:---:|:---:|
| Kulud | FLOAT | Defining costs - Kompleksteenus (€/tm), Transport (€/tm), multiplied by volume | €/tm | Manually entered |
| Kompleksteenus | FLOAT | Estimated cost of harvesting a cubic meter of wood | €/cubic meter | Manually entered |
| Transport | FLOAT | Estimated cost of transporting a cubic meter of wood | €/cubic meter | Manually entered |
| Alghinna(%) | INTEGER | Percentage of the defined base price (for calculating reccomended starting bid) | € | Manually entered |
| Stock m3 | FLOAT | All the timber on a specific forest plot | cubic meter | Linda AI generated .json file |
| Hind | FLOAT | Log, small timber, pulpwood, fuelwood prices in € | € | Hinnakiri.xlsx |
| Stand | INTEGER | Part of forest within a cadastral unit where the trees are uniform in species, age, and site conditions, managed as one unit | | Linda AI generated .json file |
| Sortiment  | TEXT | Different types of timber as logs, small logs, pulpwood, and waste | | Linda AI generated .json file |
| Species | TEXT | Distinct type of tree (Spruce, Pine, Birch, Other Deciduous) | | Linda AI generated .json file |
| Maht | FLOAT | Timber volume | cubic meter | Linda AI generated .json file |
| Diameter | FLOAT | Tree diameter | centimeter | Linda AI generated .json file |
| Height | FLOAT | Tree height | meter | Linda AI generated .json file |
| Area ha | FLOAT | Total area | hectare | Linda AI generated .json file |
| Volume | FLOAT | Timber quantity per hectare | cubic meter | Linda AI generated .json file |
| Name_EE | TEXT | Tree name in Estonian (KU - Spruce, MA - Pine, KS - Birch, Other Deciduous) | | Puu_nimetused_EE_ENG.xlsx |
| Name_ENG | TEXT | Tree name in English (Spruce, Pine, Birch, Other Deciduous) | | Puu_nimetused_EE_ENG.xlsx |
| Diameter category | FLOAT | Tree trunk diameter categories | | Calculation |
| Relative height (h24) | INTEGER | The average height of a tree with a diameter of 24 cm. Calculaton: Height / h24 coefficient, rounded up to the nearest whole number | | Suhtelised_tugikõrgused.xlsx |
| h24 coefficient | FLOAT | Ratio of trunk height above ground to total tree height | | Suhtelised_tugikõrgused.xlsx |
| Sortimentide jaotusklass | TEXT | Code that consists of - Tree diameter category, Name_EE, h24 | | Calculation |
| Mahu jaotus | FLOAT | Log volume distribution - palk, peenp, paber, küte, jäätmed | cubic meter | Mahutabel.xlsx |
| Kulud (jäätmeteta) | FLOAT | Per cubic meter prices of comprehensive service and transportation multiplied by the total wood volume, from which the cost of the waste volume has been subtracted | € | Calculation |
| Tulud-kulud (jäätmeteta) | FLOAT | Total calculated price, from which the cost of expenses has been subtracted | € | Calculation|
| Soovituslik alghind | FLOAT | Calculation based on Tulud-kulud (jäätmeteta) calculation and reduced by 10% based on the Alghind.| € | Calculation|
| | | | | |


# Creation of dummy dataset

# Description of Data Protection

# Data Quality Control 

# Data Flow 

# Exploratory Data Analysis 

# Statistical Data Analysis 

# Descriptive Report / Analysis 

# Data Story, Conclusions 
