# ⚡ Interactive Map of Tesla Charging Stations in Seattle

An interactive web map visualizing **Tesla Supercharger and Destination Charger** locations across the **Seattle metro area**, extending south past Burien.

---

## 🗺️ Overview
This project maps Tesla charging stations in the Seattle region to explore where Charging stations with J3400 Connectors are located

---

## 🧮 Data Sources
- **Charging Station Data:**  
  Provided by the [National Renewable Energy Laboratory (NREL)](https://www.nrel.gov) through the *Alternative Fuels Data Center (AFDC)* API.
- **Seattle Boundary:**  
  Custom GeoJSON boundary created using [geojson.io](https://www.geojson.io), manually adjusted to align with the coastline.

---

## 🧰 Tools & Workflow

| Tool | Purpose |
|------|----------|
| **Python (Pandas, GeoPandas)** | Cleaned and processed EV charging data |
| **GeoJSON** | Defined Seattle’s geographic boundary |
| **Mapbox / Javascript** | Built the interactive web map |

---

## 📊 Methodology Summary
1. Retrieved raw EV charging station data from the **NREL AFDC API**.  
2. Cleaned, filtered, and standardized fields in **Pandas**.  
3. Converted the dataset to a **GeoDataFrame** with **GeoPandas**.  
4. Clipped charger points to the Seattle GeoJSON boundary.  
5. Exported the processed data as a final **GeoJSON** for web visualization.

---

## 🌐 Visualization
The interactive map displays Tesla charging station locations as clickable points.  
Each marker includes details such as:
- Station name  
- Connector type and count  
- Street address  

You can pan, zoom, and explore charger clusters across Seattle.

---

## 📁 Files
| File | Description |
|------|--------------|
| `cleaned.geojson` | Cleaned dataset of Tesla charging stations |
| `seattle.geojson` | Custom Seattle coastline boundary |
| `index.html` | Interactive map output |

---

### 📍 Credits
Data sourced from [NREL.gov](https://www.nrel.gov).  
Seattle outline created using [geojson.io](https://www.geojson.io).  
Cleaned and processed in **Python** using **GeoPandas** and **Pandas**.

---

*Created by Jaeden Arnsdorf — University of Washington Geography / Data Science*
