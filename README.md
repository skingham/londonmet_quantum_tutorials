# LondonMet Quantum Tutorials

## Installation

### Python

If you don't have a python version more recent than 3.11, install a newer version.

1. Install 3.10 on your PC from the [python download page](https://www.python.org/downloads/).

    It is ususally better to deselect 'Install for all users' and have python install into a directory under your home directory.

1. somethin

### GitHub

1. If you have a windows machine, install [git bash for windows](https://dscho.github.io/git-for-windows.github.io/)

1. On GitHub, fork the repo from [skingham / londonmet_quantum_tutorials](https://github.com/skingham/londonmet_quantum_tutorials)

1. Clone the repo:

    ```sh
    git clone git@github.com:<your_github_login_name>/londonmet_quantum_tutorials.git
    cd londonmet_quantum_tutorials
    ```


### IBM QISKIT Setup

Follow the [QISKIT install procedure](https://quantum.cloud.ibm.com/docs/en/guides/install-qiskit).

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
            python -m pip install qiskit[visualization] qiskit-ibm-runtime qiskit_aer qiskit_addon_aqc_tensor jupyter tweedledum qiskit-algorithms
            ipython kernel install --user --name=ibm-qiskit
            ```

    * Conda:
        1. Create environment:

            ```sh
            conda create -c conda-forge --name 'ibm-qiskit' python=3.10
            ```

        1. Activate environment:

            ```sh
            conda activate ibm-qiskit
            ```

        1. Install packages:

            ```sh
            conda install -c conda-forge qiskit qiskit-ibm-runtime jupyter seaborn pydot pylatexenc wrapt rich tweedledum qiskit-algorithms
            python -m pip install qiskit_aer qiskit_addon_aqc_tensor 
            ipython kernel install --user --name=ibm-qiskit
            ```

1. Create an [IBM account](https://www.ibm.com/account/reg/us-en/signup?formid=urx-19776).
    * You need a free IBMid account to access documentation.
    * There is a separate product for gaining access to quantum computing resources that we will look at later.

### Hardware access

[Create an account](https://)

### Release notes

Lots of changes between tutorials and current release.  [QISKIT release notes](https://docs.quantum.ibm.com/api/qiskit/release-notes)

## Start Up Jupyter

```sh
jupyter notebook notebooks
```

The first notebook is from IBM's [hello world example](https://docs.quantum.ibm.com/guides/hello-world).

## Resources

Github repo from [Los Alamos National Laboratory Quantum Algorithms](https://github.com/lanl/quantum_algorithms).  
This accompanites [Quantum Algorithm Implementations for Beginners](https://doi.org/10.1145/3517340).



### Maths

[Quantum Computing (CST Part II) Lecture 2: Linear Algeba](https://www.cl.cam.ac.uk/teaching/1920/QuantComp/Quantum_Computing_Lecture_2.pdf)

[Prof. MacLen- nan’s Unconventional Computation course Chapter III](https://web.eecs.utk.edu/~bmaclenn/Classes/494-594-UC-F13/handouts/LNUC-III.A.pdf)

[Quantum Mechanics and Quantum Computing: an Introduction](http://www.macs.hw.ac.uk/~des/qcnotesaims17.pdf)

[All the Math you'll need](https://www.intoquantum.pub/p/all-the-math-that-you-need-to-start-312)

[Maths for Quantum Computing- A brief Introduction of Quantum Computing (Part 2)](https://kakashi007.medium.com/maths-for-quantum-computing-a-brief-introduction-of-quantum-computing-part-2-4322c1ab140d)

[Lecture 1: Axioms of QM + Bell Inequalities](https://people.eecs.berkeley.edu/~vazirani/s09quantum/notes/lecture1.pdf)

[Lecture 2: Quantum Algorithms](https://people.eecs.berkeley.edu/~vazirani/s09quantum/notes/lecture2.pdf)

[Quantum Computing: Foundations to Frontier](https://www.henryyuen.net/fall2019/scribe1-2.pdf)

[An introduction to the theory of quantum groups](https://dc.ewu.edu/cgi/viewcontent.cgi?params=/context/theses/article/1035/&path_info=Ryan_Downie_Final_Thesis_Spring_2012.pdf)

## Hadamard and Single Qubit

[measure-a-state-in-hadamard-basis](https://quantumcomputing.stackexchange.com/questions/17798/measure-a-state-in-hadamard-basis)

[Basic Quantum Computing - Super dense coding](https://medium.com/@charlie.thomas_94667/basic-quantum-computing-super-dense-coding-279eeaf233d8)

[Demystifying Superdense Coding](https://medium.com/qiskit/demystifying-superdense-coding-41d46401910e)

[](https://www.monoidal.net/papers/tutorialqpl-1.pdf)

[What Bell Did](https://arxiv.org/pdf/1408.1826)

[Simulating a Quantum Computer](https://medium.com/data-science/simulating-a-quantum-computer-with-qiskit-46eb73f78394)

[QISKIT AER](https://github.com/Qiskit/qiskit-aer)

[simulate-with-qiskit-aer](https://docs.quantum.ibm.com/guides/simulate-with-qiskit-aer)

[QISKIT SDK Primatives](https://docs.quantum.ibm.com/guides/simulate-with-qiskit-sdk-primitives)

[QISKIT Simulators](https://qiskit.github.io/qiskit-aer/tutorials/1_aersimulator.html)
