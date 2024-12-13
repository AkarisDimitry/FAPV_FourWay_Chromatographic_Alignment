# Functional Alignment of Pure Vectors (FAPV) for Chromatographic Data

This repository contains a Python implementation of the Functional Alignment of Pure Vectors (FAPV) algorithm for processing and aligning four-way chromatographic data. The FAPV approach is designed to restore quadrilinearity in complex multiway datasets affected by shifts, warping, and severe overlap, enabling reliable quantitative analysis using standard multilinear models (e.g., PARAFAC).

---

## Introduction

Four-way LC-FS data often exhibit nonlinearities and poor selectivity due to chromatographic artifacts such as retention time shifts, peak shape distortions, and heavy spectral overlap. These issues frequently hinder the application of conventional multiway calibration models.

FAPV addresses these challenges by leveraging Functional Data Analysis (FDA) to:

1. Convert discrete raw data into functional representations.
2. Align and "re-warp" pure chromatographic profiles.
3. Restore quadrilinearity, allowing robust subsequent calibration with PARAFAC or other multilinear models.

---

## Key Features

- Functional treatment of chromatographic modes.
- Enhanced robustness against severe overlap and nonlinearity.
- Improved performance in both simulated and experimental scenarios.
- Compatibility with standard multilinear calibration methods (e.g., PARAFAC).

---

## Dependencies

- Python 3.x
- NumPy
- SciPy
- Matplotlib (optional)
- Additional dependencies listed in `requirements.txt`

---

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/FAPV_FourWay_Chromatographic_Alignment.git
cd FAPV_FourWay_Chromatographic_Alignment
pip install -r requirements.txt
```

---

## Usage

### 1. Data Preparation
Provide your four-way LC-FS data as a NumPy array or a suitable data structure.

### 2. Parameter Setup
Adjust parameters in the configuration script (e.g., `config.py`).

### 3. Run the Algorithm
Execute the following command:

```bash
python run_fapv.py
```

### 4. Subsequent Analysis
Use the aligned output data for standard multilinear calibration (e.g., PARAFAC).

---

## Example

Refer to `example.ipynb` for a step-by-step demonstration:

1. Load raw four-way data.
2. Apply FAPV.
3. Perform PARAFAC decomposition.
4. Evaluate prediction performance against other models (e.g., MCR-ALS, PARAFAC2).

---

## References

1. Lombardi, J.M., & Bortolato, S.A. (2018). Functional data analysis, a new approach to aligning three-way liquid chromatographic with fluorescence detection data. *Microchemical Journal, 142*, 219–228.
2. Montemurro, M., Siano, G.G., Alcaráz, M.R., & Goicoechea, H.C. (2017). Third order chromatographic-excitation–emission fluorescence data: Advances, challenges and prospects in analytical applications. *TrAC Trends in Analytical Chemistry, 93*, 119–133.
3. Parastar, H., & Tauler, R. (2014). Multivariate Curve Resolution of Hyphenated and Multidimensional Chromatographic Measurements: A New Insight to Address Current Chromatographic Challenges. *Analytical Chemistry, 86*, 286–297.
4. Olivieri, A.C., & Escandar, G.M. (2017). A road map for multi-way calibration models. *Analyst, 142*, 2862–2873.
5. Ramsay, J.O., & Silverman, B.W. (2005). *Functional Data Analysis* (2nd ed.). Springer.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For inquiries, please contact:

**Juan Manuel Lombardi**

**Fritz Haber Institute - Max-Planck-Gesellschaft**

**lombardi@fhi-berlin.mpg.de**

