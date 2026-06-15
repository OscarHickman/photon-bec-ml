# Photon BEC Phase Diagram Characterisation using Machine Learning

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

This repository contains the analysis and machine learning experiments developed for my Bachelor's project: **Characterisation of a Photon Bose-Einstein Condensate Phase Diagram using Machine Learning**. 

The full written thesis can be found in this repository: **[BSc_Thesis.pdf](./BSc_Thesis.pdf)**.

## Overview

The project focuses on building and training machine learning models to characterise the phase diagram of a Photon Bose-Einstein Condensate. It explores binary and length-based physical parameters using TensorFlow and SciPy.

## Repository Structure

- `src/photon_bec/` — Core package modules (`photon_bec.binary` and `photon_bec.length`).
- `examples/` — Example scripts to demonstrate the module usage and training pipelines.
- `scripts/` — Utility scripts for data processing and analysis.
- `tests/` — Test suite for verifying the core logic.
- `BSc_Thesis.pdf` — The final compiled thesis document detailing the theoretical background and methodology.
- `pyproject.toml` / `requirements.txt` / `Makefile` — Project configuration and dependency management.

## Quickstart

1. **Clone the repository:**
   ```bash
   git clone https://github.com/OscarHickman/Characterisation-of-Photon-BEC-phase-diagram-using-Machine-Learning.git
   cd Characterisation-of-Photon-BEC-phase-diagram-using-Machine-Learning
   ```

2. **Set up the environment:**
   Using the provided `Makefile` is the easiest way to create a virtual environment and install dependencies:
   ```bash
   make setup
   ```
   Alternatively, you can manually create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```

3. **(Optional) Run Code Formatters:**
   If you wish to contribute or ensure code consistency:
   ```bash
   make precommit
   ```

## Usage

The package exposes the `photon_bec.binary` and `photon_bec.length` modules.

You can run the provided examples from the repository root to see the models in action:

```bash
# Ensure you are using the virtual environment
source .venv/bin/activate

# Run the binary example
PYTHONPATH=src python -m examples.run_binary_example

# Run the length example
PYTHONPATH=src python -m examples.run_length_example
```

> **Note**: To build and train new models from scratch, ensure you have TensorFlow and SciPy correctly installed and configured in your environment.
