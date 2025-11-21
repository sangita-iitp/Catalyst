# Machine Learning–Assisted Prediction of Tetracycline Photocatalytic Degradation

**Authors:**  
Palkaran Sethi • Dr. Sangita Roy • Dr. Soumen Basu*  
**Affiliations:**  
Department of Chemistry and Biochemistry & Department of Computer Science and Engineering,  
Thapar Institute of Engineering and Technology, Patiala-147004, Punjab, India  
**For further query:** soumen.basu@thapar.edu, sangita.roy@thapar.edu  

---

## 📘 Overview
This repository contains all data and code associated with the manuscript:

> **Machine Learning-Assisted Prediction of Tetracycline Photocatalytic Degradation: Bridging Experimental and Computational Insights**  
> (Submitted to *Digital Discovery*, Royal Society of Chemistry)

The project integrates **experimental photocatalytic data** and **synthetic data generated using Generative Adversarial Networks (GANs)** to predict tetracycline (TC) degradation efficiency.  
A total of 19 regression algorithms were evaluated, and the **Random Forest Regressor** achieved the highest predictive accuracy (R² = 0.9921, RMSE = 0.0071, MAPE = 0.0039).

---

## 📂 Repository Structure
Catalyst/
│
├── Catalyst data_300.xlsx        # 📊 Final dataset (19 real + 300 GAN-generated samples)
|
├── readme.md                     # 📘 Main documentation (project overview, dataset, instructions)
│
├── LICENSE                       # ⚖️ License file (e.g., Creative Commons Zero v1.0 Universal)



---

## 📊 Dataset Description
**File:** `Catalyst_data_300.xlsx`  
**Total entries:** 319 (19 original + 300 GAN-generated)

| Column | Description | Units |
|:--|:--|:--|
| `Catalyst` | Photocatalyst identifier (e.g., TiO₂-P25, g-C₃N₄, 13GS) | text |
| `Rate Constant (k)` | Pseudo-first-order kinetic constant | min⁻¹ |
| `Synergy Factor (SF)` | Quantifies interfacial enhancement | dimensionless |
| `Apparent Quantum Efficiency (AQE)` | Fraction of photons contributing to reaction | % |
| `Catalytic Efficiency (CE)` | Pollutant degraded per unit mass/time | % |
| `Degradation Efficiency (%)` | Target variable for ML models | % |

**Data origin:**
- **19 original samples:** extracted from previously published works by Basu *et al.* (see manuscript references 28–33).  
- **300 synthetic samples:** produced using a **GAN model** trained on the numerical descriptors of the original dataset, ensuring statistical realism.  
  Catalytic efficiency values were refined using a base Random Forest model.

---

 








