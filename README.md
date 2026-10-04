# scikit-learn Cookbook

Code reproduction and theoretical explanations from John Sukup's *scikit-learn Cookbook*, Third Edition (Packt Publishing, 2025; available through O'Reilly). This individual course repository develops one Jupyter notebook for each chapter and explains the code output in Indonesian.

**Student:** Muhammad Habibie Rabbani · TK-47-04 · Computer Engineering, Telkom University

## Current progress

| Chapter | General topic | Notebook | Status |
|---|---|---|---|
| 1 | Common conventions and API elements: estimators, transformers, pipelines, attributes, tuning, and metadata | [Chapter 1](01_Common_Conventions_and_API_Elements.ipynb) | Complete |
| 2 | Pre-model workflow: missing data, scaling, encoding, pipelines, and feature engineering | [Chapter 2](02_Pre_Model_Workflow_and_Data_Preprocessing.ipynb) | Complete |
| 3 | Dimensionality reduction: PCA, LDA, t-SNE, and method selection | — | Planned |
| 4 | Distance metrics and nearest neighbors: KNN training, tuning, and evaluation | — | Planned |
| 5 | Linear models and regularization: regression, Ridge, Lasso, and ElasticNet | — | Planned |
| 6 | Logistic regression: multiclass, regularization, and evaluation | — | Planned |
| 7 | Support vector machines and kernel methods | — | Planned |
| 8 | Decision trees, random forests, and ensemble methods | — | Planned |
| 9 | Text processing and multiclass classification | — | Planned |
| 10 | Clustering techniques and their evaluation | — | Planned |
| 11 | Novelty and outlier detection | — | Planned |
| 12 | Cross-validation and model evaluation | — | Planned |
| 13 | Model deployment and maintenance | — | Planned |

The course milestone for Chapters 1–5 is **10 October 2026 at 23:59**. Planned chapters are listed to show the book's scope; only notebooks linked above are complete.

## What each notebook contains

- Reproduced or clearly identified adaptations of the chapter's recipes.
- An explanation of the methods, their assumptions, output, and limitations.
- A chapter summary and references to the book and scikit-learn documentation.
- A reproducible seed for randomized examples. Modeling examples split data before fitting preprocessing and keep the test set separate from model selection.

Chapter 2 reproduces the techniques in the [publisher's Chapter 2 code](https://github.com/PacktPublishing/scikit-learn-Cookbook-Third-Edition/tree/main/Chapter_2). Its modeling demonstration uses a genuine target rather than treating one output indicator of one-hot encoding as a target. `LabelEncoder` is demonstrated on the target label. The final exercise uses California Housing when the dataset can be downloaded, with a built-in diabetes dataset fallback for offline execution. The notebook prints which dataset was used; the two scores are not directly comparable.

## Run the notebooks

Open a notebook in Google Colab from its GitHub page, or run locally with Python 3.9 or newer:

```bash
python -m venv .venv
# Activate the virtual environment using the command for your operating system.
python -m pip install -r requirements.txt
jupyter notebook
```

In Colab, select **Runtime → Restart session and run all** after opening the notebook. For offline Chapter 2 runs, set `SCIKIT_COOKBOOK_OFFLINE=1` in the process environment before launching Jupyter. Python versions and scikit-learn versions may lead to small output differences.

## Primary sources

- John Sukup, *scikit-learn Cookbook: Over 80 Recipes for Machine Learning in Python with scikit-learn*, 3rd ed., Packt Publishing, 2025.
- [Publisher's example code](https://github.com/PacktPublishing/scikit-learn-Cookbook-Third-Edition).
- [scikit-learn user guide](https://scikit-learn.org/stable/user_guide.html) and [common pitfalls](https://scikit-learn.org/stable/common_pitfalls.html).

The book is credited as the source of its recipes. Explanations and supplementary analysis are written for this assignment.
