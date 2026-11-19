# Supernova Cosmology: Exploring Dark Energy and the Expansion of the Universe

## Project Overview

This project investigates the expansion history of the Universe using Type Ia supernova (SNIa) observational data.

The analysis explores the relationship between luminosity distance and redshift, comparing observational measurements with theoretical predictions from different cosmological models. Particular attention is given to the Lambda Cold Dark Matter (ΛCDM) model and the role of dark energy in explaining the accelerated expansion of the Universe.

Using Python, numerical integration and an exploratory Markov Chain Monte Carlo (MCMC) implementation, the project examines cosmological parameters, including the Hubble constant (H₀) and the dark energy density parameter (ΩΛ).

The project was undertaken as part of an Observational Cosmology tutorial in 2017.

## Project Objectives

The main objectives of this project are to:

- Import and analyse Type Ia supernova observational data.
- Incorporate intrinsic scatter into photometric measurement uncertainties.
- Calculate luminosity distances and theoretical distance-modulus predictions.
- Investigate the relationship between luminosity distance and cosmological redshift.
- Compare observational data against different theoretical cosmological models.
- Calculate distance-modulus residuals to investigate differences between theoretical predictions and observations.
- Explore the estimation of cosmological parameters using Markov Chain Monte Carlo (MCMC).
- Examine the distribution and confidence intervals of the dark energy density parameter.

## Methodology

The analysis follows several stages:

### 1. Data Preparation

Type Ia supernova observational data from the Union 2.1 compilation are imported and prepared for analysis.

An intrinsic scatter of 0.12 magnitudes is added in quadrature to the photometric uncertainties to obtain the total measurement uncertainty.

### 2. Cosmological Distance Calculations

Numerical integration is used to calculate comoving and luminosity distances as functions of redshift.

The luminosity distance is subsequently converted into distance modulus for comparison with the observational measurements.

### 3. Cosmological Model Comparison

The observational supernova data are compared with theoretical predictions from different cosmological models, including:

- ΛCDM with H₀ = 80, Ωm = 0.3 and ΩΛ = 0.7.
- A flat matter-dominated model with Ωm = 1 and ΩΛ = 0.
- ΛCDM with H₀ = 60, Ωm = 0.3 and ΩΛ = 0.7.

Distance-modulus residuals are also calculated to examine the differences between observational measurements and theoretical predictions.

### 4. MCMC Parameter Estimation

An exploratory MCMC implementation is used to investigate the estimation of the Hubble constant (H₀) and dark energy density parameter (ΩΛ), assuming a flat cosmological model.

The analysis includes parameter sampling, a two-dimensional scatter plot and a marginalised histogram of the dark energy density parameter.

### 5. Statistical Analysis and Visualisation

Matplotlib is used to visualise supernova observations, theoretical cosmological predictions, distance-modulus residuals and parameter distributions.

Percentile-based estimates are also explored to examine the uncertainty in the dark energy density parameter.

## Technologies and Libraries

- Python
- Jupyter Notebook
- NumPy
- Matplotlib
- SciPy
- Astropy

## Repository Structure

```text
supernova-cosmology-dark-energy/
│
├── README.md
│
├── Observational_Cosmology_Tutorial.ipynb
│
└── dataset/
    └── supernova.txt
```

*Note: The structure is illustrative. Update the dataset filename and folder structure to match the files uploaded to this repository.*

## Dataset

The project uses Type Ia supernova observational data from the Union 2.1 compilation.

Original data source:

http://supernova.lbl.gov/union/figures/SCPUnion2.1_mu_vs_z.txt

Dataset documentation:

http://supernova.lbl.gov/union/descriptions.html#Magvsz

## How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/supernova-cosmology-dark-energy.git
```

2. Navigate to the project directory:

```bash
cd supernova-cosmology-dark-energy
```

3. Install the required Python libraries:

```bash
pip install numpy matplotlib scipy astropy jupyter
```

4. Launch Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `Observational_Cosmology_Tutorial.ipynb` and execute the notebook cells.

Ensure the dataset is located in the appropriate directory and update the data-loading path if necessary.

## Project Context

This project was completed as part of an Observational Cosmology tutorial in 2017, focusing on the observational evidence for the accelerated expansion of the Universe and the role of dark energy.

The tutorial explores the scientific foundations behind the discovery of cosmic acceleration, associated with the 2011 Nobel Prize in Physics.

## Author

**Phumlani Phakathi**

Astrophysics Researcher | Data Analytics | Scientific Python

## Acknowledgements

- Observational Cosmology Tutorial (2017).
- Bruce Bassett – Tutorial material and scientific guidance.
- Union 2.1 Type Ia Supernova Compilation.
- Astropy, NumPy, SciPy and Matplotlib documentation.
