# Data Dictionary: Feed Africa - Crop Yield & Climate

## 1. File Overview
| File Name | Description | Source |
| :--- | :--- | :--- |
| `yield_data.csv` | Annual yield for staple crops in Western Africa. | FAOSTAT (Production/Crops) |
| `fert_data.csv` | Nitrogenous and NPK fertilizer usage. | FAOSTAT (Inputs/Fertilizers) |
| `temp_data.csv` | Temperature change anomalies (Meteorological year). | FAOSTAT (Environment/Temp) |

## 2. Column Definitions (Common Fields)
- **Area**: The geographic region (e.g., "Western Africa" or "Ghana").
- **Year**: The calendar year of data collection (2003-2023).
- **Unit**: The metric used (e.g., kg/ha, Tonnes, °C).
- **Value**: The actual numeric measurement for that year.

## 3. Domain Specifics
### Yield Data (`yield_data.csv`)
- **Element**: "Yield"
- **Items**: Cassava, Yams, Maize (The primary staples for AfDB focus).
- **Unit**: **kg/ha** (Kilograms per Hectare). *Note: Must be converted to Tonnes if comparing directly to fertilizer mass.*

### Fertilizer Data (`fert_data.csv`)
- **Element**: "Agricultural Use"
- **Unit**: **t** (Tonnes).
- **Items**: Includes specific NPK mixes and Nitrogenous fertilizers.

### Climate Data (`temp_data.csv`)
- **Element**: "Temperature change"
- **Unit**: **°C** (Celsius).
- **Measurement**: Represents the change in temperature relative to the 1951-1980 baseline.

## 4. Known Issues & Data Quality
- **Granularity**: Yield and Temp are currently at the "Western Africa" regional level, while Fertilizer data contains country-specific entries (Ghana, Senegal, etc.). 
- **Missing Values**: Some years for specific fertilizers in smaller countries may show `0` or `null` due to reporting gaps.

## 📂 Data Provenance
Each file in this directory is derived from the following FAOSTAT domains:

| File | FAOSTAT Domain | Domain Code |
| :--- | :--- | :--- |
| `yield_data.csv` | Production: Crops and livestock products | **QCL** |
| `fert_data.csv` | Land, Inputs and Sustainability: Fertilizers by Product | **RFB** |
| `temp_data.csv` | Climate Change: Temperature change | **ET** |

**Extraction Date:** March 27, 2026  
**Method:** Manual Export (CSV)