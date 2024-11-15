## Prepare your Jupyter Python Environment

You will use our prepared **Jupyter Notebooks** to work on the exercises. They contain safety instructions, description of the experiments' setup, instructions how and what to measure, as well as runnable Python code to perform the data analysis.

You will run the Jupyter Notebooks in the **Jupyter Lab** development environment which is executed in a browser (preferably Chrome, Chromium or Edge).

We propose two ways to make use of Jupyter Lab. 

(1) Either use the **Jupyter Hub** server operated by the **HSRW Earth Observtion Lab**, which provides a personal Jupyter Lab environment for you, <br>
(2) or install your own Python system on your own computer. We highly recommend to use the **Anaconda Python Distribution**!

## (1) Use the Jupyter Hub of the HSRW EO-Lab

Go to [https://hub.eolab.de/](http://hub.eolab.de/) an log in with your university credentials.

## (2) Create a New Conda Environment

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