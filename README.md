# fameR
A reproducible R pipeline for end‑to‑end processing of GC‑FID fatty acid methyl ester (FAME) datasets. This workflow automates cleaning, calibration, quantification, metadata integration, QC checks, and visualization—producing tidy, analysis‑ready outputs with minimal manual intervention

# Key Features
- Automated import and cleaning of ChemStation GC‑FID integration reports  
- Calibration‑level mapping and extraction of slopes, intercepts, and R² values  
- Quantification of calibrated and surrogate‑calibrated compounds  
- Integration with experimental metadata  
- Quality‑control checks for internal standard issues and abnormal FAME profiles  
- Export of tidy datasets, calibration plots, and FAME‑profile visualizations  
- Example dataset and metadata included for demonstration  

## Getting Started

### 1. Install Required Packages
Install required packages before running the pipeline:
- tidyverse  
- readxl  
- stringr  
- ggpmisc  
- openxlsx  
- writexl  
- ggpubr  
- rstatix  
- tools  

### 2. Prepare Input Files
The pipeline expects:
- GC‑FID integration reports (ChemStation XLSX format)  
- Experiment metadata  
- FAME external standards calibration matrix  
- Optional: surrogate quantification rules  

Example files are provided in `data_example/`.

### 3. Update User Inputs
In `FAME_pipeline.Rmd`, update the paths under the **USER INPUT** sections:
- GC‑FID data folder  
- Calibration file  
- Quantification rules  
- Metadata file  
- Export directory  

### 4. Run the Pipeline
Run the R Markdown document chunk‑by‑chunk or knit the full workflow.

Generated outputs include:
- `GCFID_Results_Cleaned.xlsx`  
- Calibration curve JPEGs  
- FAME % composition figures  
- QC summaries and alerts  

## Example Data
`data_example/` includes:
- Synthetic GC‑FID integration reports  
- Sample calibration matrix  
- Example quantification rules  
- Example metadata  
- Expected outputs  

## Citation
If this pipeline contributes to your work, please cite this repository and **Placeholder for publication**.
