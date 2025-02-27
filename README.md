# HmmAnalysisRun3
A python-based Higgs to mu mu analysis for CMS Run 3

## Setting up environment 
(adapted from HH4b analysis)
### Creating a virtual environment

First, create a virtual environment (`micromamba` is recommended):

```bash
# Download the micromamba setup script (change if needed for your machine https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html)
# Install: (the micromamba directory can end up taking O(1-10GB) so make sure the directory you're using allows that quota)
"${SHELL}" <(curl -L micro.mamba.pm/install.sh)
# You may need to restart your shell
micromamba create -n h2mu python=3.10 -c conda-forge
micromamba activate h2mu
```
