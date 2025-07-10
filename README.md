## Confusion-Driven Machine Learning of Structural Phases of a Flexible, Magnetic Stockmayer Polymer

This repository contains the analysis code and processed data files necessary to reproduce the main plots in the paper:

**"Confusion-driven machine learning of structural phases of a flexible, magnetic Stockmayer polymer"**  
Dilina Perera, Samuel McAllister, Joan Josep Cerdà, and Thomas Vogel, *J. Chem. Theory Comput.* (2025)  
[https://doi.org/10.1021/acs.jctc.5c00381](https://doi.org/10.1021/acs.jctc.5c00381) 

---

## 📁 Repository Structure

- `notebook/` – The Jupyter notebook that implements the **confusion scheme** for identifying stucutral transitions in Stockmayer polymers
  - `confusion_method.ipynb`
- `results/` – Processed data files used to generate the main plots in the paper (to be added)
- `requirements.txt` – Python package dependencies for running the notebook
- `LICENSE` – MIT License
- `README.md` – This file
- `.gitignore`

---

## 📄 Description

The `confusion_method.ipynb` notebook implements the **confusion scheme**—a semi-supervised, neural-network-based machine learning technique for identifying phase transitions (originally introduced in *E. van Nieuwenburg, Y. Liu, and S. Huber, Nature Phys. 13, 435 (2017)*).

This code applies the confusion method to detect structural transitions in magnetic Stockmayer polymers using either monomer position data or magnetic dipole moment data as input.

---

### 📊 Input Data

Due to file size, the raw configuration data required as input to `confusion_method.ipynb` is not included in this repository.  
Data for two different values of the parameter η (η = 0.02 and η = 0.06) are available via Zenodo.

**Download links:**
- [`data_eta_0.02.tar.gz`](https://zenodo.org/records/15851811/files/data_eta_0.02.tar.gz)  
- [`data_eta_0.06.tar.gz`](https://zenodo.org/records/15851811/files/data_eta_0.06.tar.gz)

After downloading, extract the files into the root directory so that folders like `data_eta_0.02/` exist.

---

### 📦 Requirements

Before running the notebook, make sure the following Python libraries are installed:

- `tensorflow` ≥ 2.8  
- `numpy` ≥ 1.21  
- `pandas` ≥ 1.3  
- `matplotlib` ≥ 3.4  
- `scikit-learn` ≥ 0.24  

You can install all dependencies using the `requirements.txt` file included in this repository. Run the following command in a terminal:

```bash
pip install -r requirements.txt
```

---

> This notebook is part of the supporting materials for our JCTC paper and is intended for academic use. Please cite the paper if you use or adapt this code.

---

### Code Authors

Developed by **Dilina Perera** and **Samuel McAllister**.

For questions, please contact:
- Dilina Perera – `dilina.perera [at] ung.edu`
- Samuel McAllister – `smcallis [at] uab.edu` 

