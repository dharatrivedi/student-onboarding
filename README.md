# Student Onboarding Guide

**Aim:** Set up your local machine for research. This setup will also be useful when connecting to HPC resources.

## Step 1: Install Anaconda
**Task:** Manage Python environments and packages efficiently.

1. Download the Anaconda installer for your OS (Python 3.x) from [Anaconda Individual Edition](https://www.anaconda.com/products/individual).  
2. Run the installer and follow instructions.  
   - On Windows, select the option to add Anaconda to your PATH and make it the default Python.  
3. Verify installation by opening a terminal and running:  
conda --version

---

## Step 2: Create a Conda Environment
**Task:** Keep research dependencies isolated and reproducible.

1. Open your terminal.  
2. Create a new environment, for example:  
conda create -n research python=3.11
3. Activate the environment:  
conda activate research

4. Optional: Save your environment for sharing or backup:  


conda env export > setup/environment.yml


---

## Step 3: Install Jupyter Lab
**Task:** Use Jupyter for interactive Python learning and notebook-based workflows.

With your environment activated, run:  


conda install -c conda-forge jupyterlab


Verify installation:  


jupyter lab

This should open Jupyter Lab in your default browser.

---

## Step 4: Learn Python
Go through the [MolSSI Python Scripting for Computational Molecular Science](https://education.molssi.org/python_scripting_cms/index.html) tutorials to build a strong foundation.

---

## Optional Tips
- **Activate environment quickly:**  


conda activate research

- **Deactivate environment:**  


conda deactivate

- **Recreate environment from file (if provided):**  


conda env create -f setup/environment.yml


---

## Additional Resources
- [MolSSI Python Tutorial Notes](tutorials/molssi_python.md) – Optional detailed notes.  
- [Conda Cheat Sheet](https://docs.conda.io/projects/conda/en/latest/user-guide/cheatsheet.html)  
- [Jupyter Lab Documentation](https://jupyterlab.readthedocs.io/en/stable/)
