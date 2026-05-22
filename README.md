# SDS210 ZüriWieNeu – Spatial Data Analysis Project

## Overview

This project was developed as part of the course **SDS210 – Programming with Spatial Data (FS2026)** at the **Department of Geography, University of Zurich (UZH)**.

The project analyses and visualizes the spatial distribution and temporal development of reports submitted through the Zurich city platform **ZüriWieNeu** between **2013 and 2026**.

ZüriWieNeu is a public reporting platform where residents of Zurich can report damages or issues related to the city infrastructure.

ZüriWieNeu: [https://www.zueriwieneu.ch/](https://www.zueriwieneu.ch/)

---

# Project Structure

```
sds210-final-project/
│
├── data/
│   ├── raw/                 # Raw downloaded datasets
│   └── processed/           # Cleaned and processed datasets
│
├── metadata/                # Metadata, data dictionaries, and documentation
│
├── notebooks/
│   └── programming_project_ZüriWieNeu.ipynb
│
├── outputs/                 # Generated plots and visualisations
│
├── environment-sds210-final-project.yml   # Conda environment configuration
│
└── README.md
```

---

# Data Sources

The raw datasets are **not included** in this repository and must be downloaded manually.

## 1. ZüriWieNeu Reports

Contains all citizen reports submitted via the ZüriWieNeu platform.

Dataset:

City of Zurich Open Data – ZüriWieNeu Reports: [https://data.stadt-zuerich.ch/dataset/geo\_zueri\_wie\_neu](https://data.stadt-zuerich.ch/dataset/geo_zueri_wie_neu)

## 2. Statistical Districts of Zurich

Spatial boundary data for Zurich districts.

Dataset **csv!**:

City of Zurich Open Data – Statistical Districts: [https://data.stadt-zuerich.ch/dataset/geo\_statistische\_quartiere](https://data.stadt-zuerich.ch/dataset/geo_statistische_quartiere)

## 3. Population Data of the City of Zurich

Population statistics.

Dataset:

City of Zurich Population Statistics: [https://www.stadt-zuerich.ch/content/dam/web/de/politik-verwaltung/statistik-und-daten/daten/bevoelkerung/BEV321T3211\_auslaendische-Wohnbevoelkerung\_Bevoelkerung\_nach-Herkunft-Stadtkreis-Stadtquartier.xlsx](https://www.stadt-zuerich.ch/content/dam/web/de/politik-verwaltung/statistik-und-daten/daten/bevoelkerung/BEV321T3211\_auslaendische-Wohnbevoelkerung\_Bevoelkerung\_nach-Herkunft-Stadtkreis-Stadtquartier.xlsx)

---

# Installation

## Prerequisites

Make sure the following software is installed:

- Conda / Miniconda: [https://www.anaconda.com/docs/getting-started/miniconda/install/overview](https://www.anaconda.com/docs/getting-started/miniconda/install/overview)
- Git: [https://git-scm.com/install/](https://git-scm.com/install/)

# Setup Instructions in the Terminal

## 1. Navigate to your desired location

```bash
cd <path-to-desired location>
```

## 2. Clone the Repository

```bash
git clone https://github.com/ChristophUZH/sds210-final-project

```

## 3. Enter the repository folder

```bash
cd <path-to-ds210-final-project-repository-folder>

ls -a

```

## 4. Create the Conda Environment

```bash
conda env create -f environment-sds210-final-project.yml

If this file above does not work, this file might work.

conda env create -f environment-sds210-final-project_safty.yml

Otherwise use an LLM to solve the problem.
```

## 5. Activate the Environment

```bash
conda activate sds210-final-project
```

## 6. Start JupyterLab

```bash
jupyter lab
```

---

# Running the Project

## Step 1 – Download Raw Data

Download all datasets listed in the **Data Sources** section.

## Step 2 – Store Data

Place the downloaded files into:

```text
data/raw/
```

## Step 3 – Run the Notebook in JupyterLab

Open and execute:

```text
notebooks/programming_project_ZüriWieNeu.ipynb
```

The notebook performs:

- data cleaning
- data processing
- spatial analysis
- temporal analysis
- map creation
- data visualisations

---

# Outputs

After execution, the project generates:

## Processed Data

Stored in:

```text
data/processed/
```

## Visualisations and Plots

Stored in:

```text
outputs/
```

Examples include:

- heatmaps
- district comparison plots
- temporal evolution plots
- comparison of absolute and relative values

---

# Notes

- Raw data files are excluded from the repository due to file size and licensing considerations.
- Ensure all datasets are stored in the correct folder structure before running the notebook.

---

# Author

**Christoph Hüppi**\
Department of Geography\
University of Zurich (UZH)

GitHub Repository:
ChristophUZH/sds210-final-project: [https://github.com/ChristophUZH/sds210-final-project](https://github.com/ChristophUZH/sds210-final-project)

---

# License

This project was created for academic purposes as part of the SDS210 FS2026 course at the University of Zurich.

