## Project-4-Differential-Privacy

This README provides instructions on how to run the Secure Multi-Party Computation (SMPC) experiment code. The experiment measures the runtimes and accuracy error for four different SMPC approaches: **No Privacy Protection**, **Shamir's Secret Sharing**, **Paillier Encryption**, and **Differential Privacy**, across various values of `n`.

### Prerequisites

Before running the code, make sure you have the following prerequisites installed:

Python 3.x

Jupyter Notebook installed

Required Python libraries (You can install them using `pip install <library_name>`):

`plotly`

`sympy`

`phe`

### Getting Started

1. Clone this repository:

```bash
git clone https://github.com/harisiqbal10/Project-4-Differential-Privacy.git
cd Project-4-Differential-Privacy
```
2. Launch the Jupyter Notebook
   
3. Open the code file, `Project_4_Differential_Privacy.ipynb`, and update the following variables to customize your experiment:

`values_of_n`: List of `n` values for which you want to measure runtimes.

`num_experiments`: Number of experiments to run for each `n`.

`values_per_party`: The number of values generated for each party in each experiment.

Modify `secret` in the `shamir_secret_sharing` function if you want to use a different secret.

Set a privacy budget of `ε = 1.0` for testing `differential_privacy` function.

### Running the Experiment

Within the Jupyter Notebook, run each cell in the notebook sequentially. The notebook will execute the experiment for each SMPC approach and collect average runtimes and accuracy errors for each `n`. If interruption occurs, please select `Restart & Run All`.

### Viewing Results

The Jupyter Notebook will display two plots:

1. **Combined Runtimes for Different SMPC Approaches**
2. **Combined Accuracy Errors for Different SMPC Approaches**
