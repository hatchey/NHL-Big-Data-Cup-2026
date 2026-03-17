[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XCVWfNSpHMwazqTQk3ptQQl-F6aUBcKp)
# NHL Power Play Analysis using DTMC

This repository contains the code for analyzing NHL power play tactics using discrete-time Markov chain (DTMC) models. The project was developed as part of the Big Data Cup 2026.

## Overview

This project models offensive zone puck movement during NHL power plays as a discrete-time Markov chain. By representing rink locations as states and puck movements as transitions, the model captures team-specific tactical tendencies and evaluates their effectiveness.

## Objectives

- Model power play sequences using DTMCs  
- Quantify team tendencies in puck movement and zone usage  
- Evaluate scoring opportunity generation  
- Identify stylistic differences across teams  

## Methodology

- The offensive zone is discretized into a grid of states  
- Transition matrices are constructed from event and tracking data  
- Absorbing states represent terminal outcomes (e.g., shot, giveaway)  
- The fundamental matrix is used to derive:
  - Absorption probabilities (shot vs giveaway)
  - Expected sequence length
  - Zone visitation probabilities  

## Features

Key features derived from the model include:

- Shot probability  
- Giveaway probability  
- Expected sequence length  
- High-danger zone (HDZ) probability  
- Cross-seam pass probability  

## Repository Structure
.
├── notebooks/
│ └── Big_Data_Cup_2026.ipynb
└── README.md
## Usage

1. Open the notebook in Google Colab or Jupyter  
2. Run all cells to reproduce the analysis  
3. Ensure required dependencies are installed  

## Requirements

- Python 3.x  
- numpy  
- pandas  
- matplotlib  
- scikit-learn  
- networkx  
- sportypy  

Additional standard libraries:
- math  
- os  
- re  
- warnings  

## Results

The analysis identifies distinct team power play structures, including:
- Flank-oriented systems  
- Point-dominant puck movement  
- Variations in sequence length and puck circulation  

These differences are linked to variations in shot generation and scoring opportunity quality.

## Paper

The full methodology and results are detailed in the accompanying Big Data Cup 2026 submission paper.

## Author

Max Desmoulin

## Notes

- Data used in this project is subject to competition and provider restrictions  
- This repository contains code only; data may not be publicly available
  
## Reproducibility

The full analysis can be run directly in Google Colab using the link above.  
Ensure all required libraries are installed before execution.
