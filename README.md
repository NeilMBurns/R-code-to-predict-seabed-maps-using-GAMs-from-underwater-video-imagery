
# Dataset and R code to predict seabed maps using GAMs from underwater video imagery in a Scottish Sea Loch

Repository containing analysis code, and links to the data supporting the paper:

**Predicting seabed maps using GAMs from underwater video imagery in a Scottish Sea Loch**  
Burns, N.M., Bailey, D.M. and Hopkins, C.R.   
Submitted to *[Journal]*, 2025  
[DOI to follow]

---

## Abstract

These data include geolocated seabed classifications identified from Stereo Baited Remote Underwater Video (SBRUV) camera deployments in Little ...

---

## Repository Structure

```
.
├── data/                          # CSV data files for seabed classifications and bathymetry files
├── GAM_predicted_seabed_maps.Rmd  # Master RMarkdown script for entire analysis workflow
├── figures/                       # Model outputs, maps and summary figures
├── LICENSE
├── README.md
└── requirements.txt               # List of R packages for reproducibility
```

---

## How to Reproduce the Analysis

### Clone this repository:
```bash
git clone https://github.com/NeilMBurns/Wester_Ross_seabed_map.git
cd Wester_Ross_seabed_map
```

### Install R dependencies:
From within R:
```R
install.packages(c("sf", "flux", "RColorBrewer", "mgcv", "fields", "terra", "here", "dplyr", "rnaturalearth", "rnaturalearthdata", "prettymapr"))
```
Optionally use `renv` or `packrat` for environment management.

### Open `GAM_predicted_seabed_maps.Rmd` in RStudio and Knit or run code chunks sequentially.

This script:
- Reads and prepares the seabed classification data
- Converts data to spatial objects
- Summarises descriptive statistics
- Loads environmental spatial layers
- Fits spatial GAMs
- Produces figures of the probability of presence for seabed types, a combined seabed map and assesses model predictions with crossvalidation

Outputs will be saved to the `figures/` directory.

---

## Data Availability

Code and anonymised data used to generate this manuscript’s analyses are available at:  
[https://github.com/NeilMBurns/Wester_Ross_seabed_map](https://github.com/NeilMBurns/Wester_Ross_seabed_map)  
A DOI will be issued via Figshare on publication.

---

## License

- The code in this repository is released under the [MIT License](LICENSE).
- The data provided is released under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.

You are free to use, share and adapt the materials, provided appropriate credit is given to the original authors.

---

## Citation

If you use these materials, please cite:

```
Burns, N.M., Bailey, D.M. and Hopkins, C.R.  (2025). Predicting seabed maps from underwater video imagery using GAMs in a Scottish Sea Loch. [Journal]. DOI to follow.
```

BibTeX:
```bibtex
@article{Burns2025sebedmap,
  title={Predicting seabed maps from underwater video imagery using GAMs in a Scottish Sea Loch.},
  author={Burns, N.M. and Bailey, D.M. and Hopkins, C.R.},
  journal={[Journal]},
  year={2025},
  doi={DOI to follow}
}
```

---

## Contact

For questions, data access, or collaboration enquiries:

- **Dr Neil M. Burns** — [neil.burns@glasgow.ac.uk]
- Or open an issue on this repository

---
