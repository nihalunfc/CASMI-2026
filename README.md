# CASMI 2026 - Molecule ID From Mass Spectra

This repository contains the codebase and progression for my submissions to the Enveda CASMI 2026 challenge. The objective of this project is to identify molecular structures (SMILES) from raw, complex mass spectrometry data.

## Project Structure

The project is structured chronologically, representing the evolution of the data pipelines and predictive models.

### 1. Baseline Submission (01_baseline_submission/)
- **Objective:** Establish an automated end-to-end data processing pipeline.
- **Description:** This pipeline successfully reads the hidden testing data, handles formatting, and generates predictions based on the statistical frequency of molecules within the training set. It serves as the structural foundation for more complex models.

### 2. Analog Ranker (02_analog_ranker/)
- **Objective:** Implement a robust predictive model using distance and similarity metrics.
- **Description:** A more sophisticated approach that ranks candidate molecules using an analog ranking strategy. The pipeline was rigorously refactored to run efficiently on CPU clusters to manage cloud computing resource constraints.

### 3. Transformer Ensemble (03_transformer_ensemble/)
- **Objective:** Deploy advanced deep learning for maximum predictive accuracy.
- **Description:** An ensemble approach utilizing a 4-channel transformer architecture to extract deep structural signals from mass spectra, representing the state-of-the-art for this challenge.

## Setup and Usage

The notebooks are designed to be executed in a standard data science environment (e.g., Jupyter, Kaggle Kernels) with the following typical dependencies:
- Python 3.10+
- Pandas
- Numpy
- PyTorch (for the Transformer models)
- RDKit (for molecular informatics)
