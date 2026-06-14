# Radiocarbon-Dating-Bayesian-Analysis
# Radiocarbon Dating Analysis using Bayesian Inference

## Overview

This project was developed as part of the Probability Theory (PRA) course at VSB – Technical University of Ostrava.

The goal of the project is to estimate the age of an archaeological biological sample using radiocarbon dating and Bayesian statistical methods.

The analysis combines radioactive decay theory, Poisson probability models, and Bayesian inference to determine the posterior probability distribution of the sample's age.

## Problem Description

An archaeological sample containing carbon is analyzed using a radiocarbon detector.

The detector records beta particles emitted by the decay of Carbon-14 isotopes during a fixed observation period. Based on the measured number of particles and known physical constants, the age of the sample is estimated.

The unknown age is assumed to lie within the interval:

```text
1000 ≤ t ≤ 5000 years
```

## Methods Used

### Radioactive Decay Model

The decay of Carbon-14 is modeled using the exponential decay law:

```text
N(t) = N₀ e^(-λt)
```

where:

* N₀ is the initial number of Carbon-14 atoms
* λ is the decay constant
* t is the age of the sample

### Poisson Distribution

The number of detected particles is modeled as a Poisson random variable:

```text
N | t ~ Poisson(μ(t))
```

where μ(t) represents the expected number of detected particles.

### Bayesian Inference

A discrete uniform prior distribution is assumed for the unknown age:

```text
t ∈ {1000, ..., 5000}
```

Bayes' theorem is then used to compute the posterior probability distribution:

```text
p(t | N)
```

based on the observed measurement data.

## Results

The analysis produced:

* Posterior probability distribution of sample age
* Maximum posterior estimate (MAP)
* Median age estimate
* Shortest 95% credible interval

### Final Estimates

```text
Estimated age (posterior mode): approximately 1774 years

Posterior median:
1774 years

95% credible interval:
[1711, 1837] years
```

## Technologies Used

* Probability Theory
* Bayesian Statistics
* Poisson Processes
* Radiocarbon Dating
* Mathematical Modelling
* Python (verification and numerical calculations)

## Learning Outcomes

Through this project, I gained practical experience in:

* Bayesian inference
* Probability distributions
* Poisson processes
* Radioactive decay modelling
* Statistical estimation
* Scientific computing
* Mathematical modelling of real-world phenomena

## Author

**Aruzhan Abilmazhinova**

Bachelor's Degree in Computational and Applied Mathematics

Faculty of Electrical Engineering and Computer Science (FEI)

VSB – Technical University of Ostrava
