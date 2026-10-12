# MUJ-DS-2430010363

## Student Details

| Field | Details |
|---|---|
| **Name** | Gopal Deswal |
| **Registration Number** | 2430010363 |
| **Branch** | B.Tech CSE (Data Science) |
| **Section** | D |
| **GitHub Username** | Gopal-Deswal |
| **Project Title** | Deep Learning-Based Network Intrusion Detection System using CNN-LSTM Hybrid Architecture on the CICIDS2017 Dataset |

## Project Overview

This project builds a network intrusion detection system (NIDS) using a hybrid CNN-LSTM architecture trained on the CICIDS2017 dataset. It covers:

- Standard binary classification of benign vs. attack traffic
- Overfitting/underfitting, bias and variance analysis
- Evaluation with standard test metrics (confusion matrix, ROC curve, comparison against published results)
- Leave-One-Attack-Out (LOAO) experiments to study detection of unseen attack types, including an ablation study

## Repository Structure

    MUJ-DS-2430010363/
    |-- README.md
    |-- assignments/        Training assignments
    |-- notebooks/          Jupyter notebook for the NIDS CNN-LSTM project
    |-- code/               Source scripts
    |-- resources/          Research paper (LaTeX source and PDF), references
    |-- presentations/      Project slides
    |-- capstone/           Capstone work, screenshots and results

## Installation

1. Clone the repository:

        git clone https://github.com/Gopal-Deswal/MUJ-DS-2430010363.git
        cd MUJ-DS-2430010363

2. (Recommended) create a virtual environment:

        python -m venv venv
        venv\Scripts\activate

3. Install dependencies:

        pip install -r requirements.txt

4. Download the CICIDS2017 dataset (see below) and open the notebook:

        jupyter notebook notebooks/NIDS_CNN_LSTM_submission.ipynb

## Dataset

CICIDS2017 from the Canadian Institute for Cybersecurity (https://www.unb.ca/cic/datasets/ids-2017.html).
The dataset is large and is not stored in this repository. Download it and place the files where the
notebook expects them (see the data-loading cell in the notebook).

## Usage

Run the notebook cells in order. The notebook preprocesses the data, trains the CNN-LSTM model,
evaluates it, and runs the LOAO experiments.

## Results

Results are saved in `capstone/results/` and described in the research paper in `resources/`.

- Standard evaluation: bias-variance analysis, confusion matrix, ROC curve, comparison with published work
- LOAO evaluation: unseen-attack detection results and ablation study

## Research Paper

The LaTeX source is in `resources/paper/main.tex`, and the compiled PDF is in `resources/`.

## Author

Gopal Deswal, Manipal University Jaipur
