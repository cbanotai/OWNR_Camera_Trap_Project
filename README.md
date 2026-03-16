# Olifants West Nature Reserve Camera Trap Project

![Code License: MIT](https://img.shields.io/badge/Code%20License-MIT-blue.svg)
![Data License: CC--BY--4.0](https://img.shields.io/badge/Data%20License-CC--BY--4.0-green.svg)

This repository contains processed datasets and R code for analyses of wildlife activity, habitat use, species interactions, and vegetation dynamics in Olifants West Nature Reserve (OWNR), part of the Greater Kruger Ecosystem in northeastern South Africa.

The repository serves as the central working archive for the OWNR camera trap project and associated ecological datasets. It is intended to support ongoing and future manuscripts arising from this long-term field system. Materials housed here include cleaned camera trap detection data, vegetation monitoring datasets, environmental covariates, and reproducible R scripts used to generate analyses, tables, and figures.

---

## Study Overview

Wildlife activity and ecological processes were monitored using a network of camera traps deployed across multiple sites within a semi-arid savanna landscape. These data were integrated with vegetation monitoring and site-level environmental covariates to evaluate ecological relationships among wildlife behavior, environmental conditions, habitat structure, and vegetation dynamics.

This repository is designed to provide a transparent and reproducible foundation for analyses derived from the broader OWNR project.

---

## Project Status

This repository contains the working data and analysis code for the OWNR camera trap project.

The repository is actively maintained and supports multiple ongoing manuscripts. Archived releases associated with individual manuscripts will be deposited in Zenodo and assigned DOI(s) as those analyses are finalized.

---

## Current Scope

This repository is structured to support multiple analyses and manuscripts derived from the OWNR camera trap system, including but not limited to:

- wildlife activity and habitat-use analyses
- temporal ecology and nocturnal timing analyses
- species interaction and co-occurrence analyses
- herbivore–vegetation relationship analyses
- woody vegetation monitoring and disturbance analyses

As manuscripts are finalized, paper-specific analyses may be organized into separate scripts, folders, and archived Zenodo releases.

---

## Data Scope

This repository contains the processed datasets used for statistical analyses and figure generation.

The full camera trap image archive is maintained separately and is not included in this repository.

---

## Repository Structure

```text
ownr-camera-trap-project/
│
├── README.md
├── metadata.csv
├── session_info.txt
│
├── data/
│   ├── camera_trap_detections.csv
│   ├── vegetation_survey_data.csv
│   ├── site_covariates.csv
│
├── code/
│   ├── 01_data_processing.R
│   ├── 02_statistical_models.R
│   ├── 03_figure_generation.R
│
└── outputs/
    ├── model_summaries.csv
    └── derived_datasets.csv
```

---

## Data Description

### camera_trap_detections.csv

Independent wildlife detections recorded by camera traps.

| Variable | Description |
|---|---|
| site_id | Unique identifier for camera trap location |
| datetime | Timestamp of detection event |
| species | Species detected |
| detection | Binary indicator of detection |
| independent_event | Indicator that the record met the independence threshold |

### vegetation_survey_data.csv

Vegetation monitoring dataset including woody plant measurements and disturbance metrics.

| Variable | Description |
|---|---|
| tree_id | Unique tree identifier |
| site_id | Sampling location |
| species | Plant species |
| dbh_cm | Diameter at breast height (cm) |
| impact_score | Herbivore or disturbance impact category |

### site_covariates.csv

Environmental variables associated with camera trap or vegetation sampling sites.

| Variable | Description |
|---|---|
| site_id | Site identifier |
| ecotype | Vegetation community classification |
| distance_to_water | Distance to nearest waterhole (m) |
| habitat_type | Broad habitat classification |

Additional variable definitions, descriptions, and units are provided in **metadata.csv**.

---

## Quick Start

To reproduce the analysis workflow:

1. Clone the repository:

```bash
git clone https://github.com/chrisbanotai/ownr-camera-trap-project.git
```

2. Open R and set the working directory to the repository.

3. Run the analysis scripts in order:

```text
code/01_data_processing.R
code/02_statistical_models.R
code/03_figure_generation.R
```

Outputs will be written to the `outputs/` directory.

---

## Reproducing the Analysis

All analyses were conducted in **R**.

To reproduce the repository workflow:

1. Download or clone the repository.
2. Install the required R packages listed in the scripts.
3. Run the scripts in the following order:

```text
code/01_data_processing.R
code/02_statistical_models.R
code/03_figure_generation.R
```

Running these scripts sequentially will:

1. process and merge input datasets
2. fit statistical models
3. generate figures and derived outputs

Outputs will be saved to the `/outputs` directory.

As additional manuscripts are finalized, manuscript-specific scripts or subdirectories may be added to the repository.

---

## Software Environment

Analyses were performed in **R**.

The computational environment used for these analyses is documented in:

`session_info.txt`

This file records the R version and package versions used in the workflow.

---

## Metadata

Variable definitions, descriptions, and units for repository datasets are provided in:

`metadata.csv`

Users should consult this file before reusing or interpreting repository data.

---

## Data Availability

This GitHub repository serves as the working project repository for processed data, code, and derived outputs associated with the OWNR camera trap project.

Archived, citable releases associated with specific manuscripts will be deposited in Zenodo and assigned DOI(s) as those analyses are finalized.

GitHub repository:  
https://github.com/chrisbanotai/ownr-camera-trap-project

Zenodo DOI(s):  
To be added for manuscript-specific releases.

---

## Repository Principles

This repository follows open-science and reproducibility best practices:

- All analyses should be reproducible from the scripts provided.
- Data included here are the processed datasets used in analyses.
- Raw field data and full camera trap imagery are archived separately.
- Manuscript-specific releases will be archived in Zenodo with DOI(s).

---

## Data License

Unless otherwise noted, datasets contained within the `/data` directory are licensed under the **Creative Commons Attribution 4.0 International (CC-BY 4.0)** license.

Users are free to reuse and adapt these data provided appropriate citation of the associated study and archived dataset release.

License information:  
https://creativecommons.org/licenses/by/4.0/

---

## Code License

Unless otherwise noted, all scripts contained within the `/code` directory are released under the **MIT License**.

---

## Citation

If you use data or code from this repository, please cite the relevant archived Zenodo release once available.

A formal project-level citation will be added as the repository develops.

---

## Contact

Christopher M. Banotai  
Email: cbanotai38@gmail.com
