# Qualitative Dynamics in Coupled Nonlinear Systems

Research notebooks from my ongoing work as a volunteer research assistant at Kyiv National University, supervised by **Prof. Ihor Samoilenko** and **Assoc. Prof. Roman Yakymiv**.

This project investigates how the qualitative behaviour of coupled nonlinear discrete-time systems changes with their parameters. It combines numerical simulation, parameter-space exploration, machine-learning classification and mathematical analysis.

**Status:** Ongoing research. The notebooks document an evolving investigation, including exploratory experiments and earlier approaches.

## Research questions

- Which parameter configurations produce valid dynamics?
- How can stable and oscillatory regimes be identified efficiently within a large parameter space?
- How do changes in coupling and other parameters affect the system’s qualitative behaviour?
- Under what assumptions can numerically observed regime transitions be given a rigorous mathematical interpretation?

## Model and methods

The initial model describes two interacting locations through coupled Lotka–Volterra dynamics, normalisation and a conflict mechanism. The investigation explores how local dynamics and interactions between locations jointly determine the behaviour of the full system.

The computational work involves:

1. **Simulation:** implementing the discrete-time model and reproducing results from earlier work by the supervisors.
2. **Parameter exploration:** sampling parameter configurations and examining the resulting trajectories.
3. **Validity classification:** identifying regions that satisfy the model’s admissibility criteria and separating them from invalid or divergent dynamics.
4. **Regime classification:** distinguishing stable and oscillatory behaviour within valid regions.
5. **Transition analysis:** investigating changes under parameter variation and examining the mathematical justification of a numerical transition criterion.

The classification approach has evolved from an initial Gaussian-process classifier towards separate validity and regime classifiers, reflecting the difficulty of analysing a parameter space containing substantial regions of invalid dynamics.

## Mathematical analysis

The theoretical work investigates the assumptions needed to relate a numerical regime-transition criterion to stability and bifurcations.

A change in a numerical regime label does not, by itself, establish a bifurcation. Finite simulation horizons, numerical tolerances and classification errors must be considered when interpreting computational results.

## Current direction

The research is being extended towards information diffusion on social-media platforms and is integrated with my University of London final-year project, **Predictive Modelling of Social Media Trend Emergence**.

The current direction replaces the Lotka–Volterra component with a discretised information-warfare model while retaining a coupled-system framework. Planned work includes:

- Parameter identification using public Telegram data.
- Predictive validation and analysis of dynamical regimes.
- Investigation of model predictive control for specified objectives.

These are ongoing or planned extensions rather than completed results.

## Using the notebooks

The notebooks record different stages of the research and should be read as individual experiments. Earlier notebooks may use different models, classifiers or assumptions from later work.

Before running a notebook, review its imports, parameter settings and any data or file-path requirements. When comparing results, check the simulation horizon, numerical tolerances and definitions used to label trajectories.

This repository serves as a research record rather than a packaged software library.

## Author

**Timothy Gregory**  
BSc Computer Science, University of London  
Research Assistant (volunteer), Kyiv National University

[Academic website](https://timgrego.github.io) · [GitHub](https://github.com/timgrego) · [Email](mailto:tim.gregory2306@gmail.com)
