# 🗺️ Kigali Land-Use and Population Analysis

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Data: OpenStreetMap](https://img.shields.io/badge/Data-OpenStreetMap-lightgrey)](https://www.openstreetmap.org)
[![Data: WorldPop](https://img.shields.io/badge/Data-WorldPop-yellowgreen)](https://www.worldpop.org)

A geospatial analysis of **land use, buildings, roads, and population distribution** in **Kigali, Rwanda**, using open-source data from **OpenStreetMap (OSM)** and **WorldPop**.  
The project integrates multiple datasets to derive spatial insights and visualize population density, infrastructure, and building usage.

---

## 📋 Objectives

- 🏙️ Download and process **land-use, building**, and **road** data from **OpenStreetMap**  
- 👥 Integrate **population raster data** (WorldPop, 2020) in people/km²  
- 📊 Compute **population per land-use type** and **density metrics**  
- 🗺️ Visualize the data via static and interactive maps (matplotlib + folium)  
- 🧮 Optionally generate summary charts and interactive dashboards  

---

## 🌍 Data Sources

| Dataset | Source | Description |
|----------|---------|-------------|
| **OpenStreetMap (OSM)** | [https://www.openstreetmap.org](https://www.openstreetmap.org) | Land use polygons, buildings, roads |
| **WorldPop (2020)** | [https://www.worldpop.org](https://www.worldpop.org) | Population raster (people per km²) |
| **SRTM (optional)** | [https://srtm.csi.cgiar.org](https://srtm.csi.cgiar.org) | Elevation data for terrain context |

---

## 🧠 Workflow Overview

```mermaid
graph TD
A[Download OSM Data] --> B[Extract Buildings & Roads]
B --> C[Download WorldPop Raster]
C --> D[Compute Population per Land-Use Zone]
D --> E[Visualize Choropleths & Density Maps]
E --> F[Export HTML/Folium Maps & Statistics]



