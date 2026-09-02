# ICELLI 2026: Time Series Analysis in Space Physics
## *A Practical Python Workflow for Ionospheric and Geomagnetic Data*

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Presenter:** Bello Saeed Abioye  
**Affiliation:** Department of Physics, University of Ilorin, Nigeria  
**Email:** [bello.sa@unilorin.edu.ng](mailto:bello.sa@unilorin.edu.ng)  
**ORCiD:** [0000-0002-5527-1110](https://orcid.org/0000-0002-5527-1110)

---

## 📖 Overview

This repository contains the interactive hands-on tutorials, Python workflows, and datasets presented at **ICELLI 2026**. The tutorial introduces undergraduate and postgraduate space physics researchers to modern, reproducible time-series analysis workflows using Python's scientific ecosystem (`pandas`, `numpy`, and `matplotlib`).

---

## 🚀 Interactive Google Colab Notebooks

Each module is self-contained and ready to execute in **Google Colab** with one click:

| Module | Notebook | Topics & Techniques | Launch in Colab |
| :--- | :--- | :--- | :---: |
| **Module 1** | [`iono_main.ipynb`](iono_main.ipynb) | **Ionospheric Characteristics**: Loading DIDBase/Ionosonde data (IL008), data cleaning, diurnal & seasonal variations of $foF2$, $hmF2$, and peak electron density ($NmF2$). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME/blob/main/iono_main.ipynb) |
| **Module 2** | [`mag_main.ipynb`](mag_main.ipynb) | **Geomagnetic Variations**: Processing SuperMAG 60s magnetometer data for Ilorin (`ILR`), calculating Horizontal Intensity ($H$), night-time baseline subtraction (Rabiu et al., 2007), Solar Quiet ($Sq$) variation, and storm-time correlation with $Dst$ indices. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME/blob/main/mag_main.ipynb) |
| **Module 3** | [`tec_main.ipynb`](tec_main.ipynb) | **GNSS Total Electron Content (TEC)**: Ingestion of GOPI GPS receiver outputs, batch processing of multi-day `.Cmn` files, vertical TEC ($VTEC$) diurnal patterns, and ionospheric scintillation ($S_4$) overview. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME/blob/main/tec_main.ipynb) |

> **Note for Colab Users:** When running on Google Colab, execute **Cell 1** at the top of each notebook to automatically clone this repository and load the required datasets.

---

## 📂 Repository Structure

```text
├── iono_main.ipynb             # Module 1: Ionosonde analysis notebook
├── iono_main.py                # Jupytext synced Python script (Module 1)
├── mag_main.ipynb              # Module 2: Geomagnetic time-series notebook
├── mag_main.py                 # Jupytext synced Python script (Module 2)
├── tec_main.ipynb              # Module 3: GNSS-TEC analysis notebook
├── tec_main.py                 # Jupytext synced Python script (Module 3)
│
├── ILR_data.txt                # Dataset: Ilorin Ionosonde (IL008) parameters
├── SuperMAG_60s_ILR_2009.csv   # Dataset: SuperMAG 1-minute geomagnetic data
├── indices_data.txt            # Dataset: Geomagnetic indices (Dst, Kp, ap)
├── CGGN-2014_TEC_Data/         # Dataset: Daily GPS-TEC (.Cmn) files from CGGN station
│
├── baseline_source.png         # Illustration: Geomagnetic baseline derivation methodology
├── CGGN-20120704-NW.JPG        # Illustration: CGGN GNSS receiver station
├── .gitignore                  # Git ignore rules for clean workspace
└── README.md                   # Repository documentation and Colab launcher
```

---

## 💻 Local Setup (Running on your Computer)

If you prefer to run the tutorials locally in VS Code or JupyterLab:

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

### 2. Install required dependencies
```bash
pip install pandas numpy matplotlib scipy jupytext
```

### 3. Launch JupyterLab or Notebook
```bash
jupyter lab
```

---

## 📚 Data Sources & References

- **DIDBase (GIRO Data Center):** [https://giro.uml.edu/didbase/scaled.php](https://giro.uml.edu/didbase/scaled.php) — Ionogram-scaled parameters from the Global Ionosphere Radio Observatory.
- **SuperMAG Collaboration:** [https://supermag.jhuapl.edu/](https://supermag.jhuapl.edu/) — Global ground-based magnetometer network data.
- **WDC for Geomagnetism, Kyoto:** [https://wdc.kugi.kyoto-u.ac.jp/](https://wdc.kugi.kyoto-u.ac.jp/) — Geomagnetic activity indices ($Dst$, $Kp$).
- **Rabiu, A. B. et al. (2007):** *Solar quiet (Sq) variation of the magnetic field along the 96° MM at the dip equator.*

---

## 📄 License
This educational material is licensed under the [MIT License](LICENSE).
