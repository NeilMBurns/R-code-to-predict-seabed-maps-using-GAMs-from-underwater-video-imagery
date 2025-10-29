```markdown
# Wester Ross Seabed Map

This repository contains R code and workflows used to generate a high-resolution seabed habitat map for **Wester Ross, Scotland**. The methods combine video imagery from seabed camera drops with spatial modelling approaches to classify and map seabed types.  

The code is designed to be **reproducible and adaptable**, allowing users to apply the same workflow to other marine areas where camera-based seabed data are available.

---

## Overview

This project was developed to support a data paper describing the **Wester Ross seabed habitat dataset**, which will be archived and openly available on [Figshare](https://figshare.com/) (DOI to be added once released).  

The main objectives of this repository are to:

- Provide open access to the analytical workflow used to create the seabed map.  
- Demonstrate reproducible processing of video-derived seabed classifications.  
- Offer a generalised framework that can be adapted for other benthic mapping applications.

---

## Data

The associated dataset comprises:
- **Video imagery** collected using seabed camera drops across Wester Ross.  
- **Seabed type classifications** derived from expert interpretation of the imagery.  

Once the Figshare dataset is released, you will be able to access it via the DOI provided below:

> **Data DOI:** `to be added`

The repository does **not** include the raw video data but provides all scripts required to process the publicly archived data once available.

---

## Code Structure

```

Wester_Ross_seabed_map/
├── data/ # Directory for input data (empty by default)
├── scripts/ # Core R scripts for data cleaning, analysis, and mapping
├── outputs/ # Figures, maps, or model outputs
├── README.md # Project overview (this file)
└── LICENSE # License information

````

Key scripts include:
- `01_data_preparation.R` – cleans and formats seabed classification data  
- `02_model_fitting.R` – fits spatial models of seabed type  
- `03_mapping_output.R` – generates final habitat maps and visualisations  

---

## Requirements

The analysis is written in **R** (≥ 4.2).  
Recommended packages include:

```r
tidyverse
sf
raster
ggplot2
mgcv
INLA
````

You can install any missing packages with:

```r
install.packages(c("tidyverse", "sf", "raster", "ggplot2", "mgcv"))
# INLA requires a separate installation:
install.packages("INLA", repos="https://inla.r-inla-download.org/R/stable")
```

---

## Reproducibility

This repository follows open-science best practices:

* All code is open and version-controlled via GitHub.
* Data are archived on Figshare with a DOI for citation and reuse.
* Scripts are modular and annotated for transparency and reproducibility.

You are encouraged to **fork, adapt, and reuse** the workflow for other habitat mapping projects.

---

## Citation

If you use this code or data, please cite the data paper once published:

> *Authors (Year).* Title of data paper. *Journal Name.* DOI: `to be added`

---

## License

This repository is licensed under the **MIT License**, allowing reuse and modification with appropriate credit.

---

## Contact

For questions, collaboration, or feedback, please contact:
**[Your Name]**
[Your Institution or Research Group]
[Your Email]

---

*Developed as part of ongoing research into seabed habitat mapping and open data sharing in marine ecology.*

```
```

