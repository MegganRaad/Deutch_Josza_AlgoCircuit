# Quantum Deutsch-Josza Algorithm implementation

This Python program demonstrates the implementation of the Deutsch-Josza algorithm using Cirq, a quantum computing library. The Deutsch-Josza algorithm is a quantum algorithm that efficiently solves a specific problem: determining whether a given function is constant or balanced. A function is considered constant if it returns the same output for all inputs, and balanced if it returns 0 for half of the inputs and 1 for the other half.

## Features
- Quantum Circuit for Deutsch-Josza Algorithm: Implements a quantum circuit that applies the Deutsch-Josza algorithm to determine if a given function is constant or balanced.
- Balanced and Constant Oracles: Includes examples of both balanced and constant oracles to test the algorithm.
- Simulation: Utilizes Cirq's simulator to run the quantum circuit and observe the algorithm's outcome.

## Requirements
- Python 3.7 or Later
- Google's Cirq

## Installation
Ensure you have Python 3.7 or later on your system. Then, proceed to install Cirq using pip:
```sh
pip install cirq
```
_Alternatively, you can use Google's Cirq cloud platform "Collaboratory" by clicking the link below and signing in to your google account_

[Google Colaboratory](https://colab.google/) 

You'll then want to create a new New notebook and implement the following:
```
!pip install --quiet cirq
```
## Usage
1. First Clone the Repository to your local machine using `git` or download the zip file
2. Navigate to the directory containing the program and run it using the following Python command:
   ```sh
   python deutsch_josza.py
   ```
_Alternatively, if you are using Colab:_
`File > Save a copy in Github > Link Github Account > Link to public repo of choice`

## How it works
The program first creates a quantum circuit with a specific number of qubits and an auxiliary qubit. It then applies the Deutsch-Josza algorithm, which inlcudes the following steps:
1. All Qubits are initialized in the `|0>` state, and Hadamard gates are applied to put them into superposition
2. The quantum circuit applies an oracle that encodes the function being tested
3. Additional Hadamard gates are applied, followed by measurement of the input qubits

## Contributions
Contributions to improve the implementation or extend its functionality are welcomed! Please feel free to fork the repository and submit pull requests.

## License
This project is an open source contribution and is available under the [MIT LICENSE](https://opensource.org/license/mit) 


