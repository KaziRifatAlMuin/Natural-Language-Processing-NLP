# Natural Language Processing NLP

This repository contains two Jupyter notebook labs for basic NLP workflows:

- [1 - Text Preprocessing/lab1.ipynb](1%20-%20Text%20Preprocessing/lab1.ipynb)
- [2 - N-Gram/Lab2.ipynb](2%20-%20N-Gram/Lab2.ipynb)
- [2 - N-Gram/assignmentLab2.ipynb](2%20-%20N-Gram/assignmentLab2.ipynb)

## Prerequisites

- Python 3.10 or newer
- PowerShell on Windows
- Jupyter Notebook or JupyterLab

## Create And Activate A Virtual Environment

Open PowerShell in the repository root and run:

```powershell
python -m venv nlp_env
.\nlp_env\Scripts\Activate.ps1
python -m pip install --upgrade pip
```

If PowerShell blocks script execution, allow it for the current user first:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

## Install Dependencies

After activating the virtual environment, install the packages used in the notebooks:

```powershell
pip install jupyter notebook nltk numpy scikit-learn
```

Then download the required NLTK resources:

```powershell
python -m nltk.downloader punkt stopwords wordnet omw-1.4
```

## Run The Notebooks

Start Jupyter from the same virtual environment:

```powershell
jupyter notebook
```

If you use VS Code, select the `nlp_env` interpreter before opening the notebooks so the kernel matches the environment where the packages were installed.
