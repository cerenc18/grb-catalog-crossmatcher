# Multi-Mission GRB & Solar Flare Catalog Analysis

This repository contains Python-based analytical pipelines designed to compare, cross-match, and visualize high-energy astrophysical catalogs from multiple missions, specifically **Fermi (GBM/LAT)** and **Neil Gehrels Swift Observatory**.

## 🚀 Key Features

* **Temporal Comparison (GBM vs LAT) [`01_catalog_crossmatching.ipynb`]:** Merges independent event catalogs based on timestamps, normalizes data, and computes flux parameter differences.
* **Spatial Cross-Matching (Swift vs Fermi):** Iterates through Gamma-Ray Burst (GRB) coordinate lists to find potential multi-instrument observations within a defined spatial tolerance (**1.0°** radius).
* **Mollweide Sky Map Projection [`02_grb_skymap_projection.ipynb`]:** Visualizes the spatial distribution of thousands of GRBs on a full-sky map, applying coordinate transformations (RA shifting) to plot standard angular data into an equatorial projection.
* **Burst Classification:** Automatically categorizes GRBs into standard short ($T_{90} < 2.0$ s) and long ($T_{90} \geq 2.0$ s) populations.

## 📂 Repository Structure
* `notebooks/`: Contains the core analysis scripts.
* `outputs/`: Contains the generated data visualizations (Gaussian fits, pie charts, Sky Maps) and a comprehensive project poster (`Project_Poster_TR.pdf`) originally presented for this study.

## 🛠 Skills Demonstrated
* **Data Engineering:** `pandas` (cleaning, datetime normalization, cross-matching).
* **Coordinate Systems:** Transforming standard Right Ascension/Declination coordinates for complex map projections.
* **Data Visualization:** `matplotlib` (Mollweide projections, multi-layered scatter plots).

## 📄 Authorship & Usage
Developed by **Ceren C.** This repository serves as a demonstration of applying data science methodologies to astrophysical catalog integration. 
*(Note: Sample data directories are referenced in the code; full proprietary datasets are excluded for privacy).*
