# EEG Alpha Power Desynchronization Analysis

## Overview
This repository contains a Python-based analysis pipeline demonstrating how to process and statistically evaluate paired experimental data. The project simulates a common computational neuroscience paradigm: measuring the suppression (desynchronization) of EEG Alpha band power (8-12 Hz) when a subject transitions from a resting state to an active cognitive task.

## Technical Approach
Standard parametric tests (like a paired t-test) often fail when physiological data violates normality assumptions. To account for this, this script utilizes **Permutation Testing** (a robust non-parametric resampling technique) to calculate statistical significance, alongside **Cohen's d** for effect size. 

## Tech Stack
*   **Data Manipulation:** `pandas`, `numpy`
*   **Statistical Modeling:** Custom Permutation Testing algorithm (10,000 iterations).
*   **Data Visualization:** `matplotlib`, `seaborn`

## Output & Visualization
The script generates a publication-ready paired slopegraph featuring:
*   Individual subject trajectories (gray lines) to highlight the paired experimental design.
*   Mean overlay with error bars (black diamonds).
*   Embedded statistical annotations (Mean Difference, Permutation *p*-value, and Effect Size).


