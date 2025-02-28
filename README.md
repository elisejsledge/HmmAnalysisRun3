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
#create it in /nobackup/micromamba NOT in $HOME

[esledge@cmslpc333 nobackup]$ "${SHELL}" <(curl -L micro.mamba.pm/install.sh)
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
100  3059  100  3059    0     0   2583      0  0:00:01  0:00:01 --:--:--  2583
Micromamba binary folder? [~/.local/bin] .local/bin
Init shell (bash)? [Y/n] y
Configure conda-forge? [Y/n] y
Prefix location? [~/micromamba] /uscms/home/esledge/nobackup/micromamba

# You may need to restart your shell or run source ~/.bashrc
source ~/.bashrc
micromamba create -n h2mu python=3.10 root -c conda-forge
micromamba activate h2mu
```

### Installing packages

**Remember to install this in your mamba environment**.
(Looks like numba, numpy

```bash
# Clone the repository
git clone git@github.com:elisejsledge/HmmAnalysisRun3.git
cd HmmAnalysisRun3
# install requirements
pip3 install -r requirements.txt
```
