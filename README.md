# Applied Machine Learning Practice

Six Python projects exploring supervised learning on structured datasets. The collection covers preprocessing, baseline models, regularisation, ensembles, evaluation metrics and interpretation.

These are independent learning projects rather than deployed decision systems. They complement the shorter platform exercises in [python-coding-challenges](https://github.com/iamalif/python-coding-challenges).

## Start here

- [Bank marketing](classification/bank-marketing/): mixed-type preprocessing, removal of an unavailable-at-prediction feature, model comparison and threshold trade-offs.
- [Superconductor regression](regression/superconductor/): linear, regularised and ensemble regression comparisons with diagnostic plots.

## Full collection

| Project | Task | Dataset |
|---|---|---|
| [Credit risk](classification/credit-risk/) | Serious delinquency classification | Give Me Some Credit |
| [Pulsar detection](classification/pulsar-detection/) | Pulsar-candidate classification | HTRU2 |
| [Bank marketing](classification/bank-marketing/) | Term-deposit subscription classification | UCI Bank Marketing |
| [Credit card default](classification/credit-card-default/) | Default-payment classification | UCI Default of Credit Card Clients |
| [Superconductor](regression/superconductor/) | Critical-temperature regression | UCI superconductivity dataset |
| [Communities and crime](regression/communities-and-crime/) | Aggregate crime-rate regression | UCI Communities and Crime |

## What the projects demonstrate

- Missing-value handling and mixed categorical/numerical preprocessing
- Baseline comparisons, feature scaling and pipelines
- Logistic regression, linear models and regularisation
- Random Forests and boosting methods
- Classification metrics, confusion matrices and threshold trade-offs
- Regression errors, residual diagnostics and feature importance

## Evaluation context

The original notebooks and their saved outputs are preserved unchanged. They document exploratory learning, not a new independent validation exercise.

The classification notebooks inspect candidate thresholds using test-set outcomes. A threshold selected this way makes the resulting test score part of model selection rather than an untouched final estimate. The appropriate next methodological step would be selecting thresholds on separate validation data and reserving a final test set.

The Communities and Crime notebook also retains a copied Random Forest diagnostic in its boosting section, as identified in the earlier source review. Its folder README makes this limitation explicit. No code was changed or rerun for this publication.

Credit and marketing examples do not establish suitability for real lending or customer decisions. Historical community-level associations should not be interpreted as causal explanations or predictions about individuals. Metrics and feature importance must be read within each dataset's scope.

## Using the notebooks

Use Python 3 and install the shared packages in an isolated environment:

```bash
python -m pip install -r requirements.txt
python -m jupyterlab
```

First extract each dataset ZIP into its own project folder, so the original CSV, XLS or DATA file sits beside the notebook. Then open the notebook from that folder. Each notebook is independent. The dependency list reflects the existing imports, not a freshly verified version lock. The Excel-based credit-card dataset requires `xlrd`.

You can read saved outputs without running the notebooks. Existing outputs are historical experiment records, not a promise that every cell will execute unchanged under the latest library versions.

## Data and attribution

Input files are copied from the existing local practice folders and compressed individually for browser upload. Extract each dataset ZIP into its project folder before running the notebook. Dataset names are listed above; original data documentation is retained where available, including `communities.names`. The datasets and any source exercise concepts belong to their respective creators. This repository presents the analysis work and does not claim authorship of the data.

Original task-brief PDFs and duplicate local README drafts are excluded. Each project has a concise navigation and interpretation guide.

## Related work

- [Statistical Learning MSc](https://github.com/iamalif/statistical-learning-msc)
- [Swedish Job-Ad Explorer](https://github.com/iamalif/swedish-job-ad-explorer)
