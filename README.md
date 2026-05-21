# Quantum Computing

Beginner-friendly Qiskit experiments and notebooks for learning core quantum-computing concepts such as single-qubit gates, multi-qubit gates, state vectors, Bloch-sphere visualization, and circuit measurement.

## Contents

- [Project Overview](#project-overview)
- [Repository Structure](#repository-structure)
- [Requirements](#requirements)
- [Setup](#setup)
- [How to Use](#how-to-use)
- [Tutorial Notes](#tutorial-notes)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Project Overview

This repository is a compact learning workspace focused on:

- building circuits with `qiskit.QuantumCircuit`
- simulating circuits with `qiskit-aer`
- visualizing states and circuits
- practicing with small hands-on exercises

It currently includes an introductory tutorial notebook and a short exercise notebook under `tutorial-1/`.

## Repository Structure

```text
.
├── main.py
├── pyproject.toml
├── uv.lock
└── tutorial-1
    ├── t1nb1.ipynb
    └── exercise.ipynb
```

- `main.py`: lightweight Python entrypoint.
- `tutorial-1/t1nb1.ipynb`: Tutorial 1 notebook (gate basics, Bloch sphere, measurement).
- `tutorial-1/exercise.ipynb`: practice notebook with a multi-qubit circuit exercise.

## Requirements

- Python 3.11+ (see `.python-version`)
- Jupyter environment (for notebooks)

## Setup

### Option 1: pip

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e .
```

### Option 2: uv

If you use [uv](https://docs.astral.sh/uv/):

```bash
uv sync
```

## How to Use

### Run the Python entrypoint

```bash
python main.py
```

### Open the notebooks

```bash
jupyter notebook
```

Then open:

- `tutorial-1/t1nb1.ipynb`
- `tutorial-1/exercise.ipynb`

## Tutorial Notes

### `tutorial-1/t1nb1.ipynb`

Covers introductory concepts including:

- basic gates (`X`, `Y`, `Z`, `H`, `CX`)
- circuit drawing
- statevector simulation
- Bloch-sphere visualization
- measurement and shot-based simulation with `AerSimulator`

### `tutorial-1/exercise.ipynb`

Provides a larger multi-qubit practice circuit to reinforce:

- gate composition on multiple qubits
- circuit organization with barriers
- simulation and measurement workflows

## Dependencies

Main project dependencies are managed in `pyproject.toml`:

- `qiskit[visualization]`
- `qiskit-aer`
- `matplotlib`
- `pylatexenc`
- `ipykernel`

## Contributing

Contributions are welcome. Useful improvements include:

- additional tutorials (entanglement, Bell states, teleportation, algorithms)
- clearer notebook explanations and comments
- more exercises and challenge problems
