# ML_Tutorials

A hands-on collection of machine-learning tutorials and exercises for the USCMS PURSUE 2025 SPANet project.

Based on: https://github.com/UAPH451551/PH451_551_Sp25/tree/main

---

## 🖥 Quick Setup on macOS

Follow these steps to get up and running in **5 minutes**:

1. **Install Miniconda** (if you don’t have it)

    ```bash
    brew install --cask miniconda
    conda init "$(basename "$SHELL")"
    # Restart your terminal (or run `source ~/.zshrc` / `source ~/.bash_profile`)
    ```

2. **Create & Activate a New Environment**

    ```bash
    conda create -n ml_tutorials python=3.9 -y
    conda activate ml_tutorials
    ```

    > **Tip:** Each time you open a new terminal, run  
    > `conda activate ml_tutorials`

3. **Install Core Packages via Conda**

    ```bash
    conda install -y \
      jupyterlab notebook \
      scikit-learn \
      numpy pandas matplotlib \
      pytorch torchvision cpuonly -c pytorch
    ```

4. **Install Apple-Optimized TensorFlow via pip**

    ```bash
    pip install tensorflow-macos tensorflow-metal
    ```

5. **Launch Jupyter**

    ```bash
    jupyter lab   # or: jupyter notebook
    ```

6. **Deactivate When Done**

    ```bash
    conda deactivate
    ```

---

Now open any notebook in `exercise/`—you’re ready to go!  


:)
