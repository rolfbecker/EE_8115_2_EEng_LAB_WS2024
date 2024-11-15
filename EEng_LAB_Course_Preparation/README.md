# EEng Lab Course Preparation

## (1) Prepare your Jupyter Python Environment

You will use our prepared **Jupyter Notebooks** to work on the exercises. They contain safety instructions, description of the experiments' setup, instructions how and what to measure, as well as runnable Python code to perform the data analysis.

You will run the Jupyter Notebooks in the **Jupyter Lab** development environment which is executed in a browser (preferably Chrome, Chromium or Edge).

We propose two ways to **make use of Jupyter Lab**. 

(1) Either use the **Jupyter Hub** server operated by the **HSRW Earth Observtion Lab**, which provides a personal Jupyter Lab environment for the HSRW students, <br>
(2) or install your own Python system on your own computer. We highly recommend to use the **Anaconda Python Distribution**!

### Alternative (A):  Use the Jupyter Hub of the HSRW EO-Lab

Go to [https://hub.eolab.de/](http://hub.eolab.de/) an log in with your university credentials.

### Alternative (B): Local Anaconda Python Installation 

In case you do not want to or cannot use the HSRW EO-Lab's Jupyter Hub you should install Anaconda locally. Anaconda is a powerful Python distribution also providing the Jupyer Lab development system for Python.

#### (B.1) Install Anaconda

Find the official installation instructions here:

* [Install Anaconda](https://docs.anaconda.com/anaconda/install/index.html)

#### (B.2) Create a New Conda Environment

Python environments allow for separate parallel project specific software installations which are independent from each other. These environments are used to provide a conflict free software installation for a specific task. 

* [Create a Conda Environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

**On Windows:** Open an **Anaconda Powershell Prompt** (Start -> Anaconda3 -> Anaconda Powershell Prompt). 

**Other operating systems:** Open a terminal. 

On the command line prompt you should see an indicator which Python environment is currently active, e.g. `(base) PS C:\Users\me`

The token `(base)` shows the active environment.

The fastest way to create the necessary conda environment named `eeng` for this course is:

```
conda create -c conda-forge -n eeng python=3 jupyterlab numpy scipy matplotlib pandas ipywidgets pyserial bqplot
```

This command installs packages from the **conda-forge** software 'channel'. A channel is a online software source, a huge repository providing the software packages for installation.

After successful creation **activate** the environment and start **jupyter-lab** from within the environment.

```
conda activate eeng

jupyter-lab
```

## (2) Clone or Download the EEng Lab Notebook Repository from Git

We use this git repository to disseminate the course material. The are two alternatives to get the lab notebooks.

**Alternative (A): Use a Git client.**

Use a Git client to **clone the repository** regularly. More on Git **[here](./eeng0020_LAB_Course_Preparation/git.md)**. 

Open a terminal in your intended Python (conda) environment. On the command line interface (CLI) execute:

```
git clone https://github.com/rolfbecker/EE_8115_2_EEng_LAB_WS2024.git
``` 

**Alternative (B): download the zipped repository.**

Alternatively you can also **download the zipped repository**. Go to the [repository homepage](https://github.com/rolfbecker/EE_8115_2_EEng_LAB_WS2024) and click on the green botton at the upper right corner. Choose "Download zip" and save the zip archieve to an appropriate folder on your harddrive. Go to this folder and **really unzip** the archieve. Do not just click and enter it!




