# The Role of Topic Choice in Cross-Partisan Conversations: Dataset and Analysis

This repository contains the full dataset and analysis code for the paper:
**“The Role of Topic Choice in Cross-Partisan Conversations”**
_Authors: James Houghton, Duncan Watts_
_Date: Under Review 2025_

---

## 🗃️ Overview

This study investigates whether certain conversation topics are more effective than others at improving affective attitudes toward political outgroups. We assess how features such as partisanship, contentiousness, and identity threat shape cross-partisan dialogue outcomes.

We find that:

- While some topics consistently produce better average results, the topics political nature or the disagreement between participants explain little of that variation.
- Outcomes varied widely within topics.
- Individual-level attributes (demographics, psychometrics, and attitudes attributes) were also poor predictors of outcomes.
- Behavioral self-reports, such as listening and perspective-taking, strongly correlate with positive affective change, though these measures are post hoc and correlational, implying the need for a study that manipulates behaviors.

## 📂 Repository Contents

### 🧪 Code Notebooks

- **`analyze_study_data.ipynb`**
  Reproduces all figures and tables used in the paper. Contains code for all study outcome analyses.

- **`analyze_topics_pretest.ipynb`**
  Documents the pre-survey process used to select the final set of 10 discussion topics from an initial pool of 174. Includes exploratory analyses and figures for the supplement.

### 📊 Figures (PDFs)

All figures used in the main paper and supplement are exported as standalone PDFs:

- `fig_balanced_samples.pdf` – sample balancing overview
- `fig_topic_effects.pdf` – estimated effects of each topic
- `fig_topic_identity_threat.pdf` – identity threat ratings per topic
- `fig_disagreement_predictors.pdf` – predictor slopes from regression models
- `fig_change_histograms_kde.pdf` – outcome distributions
- ...and others (see file list for full set)

### 📀 Tables (LaTeX exports)

- `table_primary_predictors.tex`, `table_secondary_predictors_attributes.tex`, `table_secondary_predictors_behavior.tex` – coefficient tables from regression models
- `table_r2_comparison.tex` – explained variation by predictor group
- `table_univariate_rope.tex` – Bayesian ROPE analysis results
- `table_attrition_t_test.tex` – sample attrition checks

### 📁 Data Files

#### Topic Definitions

- `topic_list.csv`
  Contains full topic texts and short name identifiers used in code and figures.

#### Pretest Data

- `topic_pretest_identity_threat_responses.csv`
  Qualtrics survey data capturing participants’ fear of judgment (identity threat) for each topic.

- `topic_pretest_responses.csv`
  Main pre-survey dataset used to estimate contentiousness and partisanship for topic selection.

#### Study Data

- `topic_study_responses.csv`
  Follow-up topic feature responses collected during the study to refine feature estimates.

- `study_data.csv`
  Final merged and cleaned dataset from the experiment, ready for analysis.

## 🔍 Citation

Please cite the study as:

> Houghton, J., Watts, D. “The Role of Topic Choice in Cross-Partisan Conversations.”
