# VQE-spin-liquid
Quantum Spin Liquids are a unique state of matter that occurs when the electron configuration within the material cause the spin of each electron to enter into a quantum state. This creates a ferromagnetic lattice that has some applications in information processesing and potentially room temperature superconductivity. Because QSLs are a new concept, there are some things that aren't fully understood. One of these includes the lowest ground state energy configuration of these lattices to understand the properties of the materials. This repository uses a custom VQE algorithm and ansatz to calculate the lowest ground state energy configuration of a given lattice.

## Required Software
To run the software, you will need the following:
* IBM Qiskit library
* matplotlib
* numpy
* pylatexenc
* ipywidgets
* ipykernel
* (Optional to run your own simulations) IBM API token

### Library installation
To install the all of the necessary libraries, we recommend doing the following:
* Ensure that you're running a version of Python that is 3.7 or above
* Open a terminal for a version of Linux installed on your machine
* Once it loads, we recommend creating a new Anaconda environment. This can be done by doing the following
```
conda create --name <Environment Name> python=3.9
```
Where you may name your environment whatever you would like
* Be patient and make sure that you type y to create your environment after a dialog box appears
* After the environment has been created, run the following command
```
conda activate <Environment Name>
```
To activate your Anaconda environment
* You're now ready to install the libraries to use this repository. Ensure that your file directory is at the root of this repository. By typing `ls` in the repository directory, you should see a file called `requirements.txt`. Finally, you can run the following

```
pip install -r requirements.txt
```
* Be patient and wait for the libraries to finish installing

### IBM API token
If you would like to get access to the quantum computers used in this project to run your own simulations, please do the following:
* Go to [quantum-computing.ibm.com](https://quantum-computing.ibm.com)
* Create an IBMid account if you do not have one already and follow the steps to set up your account. If you do, log in to your account.
* Once you have your account, go to the homepage
* On the homepage, you will see a section that says `API token` with a copy icon next to the asterisks. Click on the icon.
* What you have is your own unique API token to retrieve your own job requests to the IBM quantum backend. DO NOT SHARE THIS TOKEN WITH ANYONE!!!
* If there is a section in the files that are listed with a comment mentioning an API token, you may paste your API token to get your own job requests

(*NOTE*) If you run your own simulations, it may take some time until you can get your results back due to the other people requesting to run other quantum simulations. It is in your best interest to go back to the homepage on [quantum-computing.ibm.com](https://quantum-computing.ibm.com) and click on `View all` in the section of the page that says "Run on circuits & programs via IBM Quantum compute resources". Any computer that says "open" under the `Plan` category is a computer that you can run your simulations on. A computer that says "premium" will require you to make a payment to use, though there will be less traffic for these computers. You should make the proper judgement as to which computer you should use to obtain your simulation results. You should go to the `job_request.py` file and put in your own API key to run your own simulations and run every cell in the Jupyter notebook. This way, you will get a set of text files that denote the circuit tested and the number of times a specific configuration appeared.

If you have any questions, please feel free to reach out to Kevin Lie-Atjam (klieatjam@olin.edu)
