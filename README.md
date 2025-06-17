# ML_Tutorials

A hands-on collection of machine-learning tutorials and exercises for the USCMS PURSUE 2025 SPANet project.

Based on: https://github.com/UAPH451551/PH451_551_Sp25/tree/main






````markdown
## Quick Setup on macOS

Follow these steps to get up and running in **5 minutes**:

### 1. Install Miniconda (if you don’t have it)

```bash
brew install --cask miniconda
# Initialize Conda in your shell
conda init "$(basename "$SHELL")"
# Restart your terminal (or run `source ~/.zshrc` / `source ~/.bash_profile`)
````

---

### 2. Create & Activate a New Environment

```bash
# Create with Python 3.9
conda create -n ml_tutorials python=3.9 -y

# Activate it
conda activate ml_tutorials
```

> **Tip:**
>
> * Whenever you open a new terminal session, re-activate with:
>
>   ```bash
>   conda activate ml_tutorials
>   ```

---

### 3. Install Core Packages via Conda

```bash
# Jupyter, scikit-learn, NumPy, pandas, Matplotlib, PyTorch (CPU-only)
conda install -y \
  jupyterlab notebook \
  scikit-learn \
  numpy pandas matplotlib \
  pytorch torchvision cpuonly -c pytorch
```

---

### 4. Install Apple-Optimized TensorFlow via pip

```bash
pip install tensorflow-macos tensorflow-metal
```

---

### 5. Verify Your Setup

```bash
python - <<EOF
import sklearn, torch, tensorflow as tf
print("scikit-learn:", sklearn.__version__)
print("PyTorch:", torch.__version__, "| CUDA available?", torch.cuda.is_available())
print("TensorFlow:", tf.__version__, "| GPU/Metal:", tf.config.list_physical_devices())
EOF
```

---

### 6. Launch Jupyter

```bash
jupyter lab   # or: jupyter notebook
```

---

### 7. Deactivate When Done

To exit the environment and return to your base shell:

```bash
conda deactivate
```

Now open any notebook in `exercise/`—you’re ready to go!

```
```
