# Enzyme Kinetics Analysis: Invertase Activity
![Language](https://img.shields.io/badge/language-Python%20%7C%20C-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-Active-success)

## 📖 Overview
This project analyzes the catalytic activity of the enzyme **Invertase** (β-fructofuranosidase), which hydrolyzes sucrose into glucose and fructose. 

By combining **biochemical experimentation** (DNS method) with **computational analysis** (Python & C), this repository demonstrates the calculation of kinetic parameters, specifically the **Michaelis Constant ($K_m$)** and **Maximum Reaction Velocity ($V_{max}$)**, using the Michaelis-Menten equation and Lineweaver-Burk plots.

## 🧬 Scientific Background
* **Enzyme:** Invertase (EC 3.2.1.26)
* **Substrate:** Sucrose
* **Method:** DNS (3,5-Dinitrosalicylic acid) assay to measure reducing sugars.
* **Kinetics Model:** Michaelis-Menten kinetics.

## 🛠 Technologies & Skills
This project bridges the gap between molecular biology and data science.

* **Python (Pandas, NumPy, Matplotlib):** Used for data cleaning, statistical regression, and visualization of reaction curves.
* **C Language:** Used for implementing raw data processing algorithms to handle large datasets efficiently.
* **Laboratory Techniques:** Spectrophotometry (Absorbance at 540nm), Preparation of standard curves.

## 📊 Methodology & Analysis workflow

1.  **Data Collection:** Measured absorbance (OD540) at various substrate concentrations $[S]$.
2.  **Conversion:** Converted absorbance to product concentration $[P]$ using a glucose standard curve.
3.  **Velocity Calculation:** Calculated initial reaction velocity $V_0$.
4.  **Parameter Estimation:** Applied linear regression to the **Lineweaver-Burk plot** ($1/V_0$ vs $1/[S]$) to derive:
    * $V_{max}$ (y-intercept)
    * $K_m$ (slope)

### Visualization
![Image](https://via.placeholder.com/600x400?text=Insert+Your+Graph+Image+Here)

*Figure 1: The saturation curve showing the relationship between substrate concentration and reaction velocity.*

## 🚀 How to Run
To reproduce the analysis, clone this repository and run the Python script.

```bash
# Clone the repository
git clone [https://github.com/yoshinight/enzyme-kinetics-analysis.git]

# Navigate to the directory
cd enzyme-kinetics-analysis

# Run the analysis script
python analysis.py
