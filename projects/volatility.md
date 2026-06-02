# Volatility-Dependent Learning Rates: Model Comparison and Parameter Recovery

> **Level:** MSc  
> **Duration:** 6 months  
> **Keywords:** `cognitive modelling`, `reinforcement learning`, `volatility`, `parameter recovery`, `Kalman filter`, `learning rates`

---

## Description

Classical reinforcement learning models assume that learning rates are constant across trials. More recent models propose that learning rates should vary dynamically, tracking how volatile the environment is — that is, how often reward contingencies change. Two prominent examples are the Volatile Kalman Filter (VKF) and the Hierarchical Gaussian Filter (HGF).

Despite their theoretical appeal, preliminary testing suggests that these models suffer from poor parameter recovery — meaning that the parameters estimated from data do not reliably reflect the true underlying values. This is a fundamental problem: if parameters cannot be recovered, conclusions drawn from fitting these models to empirical data are unreliable. Interestingly, this issue persists even when using the original code supplied by the authors of these models, suggesting it may be a deeper structural problem rather than an implementation error.

## Goal

To rigorously evaluate the parameter recovery of the VKF, HGF, and related volatility-based learning models, and to identify or develop a model that implements dynamic, volatility-dependent learning rates with good estimation properties — embedded within the EMC2 framework.

## Tasks

1. Implement and rigorously test parameter recovery of the VKF and HGF (and related models) within EMC2.
2. Systematically diagnose where and why recovery fails.
3. Survey the literature for alternative models that capture volatility-dependent learning.
4. Test whether any of these alternatives show better estimation properties, and if not, explore what modifications might help.

## Required Knowledge

- R (or a strong willingness to learn)
- Basic statistics and probability
- Familiarity with reinforcement learning or cognitive modelling

## Background & Recommended Reading

- Piray & Daw (2020) — [A simple model for learning in volatile environments](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1007963) *(VKF)*
- Mathys et al. (2011) — [A Bayesian Foundation for Individual Learning Under Uncertainty](https://www.frontiersin.org/journals/human-neuroscience/articles/10.3389/fnhum.2011.00039/full) *(HGF)*
- EMC2 R package — [GitHub repository](https://github.com/ampl-psych/EMC2)
- Recovery methodology example: Miletić et al. (2017) — [Parameter recovery for the Leaky Competing Accumulator model](https://www.sciencedirect.com/science/article/abs/pii/S0022249616301663)

## Expected Output

- Parameter recovery analyses for VKF, HGF, and related models
- Written MSc thesis / report
- Codebase (R scripts / reproducible analysis pipeline)
