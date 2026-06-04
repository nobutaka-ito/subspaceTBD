# Subspace Track-before-Detect for Passive Multi-Target Tracking with Unknown Emitted Signals
This repository provides a Python notebook for passive multi-target track-before-detect (TBD) under unknown emitted signals. The notebook presents a comparative simulation study between the proposed subspace TBD method based on the Bingham likelihood and a conventional TBD method based on a Gaussian likelihood, evaluated under identical trajectories, observations, and random seeds. 
The simulation considers microphones placed uniformly along the perimeter of a square room, sinc-correlated noise, soft spatial boundary weighting, and a particle-filter-based TBD framework. The notebook generates synthetic multichannel observations, applies both likelihood models, and visualizes the resulting target position estimates together with the root mean square error (RMSE).
Copyright (c) 2026 National Institute of Advanced Industrial Science and Technology (AIST). Licensed under CC BY-SA 4.0.
## Software Requirements
The notebook is written in Python and depends mainly on NumPy, Matplotlib, and FilterPy.
## Quick Start
1.	Clone this repository.
```bash
git clone <repository-url>
cd <repository-directory>
```
2.	Create a virtual environment and install the required packages.
```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install numpy matplotlib filterpy jupyter
```
3.	Launch Jupyter and run all cells in the notebook.
```bash
jupyter notebook
```
## Methodological Overview
The notebook consists of the following components:
- Definition of simulation parameters and microphone configuration.
- Generation of target activity patterns and trajectories.
- Simulation of multichannel observations with correlated noise.
- Particle-filter-based TBD using Gaussian and Bingham likelihoods.
- Visualization of estimated trajectories, time-varying tracking error, and final RMSE.
## Citation
If this repository contributes to your research, please cite the following reference:
```bibtex
@misc{ito2026subspacetrackbeforedetectpassivemultitarget,
  title={Subspace Track-before-Detect for Passive Multi-Target Tracking with Unknown Emitted Signals},
  author={Nobutaka Ito and Yoshiaki Bando},
  year={2026},
  eprint={2605.25498},
  archivePrefix={arXiv},
  primaryClass={eess.AS},
  url={https://arxiv.org/abs/2605.25498}
}
```
## License
This repository is distributed under the Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0).
