# Gravitational De-lensing for Reconstructing Distorted Galaxy Images with Horseshoe Prior and Starlet Basis
Reconstructing Background Galaxies via Sparse Horseshoe Prior and Starlet Basis[minimization_jax_mcmc-2.py](..%2F..%2FDownloads%2Fcopy_of_main_minimization_jax_mcmc-2.py)


By harnessing regularization and minimization techniques, our methods aim to restore the true appearance of galaxies affected by gravitational lensing. Here's an overview of the core objectives and techniques:

## Objective: Reconstructing Distorted Galaxy Images
At the heart of this repository lies the goal of restoring the original appearance of galaxies that have been distorted by gravitational lensing effects. We leverage advanced computational methods and regularization techniques to unravel the universe's hidden treasures.

## Methods for De-lensing
We present several methods tailored to this objective:

### Method: HS + Starlet
The `model_HS_likelihood` function combines tax-based regularization with the starlet transformation. This synergistic approach enhances de-lensing accuracy by addressing both regularization and transformation aspects.

### Method: HS (Horseshoe)
For a pure Horseshoe (HS) regularization method, the `model_HS_withoutStarlet_likelihood` function focuses on tax-based regularization. This approach offers a baseline for comparison with the hybrid method.

### Method: L1 + Starlet
The `model_L1_likelihood` function incorporates L1 regularization alongside the starlet transformation, presenting an alternative regularization strategy with transformation benefits.

### Method: L2 + Starlet
Similar to the L1 method, the `model_L2_likelihood` function introduces L2 regularization paired with the starlet transformation. This approach provides a distinct regularization perspective.

## MCMC Inference for Accurate Results
All methods utilize Markov Chain Monte Carlo (MCMC) inference to estimate model parameters and capture the underlying structures of galaxy images. The `run_inference` function orchestrates this process, yielding valuable samples for each method.

## Model Configuration and Experimentation
Explore the nuances of de-lensing by adjusting the `model` parameter. Tailor the `warmup` and `samples` parameters to control warmup steps and sampling iterations, adapting the method to specific datasets and objectives.

## Execution and Insightful Summaries
By configuring the chosen method through the `args` object, the appropriate functions are selected. The `main` function coordinates the MCMC inference and generates comprehensive summaries, enabling a deeper understanding of the de-lensed images.

