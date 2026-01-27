# SWE to MLE: The Code

This folder contains all the code samples for the "Software Engineer to Machine Learning Engineer" series.

## 🛠️ Environment Setup (One-time)

We use a single shared Conda environment (`swe2ml`) for all episodes.

### 1. Install Conda
If you don't have it, install [Miniconda](https://docs.anaconda.com/miniconda/).

### 2. Create the Environment
```bash
conda create -n swe2ml python=3.10 -y
conda activate swe2ml
```

### 3. Install Common Dependencies & Kernel
We need `ipykernel` so Jupyter can see this environment.

```bash
pip install jupyter scikit-learn matplotlib pandas numpy ipykernel
python -m ipykernel install --user --name=swe2ml
```

> [!TIP]
> **If the kernel doesn't show up immediately:**
> 1. **Refresh your browser tab** where Jupyter is open.
> 2. **Restart the Jupyter server**: Stop it with `Ctrl+C` in your terminal and run `jupyter notebook` again.
> 3. **VS Code users**: Click the "Select Kernel" button in the top right and select "swe2ml" from the list. If it's missing, click the refresh icon.

---

## 📂 Episodes

### [Episode 3: Your First Model (Digits)](episode-3/)
*   **Concepts**: Scikit-Learn API, K-Nearest Neighbors, Train/Test Split.
*   **Notebook**: [`digits_recognizer.ipynb`](episode-3/digits_recognizer.ipynb)

**To Run:**
```bash
cd episode-3
# (Optional) Ensure specific deps are installed
pip install -r requirements.txt
jupyter notebook digits_recognizer.ipynb
```
