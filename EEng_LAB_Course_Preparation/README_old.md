# EEng LAB Course Preparation

Software we will be using during the course:

1. Anaconda Python distribution: https://www.anaconda.com/products/distribution#Downloads
1. notepad++ Text Editor (for Windows users only): https://notepad-plus-plus.org/
1. LTspice: https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html
1. LibreOffice: https://www.libreoffice.org/download/download-libreoffice/ 

## git 

We use git to provide the course material. You should familiarize yourself with git. A short introduction on how to use git is given [here](git.md).

## Create a New Conda Environment

For more information see the [**conda-cheatsheet.pdf**](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)

**On Windows:** Open an **Anaconda Powershell Prompt** (Start -> Anaconda3 -> Anaconda Powershell Prompt). 

**Other operating systems:** Open a terminal. 

On the command line prompt you should see an indicator which Python environment is currently active, e.g. `(base) PS C:\Users\me`

The token `(base)` shows the active environment.

The fastest way to create the necessary conda environment named `eeng` for this course is:

```
conda create -c conda-forge -n eeng python=3 jupyterlab numpy scipy matplotlib pandas ipywidgets

conda activate eeng

jupyter-lab
```

