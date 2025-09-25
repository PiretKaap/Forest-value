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
| Eraldise nr | INTEGER | Part of forest within a cadastral unit where the trees are uniform in species, age, and site conditions | | Linda AI generated .json file |
| Puuliik | TEXT | Distinct type of tree (Spruce, Pine, Birch, Other Deciduous) | | Linda AI generated .json file |
| Kõrgus | FLOAT | Tree height | meter | Linda AI generated .json file |
| Diameeter | FLOAT | Tree diameter | centimeter | Linda AI generated .json file |
| Pindala ha | FLOAT | Area of the stand | hectare | Linda AI generated .json file |
| Tihedus m3/ha | FLOAT | Timber volume per hectare | cubic meter per hectare | Linda AI generated .json file |
| Tagavara m3 | FLOAT | All the timber on a stand | cubic meter | Calculation |
| Name_EE | TEXT | Tree name in Estonian (KU - Spruce, MA - Pine, KS - Birch, Other Deciduous) | | Puu_nimetused_EE_ENG.xlsx |
| Name_ENG | TEXT | Tree name in English (Spruce, Pine, Birch, Other Deciduous) | | Puu_nimetused_EE_ENG.xlsx |
| Suhteline tugikõrgus | FLOAT | Ratio of trunk height above ground to total tree height | | Suhtelised_tugikõrgused.xlsx |
| h24 | INT | The average height of a tree with a diameter of 24 cm | meter | Calculation |
| Diameetri klass | INT | Tree trunk diameter category| centimeter | Calculation |
| Sortimentide jaotusklass | TEXT | Code that consists of - diameetri klass, Name_EE, h24 | | Calculation |
| Kasutusotstarbe kategooria | TEXT | Intended purpose or application of a specific wood or forest product - palk, peenp, paber, küte, jäätmed | | Mahutabel.xlsx |
| Kasutusotstarbe kategooria osakaal| FLOAT | proportion of total wood volume in this usage category | % | Mahutabel.xlsx |
| Maht (tm) | FLOAT | Total volume of each usage category by species on the cadastral area | solid cubic meter | Calculation |
| Hind (€/tm) | FLOAT | Log, small timber, pulpwood, fuelwood price per solid cubic meter | €/solid cubic meter | Hinnakiri.xlsx |
| Hind (€) | FLOAT | Price for total volume  | € | Calculation |
| Kompleksteenus (€/tm)| FLOAT | Estimated cost of harvesting a cubic meter of wood | €/solid cubic meter | Manually entered |
| Transport (€/tm) | FLOAT | Estimated cost of transporting a cubic meter of wood | €/solid cubic meter | Manually entered |
| Alghinna(%) | INT | Percentage of the defined base price (for calculating reccomended starting bid) | % | Manually entered |
| Kulud (jäätmeteta) | FLOAT | Per cubic meter prices of comprehensive service and transportation multiplied by the total wood volume, from which the cost of the waste volume has been subtracted | € | Calculation |
| Soovituslik alghind | FLOAT | Calculation based on Tulud-kulud (jäätmeteta) calculation and reduced by 10% based on the Alghind.| € | Calculation |

# Creation of dummy dataset

# Description of Data Protection
Üldpõhimõtted + Firmasisene kasutamine + programmi koostamisel on meid usaldatud/oleme saanud ligipääsu ... failidele.

# Data Quality Control 

# Data Flow 

# Exploratory Data Analysis 
Initial Data Assessment:
Input Validation:

# Statistical Data Analysis 

# Descriptive Report / Analysis 

# Data Story, Conclusions 
