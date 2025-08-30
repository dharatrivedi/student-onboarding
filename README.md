# Student Onboarding Guide

**Aim:** Set up your local machine for research. This setup will also be useful when connecting to HPC resources.

---

## Step 1: Install Anaconda
**Task:** Manage Python environments and packages efficiently.

1. Download the Anaconda installer for your OS (Python 3.x) from [Anaconda Individual Edition](https://www.anaconda.com/products/individual).  
2. Run the installer:
   - **Windows:** Double-click the .exe file and follow the prompts. Check the box to add Anaconda to your PATH (recommended for simplicity, despite the installer’s warning) and make it the default Python.
   - **macOS/Linux:** Open a terminal, navigate to the download directory, and run the `.sh` installer:
     - Linux: `bash Anaconda3-latest-Linux-x86_64.sh`
     - macOS: `bash <replace-with-downloaded-filename>.sh`
       Follow the prompts, accept the license, and choose the installation location (default is `~/anaconda3`). Agree to initialize Conda by adding it to your shell’s startup file (e.g., `.bashrc` or `.zshrc`).
3. Verification: After installation, close and reopen your terminal to refresh the shell.
   Use `conda --version` to check your Conda installation.

---

## Step 2: Create a Conda Environment
**Task:** Keep research dependencies isolated and reproducible.

1. Open your terminal.  
2. Create a new environment, for example:  
`conda create -n research python=3.11`

3. Activate the environment:  
`conda activate research`

4. Optional: Save your environment for sharing or backup:  
`conda env export > setup/environment.yml`


---

## Step 3: Install Jupyter Lab
**Task:** Use Jupyter for interactive Python learning and notebook-based workflows.

With your environment activated, run:  
`conda install -c conda-forge jupyterlab`

Verify installation:  
`jupyter lab`

This should open Jupyter Lab in your default browser.

---

## Step 4: Learn Python
Go through the [MolSSI Python Scripting for Computational Molecular Science](https://education.molssi.org/python_scripting_cms/index.html) tutorials to build a strong foundation.

---

## Optional Tips
- **Activate environment quickly:**  
`conda activate research`

- **Deactivate environment:**  
`conda deactivate`

- **Recreate environment from file (if provided):**  
`conda env create -f setup/environment.yml`

---

## Additional Resources
- [MolSSI Python Tutorial Notes](tutorials/molssi_python.md) – Optional detailed notes.  
- [Conda Cheat Sheet](https://docs.conda.io/projects/conda/en/latest/user-guide/cheatsheet.html)  
- [Jupyter Lab Documentation](https://jupyterlab.readthedocs.io/en/stable/)
