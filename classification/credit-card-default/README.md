# Credit Card Default

Model default-payment outcomes using the UCI Default of Credit Card Clients dataset, with categorical and numerical preprocessing, classifier comparison and threshold analysis.

[Open the notebook](credit_card_default.ipynb).

## Files and setup

The original input files are supplied as ZIP archives beside the notebook. Extract each archive into this same folder before running the notebook; extraction restores the original filename expected by the code. Install the shared dependencies from the repository root, then open this notebook with its own folder as the working directory. The notebook and saved outputs are copied unchanged from the local practice project; no new execution was performed.

## Evaluation context

The notebook examines decision thresholds using test-set outcomes. Treat its final threshold-based scores as exploratory, rather than an untouched final holdout evaluation. A separate validation set or nested procedure would be needed for threshold selection before final testing.

This is a learning exercise. Source datasets and task concepts remain attributable to their respective creators. See the repository-level data-source and interpretation notes.
