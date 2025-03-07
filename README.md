# LondonMet Quantum Tutorials

## Installation

### Python

If you don't have a python version more recent than 3.11, install a newer version.

1. Install 3.13 on your PC from the (python download page)[https://www.python.org/downloads/].

    It is ususally better to deselect 'Install for all users' and have python install into a directory under your home directory.

1. somethin

### GitHub

1. If you have a windows machine, install (git bash for windows)[https://dscho.github.io/git-for-windows.github.io/]

1. On GitHub, fork the repo from (skingham / londonmet_quantum_tutorials)[https://github.com/skingham/londonmet_quantum_tutorials]

1. Clone your fork:
    ```sh
    git clone git@github.com:<your_github_login_name>/londonmet_quantum_tutorials.git
    cd londonmet_quantum_tutorials
    ```


### IBM QISKIT Setup

Follow the (QISKIT install procedure)[https://quantum.cloud.ibm.com/docs/en/guides/install-qiskit].

1. Create a virtual environment (e.g. conda or venv)
    * Pip:
        1. Create environment:     
            ```sh
            python -m venv .venv
            ```
        1. Activate the environment
            * Windows Powershell
                ```powershell
                .venv\scripts\activate.ps1
                ```
            * Windows Git Bash
                ```sh
                source .venv/scripts/activate
                ```
            * Windows command prompt:
                ```sh
                .venv\Scripts\activate
                ```
            * Linux/Mac
                ```sh
                source .venv/bin/activate
                ```
        1. Install packages:
            ```sh
            python -m pip install qiskit[visualization] qiskit-ibm-runtime qiskit_aer qiskit_addon_aqc_tensor jupyter
            ipython kernel install --user --name=ibm-qiskit
            ```
    * Conda:
        1. Create environment:
            ```sh
            conda create -c conda-forge --name 'ibm-qiskit' python=3.13
            ```
        1. Activate environment: 
            ```sh
            conda activate ibm-qiskit
            ```
        1. Install packages:
            ```sh
            conda install -c conda-forge qiskit qiskit-ibm-runtime jupyter seaborn pydot pylatexenc wrapt rich
            python -m pip install qiskit_aer qiskit_addon_aqc_tensor 
            ipython kernel install --user --name=ibm-qiskit
            ```
1. Create an [IBM account](https://www.ibm.com/account/reg/us-en/signup?formid=urx-19776).
    * You need a free IBMid account to access documentation.
    * There is a separate product for gaining access to quantum computing resources that we will look at later.

### 

### Release notes

Lots of changes between tutorials and current release.  (QISKIT release notes)[https://docs.quantum.ibm.com/api/qiskit/release-notes]

## Start Up Jupyter

```sh
jupyter notebook notebooks
```

The first notebook is from IBM's (hello world example)[https://docs.quantum.ibm.com/guides/hello-world].

## Resources

Github repo from (Los Alamos National Laboratory Quantum Algorithms)[https://github.com/lanl/quantum_algorithms].  
This accompanites (Quantum Algorithm Implementations for Beginners)[https://doi.org/10.1145/3517340].



