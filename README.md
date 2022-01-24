# BIGMAP AI Cluster Expansion Exercises
This repository contains the execises for the 2022 BIG-MAP AI Workshop.

## Software Installation
All of the exercises will be done using Python within a Jupyter notebook.

The [CLEASE](https://clease.readthedocs.io) package will be used ([source](https://gitlab.com/computationalmaterials/clease)) for the cluster expansion models. The package is installable via `pip`, but requires a C++ compiler. This is generally not an issue on mac and linux, but usually is a little more difficult on Windows. Therefore, we recommend installing `clease` via anaconda if you're on windows, see below.

### Installation via pip
If you already have a python environment and a c++ compiler, you can install CLEASE via pip. we always recommend setting up a separate virutal environment before installing. From a terminal, do:

```shell
# Note, this is optional
python -m venv myenv
source activate myenv/bin/activate
```

Then install the required software:

```shell
pip install clease pandas tqdm jupyter
```
You can verify that `clease` is installed by running the command
```shell
clease --version
```
which should say `clease, version 0.10.8` (or higher).
### Installation via conda
Miniconda can be installed from [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html), which is our recommended version of anaconda.

Once that has been installed, open a new terminal. Note, on windows, you will now have a special anaconda terminal which you can use. In the new terminal, create a new virtual environment and install the software:

```shell
conda create -n myenv -y python=3.9                         # Create a new virtual venv named "myenv"
conda activate myenv                                        # Activate the new environment
conda install -y -c conda-forge clease pandas tqdm jupyter  # Install the required python packages
```
You can verify that `clease` is installed by running the command
```shell
clease --version
```
which should say `clease, version 0.10.8` (or higher).

## Running the exercises
First, if you didn't already download the exercises, we need to get them. We do this using git. From your terminal, fetch the exercises using `git` (if you're using `conda`, and it doesn't recognize the `git` command, do `conda install git`)
```shell
git clone https://github.com/atygesen/bigmap_clease_workshop.git
```
And then enter the new folder:
```shell
cd bigmap_clease_workshop
```
and finally, launch a new Jupyter notebook:
```shell
jupyter notebook
```

If you need to update your reposotory, e.g. due to any changes or updates to the exercises, go into the git repository and do
```shell
git pull
```
