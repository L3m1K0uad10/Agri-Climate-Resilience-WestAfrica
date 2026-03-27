# 🌾 AI for "Feed Africa": Crop Yield Prediction

## 📌 1. Project Overview
This project addresses the **AfDB "High 5s"** priority to **Feed Africa**. We leverage Machine Learning to predict crop yields (Cassava, Yams, etc.) in Western Africa based on agricultural inputs and climate anomalies.

## 📁 2. Project Structure
- `analysis.ipynb`: Main Jupyter Notebook for modeling.
- `dataset/`:
    - `yield_data.csv`: Raw yield data.
    - `fert_data.csv`: Raw fertilizer data.
    - `temp_data.csv`: Raw climate data.
    - **`metadata.md`**: Technical data dictionary and column definitions.
- `README.md`: Project overview and AfDB alignment.

## 📊 3. The Data
We utilize three primary streams of data from FAOSTAT (2003-2023):
1. **Crop Yield**: Measured in kg/ha for regional staples.
2. **Fertilizer Usage**: Agricultural use measured in tonnes.
3. **Climate Change**: Temperature change anomalies in °C.

> 💡 *For a detailed breakdown of columns, units, and cleaning steps, see the [Dataset Metadata](datasets/metadata.md).*

## 🎯 4. Objectives
- **Identify Correlation**: How sensitive are West African staples to the current 1.5°C warming trend?
- **Predictive Modeling**: Build a regression model to forecast 2025 yields.
- **Policy Insight**: Provide data-driven recommendations for the AfDB’s "Climate-Smart Agriculture" investments.

## 🚀 5. How to Run
1. Clone the repository.
2. Ensure you have `pandas`, `matplotlib`, and `scikit-learn` installed.
3. Run `analysis.ipynb`.

## 📚 Data Attribution & Sources
The data used in this project is sourced from **FAOSTAT**, managed by the Food and Agriculture Organization of the United Nations (FAO).

* **Primary Source:** [FAOSTAT Database](https://www.fao.org/faostat/en/#data)
* **Citation:** FAO. 2024. FAOSTAT Statistical Database. Rome: FAO.
* **License:** Data is provided under the [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 IGO (CC BY-NC-SA 3.0 IGO)](https://creativecommons.org/licenses/by-nc-sa/3.0/igo/legalcode).

---
*Developed as an application of Predictive Analytics and Data Science to support Climate-Smart Agriculture and the AfDB "Feed Africa" initiative.*
