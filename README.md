# ATTRIBUTED_EAGLE

This repository contains the code and data associated with a data analysis project based on the 2010 Demographic Census from the Brazilian Institute of Geography and Statistics (IBGE). The primary objective is to perform statistical analyses and visualizations on a complex dataset, focusing on the evaluation of a specific `K` parameter and the exploration of various census characteristics.

## About the Project

The `ATTRIBUTED_EAGLE` project aims to explore and analyze a vast dataset derived from the 2010 IBGE Demographic Census. Given the granularity and volume of census information, the dataset comprises over 4000 features, categorized for better organization and understanding. The analysis focuses on conducting statistical tests and generating graphs, particularly to understand the behavior or optimize a parameter `K`.

## Dataset

The main dataset used in this project is `data_noelections.csv` (or its compressed version `data_noelections.csv.zip`), derived from the 2010 IBGE Demographic Census. It is a robust set of data covering various socioeconomic, demographic, and geographical characteristics of Brazil.

Due to the considerable size of some raw data files (`.csv`), **Git Large File Storage (Git LFS)** is used to manage files larger than 100 MB. It is recommended to download the compressed version (`.zip`) or configure Git LFS to clone the repository correctly.

### Feature Structure and Categories

The dataset consists of **4061 features**, organized into the following categories for easier analysis. Although some categorical variables may be represented by numerical codes in the dataset for storage and processing efficiency, their inherent categorical nature is maintained for data analysis and interpretation purposes.

| Feature Category    | #    | Typical Data Type               | Generic Description                                                                   |
| :------------------ | :--- | :------------------------------ | :------------------------------------------------------------------------------------ |
| IDHM                | 8    | Numeric (Float)                 | Municipal Human Development Index indicators (Education, Longevity, Income).          |
| GLOBAL              | 3    | Mixed (Numeric, Categorical)    | General characteristics of the census tract or municipality (e.g., total population, area). |
| GEO                 | 22   | Categorical (ID), Numeric (Coordinates) | Geographic identifiers and spatial information (e.g., municipality codes, latitude, longitude). |
| CENSUS BASIC        | 12   | Mixed (Numeric, Categorical)    | Fundamental census data, such as household counts, population by sex.                 |
| CENSUS DOMICILE     | 380  | Mixed (Numeric, Categorical)    | Characteristics of households (e.g., housing type, access to sanitation, number of rooms). |
| CENSUS PEOPLE       | 2119 | Mixed (Numeric, Categorical)    | Demographic and socioeconomic data of the population (e.g., age, education level, income, occupation). |
| CENSUS RESPONSIBLE  | 456  | Mixed (Numeric, Categorical)    | Information about the head of the household or family (e.g., age of head, education level of head). |
| CENSUS SURROUNDINGS | 1062 | Mixed (Numeric, Categorical)    | Characteristics of the surroundings of households or the census tract (e.g., access to neighborhood services, infrastructure). |
| **Total** | **4062** |                                 |                                                                                       |

**Data Source:**
* **2010 Demographic Census (Results - IBGE):** [https://censo2010.ibge.gov.br/resultados.html](https://censo2010.ibge.gov.br/resultados.html)


* **`k_analysis_and_plots.py`**: This script is responsible for executing statistical tests and generating graphs related to the `K` parameter.
