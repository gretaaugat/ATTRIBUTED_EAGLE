
# ATTRIBUTED_EAGLE

## Introduction

This project provides datasets and code for the implementation of ATTRIBUTED_EAGLE, an algorithm designed for feature selection from attributed graph data. It has been applied to two real-world scenarios: analyzing CO2 emissions and homicide rates in Brazil during 2010.

---

## Folder Structure

```
.
├── datasets/
│   ├── br_data_census_2010.csv.zip
│   ├── br_data_census_2010_co2_log.csv.zip
│   ├── br_data_census_2010_homicides.csv.zip
│   ├── br_co2_log_2010.csv
│   ├── br_homicides_2010.csv
│   └── filtered_adjacency_matrix_inv.csv.zip
├── codes/
│   ├── k_value_and_statistical_test_co2.ipynb
│   ├── k_value_and_statistical_test_homicides.ipynb
│   ├── attributed_eagle_homicides.ipynb
│   ├── compute_RF_RFE_co2.ipynb
│   ├── compute_RF_RFE_homicides.ipynb
│   └── attributed_eagle_log_co2.ipynb
├── images/
│   └── ...
├── features_selected_homicides/
│   ├── rf.json
│   ├── rfe.json
│   └── attributed_eagle_hom.json
├── features_selected_co2/
│   ├── rf.json
│   ├── rfe.json
│   ├── attributed_eagle_log_co2_n2.json
│   └── attributed_eagle_log_co2.ipynb
└── pipeline/
    └── [See Google Drive](https://drive.google.com/drive/folders/1UlZS2eW3CW2EFhv1T8RaQzXLm9_mkCT5?usp=drive_link)
```

---

## Datasets

The `datasets/` folder contains:
- **`br_co2_log_2010.csv`**: Log-transformed CO2 emission data for Brazil in 2010.
- **`br_data_census_2010.csv.zip`**: Brazilian census data from 2010.
- **`br_data_census_2010_co2_log.csv.zip`**: Census data combined with log-transformed CO2 emission data.
- **`br_data_census_2010_homicides.csv.zip`**: Census data combined with homicide rates for 2010.
- **`br_homicides_2010.csv`**: Absolute Brazilian homicide rates for 2010.
- **`filtered_adjacency_matrix_inv.csv.zip`**: Inverse adjacency matrix.

---

## Pipeline

The `pipeline/` folder contains the following result files:
- **`results_co2.zip`**: Contains predictive model results for CO2 emissions.
- **`results_homicides.zip`**: Contains predictive model results for homicide rates.

Due to the large size of these files, they are hosted on Google Drive. You can access them at:

**[Pipeline Folder on Google Drive](https://drive.google.com/drive/folders/1UlZS2eW3CW2EFhv1T8RaQzXLm9_mkCT5?usp=drive_link)**

---

## Usage

### Key Notebooks:
- **`k_value_and_statistical_test_co2.ipynb`**: Analyzes K-values and statistical tests for CO2 prediction using results from the `pipeline/results_co2` folder.
- **`k_value_and_statistical_test_homicides.ipynb`**: Similar analysis for homicide prediction using results from the `pipeline/results_homicides` folder.
- **`compute_RF_RFE_co2.ipynb`**: Performs feature selection using Random Forest (RF) and Recursive Feature Elimination (RFE) for CO2 use case. 
- **`compute_RF_RFE_homicides.ipynb`**: Performs feature selection using Random Forest (RF) and Recursive Feature Elimination (RFE) for homicide use case.
- **`attributed_eagle_log_co2.ipynb`**: Implements ATTRIBUTED_EAGLE for log-transformed CO2 prediction.
- **`attributed_eagle_homicides.ipynb`**: Implements ATTRIBUTED_EAGLE for homicide prediction.

---

## Results

Results of the predictive models are stored in the `pipeline/` folder as **`results_co2.zip`** and **`results_homicides.zip`**. Please access these files via Google Drive:

**[Pipeline Folder on Google Drive](https://drive.google.com/drive/folders/1UlZS2eW3CW2EFhv1T8RaQzXLm9_mkCT5?usp=drive_link)**

---

## Contributing

We welcome contributions! For suggestions or new features, please open an issue or submit a pull request.
