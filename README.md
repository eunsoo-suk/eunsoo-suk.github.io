# Analysis of Occupational Fatalities Across U.S. Industries

#### Author: Eunsoo Suk

This project presents a systematic analysis of occupational fatality patterns across U.S. industries using longitudinal data from the Bureau of Labor Statistics (BLS). The study emphasizes rigorous data preprocessing, exploratory statistical analysis, and unsupervised representation learning to identify structural similarities among industries based on fatality characteristics.

## 1. Objective

**The primary objectives of this project are:**

- To examine temporal and industry-level trends in occupational fatalities

- To characterize accident-type distributions across industries

- To identify latent industry groupings using data-driven, unsupervised learning methods

- To demonstrate the applicability of deep representation learning to structured occupational safety data

## 2. Data Source

**Provider:** U.S. Bureau of Labor Statistics (BLS)

**Dataset:** Census of Fatal Occupational Injuries (CFOI)

**Granularity:** Industry-level annual fatality counts

**Attributes:** Total fatalities, Accident-type–specific fatalities, NAICS industry codes, Yearly observations

## 3. Data Preprocessing and Cleaning

**To ensure analytical validity and cross-year comparability, the following preprocessing steps were applied:**

- Initial inspection and schema validation

- Standardization of industry names across reporting years

- Conversion of accident-type columns to numeric representations

- Recalculation and verification of total fatality counts

- Cleaning, imputation, and normalization of NAICS codes

- Manual reconciliation of inconsistent industry labels

- Removal of aggregated summary rows to produce the final modeling dataset

## 4. Exploratory Data Analysis (EDA)

**Exploratory analysis was conducted to understand both global and industry-specific fatality patterns:**

- Descriptive statistics of fatality counts

- Distributional analysis of total fatalities

- Temporal trend analysis across industries

- Identification of industries with consistently high fatality burdens

- Accident-type composition analysis

- Industry–year heatmap visualization

- NAICS-level comparative analysis

<p align="center">
  <img src="https://github.com/user-attachments/assets/b9c0ab91-6c8c-4d8f-ad6b-e340f26a8804" width="49%" />
  <img src="https://github.com/user-attachments/assets/1405f1b5-4cd2-4d5b-81f4-8f287280ab19" width="49%" />
</p>

## 5. Unsupervised Industry Clustering

**To uncover latent structural similarities among industries, an unsupervised learning pipeline was implemented.**

**5.1 Feature Engineering**

- Aggregation of fatality metrics at the industry level

- Feature normalization to ensure scale invariance

**5.2 Representation Learning**

- A feedforward autoencoder was trained to learn compact latent embeddings

- The latent space captures non-linear relationships among fatality features

**5.3 Clustering**

- KMeans clustering was applied to the learned latent representations

- Resulting clusters represent industry groups with similar fatality profiles

<img width="1106" height="817" alt="image" src="https://github.com/user-attachments/assets/0e3fce06-9d59-46d8-bf00-99cdc72fdf24" />

## 6. Fatal Injury Forecasting

**Objective:** Forecast future occupational fatality trends to support proactive risk assessment

**Target:** Annual fatality counts (industry-level; optional accident-type level)

**Method:** Time-series forecasting using trend-based and classical statistical models

**Validation:** Evaluation on held-out years using MAE and RMSE

**Outcome:** Identification of industries and accident types with increasing fatality risk

<p align="center">
  <img src="https://github.com/user-attachments/assets/4c1d762f-540d-46c1-87bb-76af6d3efabf" width="49%" />
  <img src="https://github.com/user-attachments/assets/b3979f1c-4f00-4c89-b76c-92635ef24706" width="49%" />
</p>

<img width="964" height="477" alt="image" src="https://github.com/user-attachments/assets/2d05319b-f375-4738-8cad-a11f9895951a" />

## 7. Key Contributions

- A reproducible pipeline for occupational fatality data analysis

- Robust preprocessing methodology for multi-year BLS datasets

- Application of deep unsupervised learning to occupational safety analytics

- Data-driven insights into industry-level risk structures

## 8. Reproducibility

- All data processing and modeling steps are fully scripted in Jupyter notebooks

- Raw data files are excluded due to size and licensing constraints

- Data acquisition and preprocessing steps are documented to support replication

## 9. Intended Audience

- This repository is intended for:

- Occupational safety and health researchers

- Data scientists working with public labor statistics

- Policy analysts interested in industry-level risk assessment

- Students and researchers studying applied machine learning on tabular data

<img width="1106" height="598" alt="image" src="https://github.com/user-attachments/assets/a25b8386-5145-4593-9336-91f928c74c3f" />
