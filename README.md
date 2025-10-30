
# 📄 Conservation Relevant Fine-Scale Distribution and Habitat Associations of Threatened Elasmobranchs in Temperate Nearshore Waters

Repository containing analysis code, data, and supplementary materials supporting the paper:

**Conservation Relevant Fine-Scale Distribution and Habitat Associations of Threatened Elasmobranchs in Temperate Nearshore Waters**  
Hopkins, C.R., Cullen, G., Flatt, R.L., Brooker, E.E., Bailey, D.M., and Burns, N.M.  
Submitted to *[Journal]*, 2025  
[DOI to follow]

---

## 📑 Abstract

This study examined elasmobranch species richness, abundance and habitat associations in Scottish nearshore waters using Stereo Baited Remote Underwater Video Systems (SBRUVs) between 2021–2023. Bayesian hierarchical spatial models fitted with INLA were used to quantify the influence of depth, substratum, and spatial autocorrelation on species presence for key threatened species. Findings provide new conservation-relevant data on distribution patterns and habitat preferences of elasmobranchs, including flapper skate (*Dipturus intermedius*), spiny dogfish (*Squalus acanthias*), and porbeagle (*Lamna nasus*).

---

## 📂 Repository Structure

```
.
├── data/                      # CSV data files for species presence and environmental covariates
├── Scotland_sharks.Rmd        # Master RMarkdown script for entire analysis workflow
├── figures/                   # Model outputs, maps and summary figures
├── LICENSE
├── README.md
└── requirements.txt           # List of R packages for reproducibility
```

---

## 📝 How to Reproduce the Analysis

### 1️⃣ Clone this repository:
```bash
git clone https://github.com/NeilMBurns/Temperate_Elasmobranchs.git
cd Temperate_Elasmobranchs
```

### 2️⃣ Install R dependencies:
From within R:
```R
install.packages(c("INLA", "fmesher", "sf", "terra", "vegan", "dagitty", "boot", "RColorBrewer", "tidyterra", "fields"))
```
Optionally use `renv` or `packrat` for environment management.

### 3️⃣ Open `Scotland_sharks.Rmd` in RStudio and Knit or run code chunks sequentially.

This script:
- Reads and prepares elasmobranch presence-absence data
- Converts data to spatial objects
- Summarises descriptive statistics and species richness by location and year
- Loads environmental spatial layers
- Fits spatial Bayesian models via R-INLA
- Produces figures of species distribution, habitat associations and model predictions

Outputs will be saved to the `figures/` directory.

---

## 📊 Data Availability

Code and anonymised data used to generate this manuscript’s analyses are available at:  
👉 [https://github.com/NeilMBurns/Temperate_Elasmobranchs](https://github.com/NeilMBurns/Temperate_Elasmobranchs)  
A DOI will be issued via Figshare on publication.

---

## 📄 License

- The code in this repository is released under the [MIT License](LICENSE).
- The data provided is released under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.

You are free to use, share and adapt the materials, provided appropriate credit is given to the original authors.

---

## 📣 Citation

If you use these materials, please cite:

```
Hopkins, C.R., Cullen, G., Flatt, R.L., Brooker, E.E., Bailey, D.M., Burns, N.M. (2025). Conservation Relevant Fine-Scale Distribution and Habitat Associations of Threatened Elasmobranchs in Temperate Nearshore Waters. [Journal]. DOI to follow.
```

BibTeX:
```bibtex
@article{hopkins2025elasmobranchs,
  title={Conservation Relevant Fine-Scale Distribution and Habitat Associations of Threatened Elasmobranchs in Temperate Nearshore Waters},
  author={Hopkins, C.R. and Cullen, G. and Flatt, R.L. and Brooker, E.E. and Bailey, D.M. and Burns, N.M.},
  journal={[Journal]},
  year={2025},
  doi={DOI to follow}
}
```

---

## 📬 Contact

For questions, data access, or collaboration enquiries:

- **Dr Neil M. Burns** — [your email]
- Or open an issue on this repository

---
