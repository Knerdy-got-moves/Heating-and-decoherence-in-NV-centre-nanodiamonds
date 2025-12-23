# Heating and Decoherence in NV Centre Nanodiamonds

This repository contains theoretical and computational research on laser-induced heating and decoherence mechanisms in nitrogen-vacancy (NV) centre nanodiamonds. This work is relevant to quantum sensing applications, cavity optomechanics, and tests of quantum gravity using optically levitated nanodiamonds.

## Project Overview

This research investigates the thermal dynamics of NV centre nanodiamonds under laser illumination in the Rayleigh scattering regime. The work combines analytical derivations with numerical simulations to understand:

- **Laser heating mechanisms** in optically trapped nanodiamonds
- **Heat dissipation pathways** through gas collisions and blackbody radiation
- **Volumetric heat capacity** calculations for CVD and HTHP diamond nanocrystals
- **Decoherence processes** caused by phonon interactions
- **Temperature-dependent behavior** across various experimental conditions

## Repository Structure

### Documentation

- **`NV_centre_nanodiamond/`** - LaTeX source files for comprehensive theoretical treatment
  - `Chapters/` - Individual chapter files covering:
    - Chapter 1: Laser light heating in the Rayleigh regime
    - Chapter 2-4: Additional theoretical developments
  - `Appendix/` - Supplementary derivations and calculations
  - `Reference papers (not a bib file)/` - Organized literature on:
    - Cooling pathways
    - Diamond lattice dynamics
    - Dielectric properties
    - Optomechanics
    - Phonon interactions and quantum field theory
  - `Figures/` - Plots and diagrams
  - `main.tex` - Main document file

- **`Heating_decoherence_NVcentre_nanodiamonds.pdf`** - Compiled PDF of the theoretical work

### Computational Notebooks

- **`C_V_of_NV_CVD_HTHP_Diamond_and_Laser_heating.ipynb`**
  - Heat capacity (C_V) calculations from experimental data
  - Conversion from constant pressure (C_p) to constant volume (C_V)
  - Power-law fits for different temperature ranges (5-300 K)
  - Analysis of size effects and impurity contributions
  - Laser heating simulations with multiple parameters:
    - Temperature vs pressure relationships
    - Wavelength and intensity dependencies
    - Blackbody emission and absorption
    - Particle size effects

- **`Nanodiamond_TB_calculation.ipynb`**
  - Tight-binding band structure calculations for nanodiamonds

## Key Physics

### Heating Equation

The net temperature evolution is governed by:

```
V d[C_V(T-T_0)]/dt = P_laser - P_gas - P_blackbody
```

Where:
- **P_laser**: Absorption via electric dipole polarization in the Rayleigh regime
- **P_gas**: Cooling through thermal collisions with background gas
- **P_blackbody**: Radiative exchange with thermal environment

### Temperature Ranges

The heat capacity fits cover:
- Low temperature (5-30 K): C_V ∝ T^1.75
- Mid temperature (30-100 K): C_V ∝ T^2.4
- Extended range (15-100 K): C_V ∝ T^2.16

## Requirements

### For Jupyter Notebooks

```bash
numpy
scipy
matplotlib
pandas
```

Install with:
```bash
pip install numpy scipy matplotlib pandas
```

### For LaTeX Documentation

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- BibLaTeX with Biber backend
- Standard packages: amsmath, graphicx, hyperref, siunitx, etc.

## Usage

### Running the Simulations

Open the notebooks in Jupyter or Google Colab:

```bash
jupyter notebook C_V_of_NV_CVD_HTHP_Diamond_and_Laser_heating.ipynb
```

Or click the "Open in Colab" badge at the top of the notebook.

### Compiling the Documentation

```bash
cd NV_centre_nanodiamond
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

Or use Overleaf for online compilation.

## Applications

This research is relevant to:

- **Quantum optomechanics** with levitated nanodiamonds
- **Quantum sensing** using NV centres
- **Tests of quantum gravity** (QGEM experiments)
- **Cavity optomechanics** at cryogenic temperatures
- **Decoherence studies** in mesoscopic quantum systems

## Physical Parameters

Typical experimental conditions explored:
- Particle radius: 10 nm - 1 μm
- Laser wavelength: 532 nm - 1064 nm
- Laser intensity: 10 MW/m² - 10 GW/m²
- Background temperature: 5 K - 300 K
- Pressure: 10 Pa - 10⁵ Pa (vacuum to atmospheric)

## Current Status

**This is an ongoing research project.** Active development areas include:

- Refinement of dielectric constant values for NV centre diamonds
- Extension to non-spherical particle geometries
- Incorporation of quantum decoherence models
- Comparison with experimental data from levitation experiments
- Analysis of cooling pathways and ground-state cooling protocols

## References

Key theoretical foundations are drawn from:
- Rayleigh scattering and dipole approximation for small particles
- Planck blackbody radiation and Stefan-Boltzmann law
- Debye model for diamond heat capacity
- Equipartition theorem for gas collisions
- Classical and quantum optomechanics literature

See the `Reference papers (not a bib file)/` directory for detailed bibliography.

## License

[Specify license here]

## Contact

[Add contact information]

## Acknowledgments

This work builds upon experimental and theoretical advances in:
- NV centre physics and quantum sensing
- Levitated optomechanics
- Diamond materials science
- Cavity quantum optomechanics

---

**Note:** This research is actively being developed. Results and methods may be updated as the investigation progresses. For the most current findings, please refer to the latest commit or contact the authors directly.
