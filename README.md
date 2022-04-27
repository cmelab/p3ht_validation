# P3HT validation

P3HT dataset: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5911940.svg)](https://doi.org/10.5281/zenodo.5911940)

P3HT dataset was generated using [PlanckTon container v0.6.1](https://hub.docker.com/layers/169424362/cmelab/planckton_gpu/v0.6.1/images/sha256-c31a85f9f454b4b9b4568bd6ffc7508cbf998343bbaea863c8397cd4600f567d?context=repo) and [PlanckTon-flow](https://github.com/cmelab/planckton-flow/commit/d2e24a40c62dd49ccf64f7e177e016599c8aeb6a)

The steps to reproduce this study are as follows.
If you want to re-run the MD simulations, follow the steps in this first block--otherwise the complete simulation data can be downloaded from [United-atom P3HT workspace on Zenodo](https://doi.org/10.5281/zenodo.5911940) and you can skip to the analysis block:
  1. Pull our docker container (`docker pull cmelab/planckton_gpu:v0.6.1`).
  1. Clone planckton-flow (`git clone https://github.com/cmelab/planckton-flow`)
  1. Set the init file parameters (the exact init file is included in the zenodo dataset)
  1. Initialize and submit the workspace

The analysis can be run as follows:
  1. Clone the analysis notebook (`git clone https://github.com/cmelab/p3ht_validation`)
  1. Create and activate the conda environment using the environment file provided (`conda create -f environment.yml`)
  1. Move the planckton-flow directory into the analysis directory
  1. Run the notebook
