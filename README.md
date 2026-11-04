# Samson Obasanmi
 
Machine learning engineer working on **natural language inference** and
**scientific machine learning**. I build open-source research software and
apply it to shared-task benchmarks, with an emphasis on reproducible,
honestly reported results.
 
[ORCID 0009-0009-6935-5479](https://orcid.org/0009-0009-6935-5479) ·
[pinnr documentation](https://obasanmii.github.io/pinnr/)
 
---
 
## Open-source software
 
### [pinnr](https://github.com/Obasanmii/pinnr): physics-informed neural networks in native R
 
[![R-CMD-check](https://github.com/Obasanmii/pinnr/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/Obasanmii/pinnr/actions/workflows/R-CMD-check.yaml)
[![R-universe](https://obasanmii.r-universe.dev/badges/pinnr)](https://obasanmii.r-universe.dev/pinnr)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23835717.svg)](https://doi.org/10.5281/zenodo.23835717)
 
Physics-informed neural networks have so far needed Python libraries such as
DeepXDE, or R packages built for a single application. pinnr is a general,
R-native PINN library built on [`torch`](https://torch.mlverse.org), with no
Python dependency.
 
- Solves ordinary and partial differential equations and estimates unknown
  model parameters from observations
- Accepts existing `deSolve` models unchanged
- Supports Dirichlet, Neumann, initial and custom conditions, and hard
  constraints
- Trains with Adam and L-BFGS, uses Latin hypercube resampling and time
  marching, and runs on GPU
- Is tested on Linux, macOS and Windows in CI, is archived on Zenodo, and
  installs from R-universe
```r
install.packages("pinnr", repos = c("https://obasanmii.r-universe.dev",
                                    "https://cloud.r-project.org"))
```
 
Feedback, issues and pull requests are welcome. See
[CONTRIBUTING](https://github.com/Obasanmii/pinnr/blob/main/CONTRIBUTING.md).
 
---
 
## Research
 
### SemEval-2027 Task 2: DiCo-NLI, directional consistency in NLI
 
I am building a system for all four tracks: English, Spanish, Basque and
mixed-language pairs. It combines transformer ensembles (DeBERTa-v3, mDeBERTa,
XLM-R) with a **consistent decoding** step that predicts both directions of a
sentence pair jointly, so that the two labels cannot contradict each other.
The analysis separates how much of the gain comes from joint decoding itself
and how much comes from properties of the data. The system paper and code
will be released with the task in 2027.
 
---
 
## Applied ML projects
 
| Project | Overview/Description |
|---|---|
| [churn_classifier](https://github.com/Obasanmii/churn_classifier) | Leakage-safe churn model at a 5% base rate, with cost-based threshold choice and tested pipeline invariants |
| [ml-service](https://github.com/Obasanmii/ml-service) | FastAPI model serving with input validation, KS drift monitoring, Prometheus metrics, Docker and CI |
| [streaming-ml](https://github.com/Obasanmii/streaming-ml) | Real-time inference on a Kafka event stream, with a CI end-to-end check |
| [ga4-activation-and-retention](https://github.com/Obasanmii/ga4-activation-and-retention) | Activation funnel and retention cohorts modelled from 4.3M raw GA4 events in BigQuery and Dataform, with data-quality assertions |
 
---
 
## Tools
 
**Languages:** Python, R, SQL<br>
**Machine learning:** PyTorch, Hugging Face Transformers, torch for R, scikit-learn, LightGBM, SHAP<br>
**Engineering:** FastAPI, Docker, Kafka, GitHub Actions, Prometheus, pkgdown, testthat, pytest<br>
**Data:** BigQuery, Dataform, Tableau
 
## Currently
 
- Developing pinnr: regular releases, benchmarks against classical solvers,
  and more PDE examples
- Participating in SemEval-2027 Task 2 (DiCo-NLI) across all four language tracks, and writing the system paper
