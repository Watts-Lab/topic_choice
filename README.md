# The Role of Topic Choice in Cross-Partisan Conversations: Dataset and Analysis

This repository contains the full dataset and analysis code for the paper:

**"The Role of Topic Choice in Cross-Partisan Conversations"**
_James Houghton, Gus Cooney, Duncan Watts_
(2026) [https://osf.io/preprints/socarxiv/nygt3_v3/](https://osf.io/preprints/socarxiv/nygt3_v1/)

---

## Abstract

_Affective polarization in the United States — animosity between Republicans and Democrats — has escalated for decades, threatening the health of American democracy. Research on intergroup contact suggests that talking across party lines can reduce polarization, yet studies disagree on whether confronting or avoiding political disagreement is the more effective strategy. We address this debate using a large-scale integrative experiment in which Republicans and Democrats engaged in face-to-face video conversations, with levels of disagreement and political relevance systematically varied across a diverse set of topics. While some topics reduced affective polarization more than others, how "political" a topic was did not predict which conversations went well. Moreover, topic assignment explained just 2% of the variance in individual outcomes, with people assigned to the same topic often having entirely different experiences. What did correlate with conversational success was how individuals experienced the interaction (i.e., whether their partner listened, took their perspective, and made them feel heard). We suggest a shift in focus from choosing the "right" topic to understanding the detailed interactional dynamics that make cross-partisan conversation succeed._

## Repository Contents

### Code Notebooks

- **`analyze_study_data.ipynb`**
  Reproduces all figures and tables used in the paper. Contains code for all study outcome analyses.

- **`analyze_topics_pretest.ipynb`**
  Documents the pre-survey process used to select the final set of 10 discussion topics from an initial pool of 174. Includes exploratory analyses and figures for the supplement.

### Figures

All figures are exported as both PDF and PNG:

#### From `analyze_study_data.ipynb`

| File                               | Description                                                     |
| ---------------------------------- | --------------------------------------------------------------- |
| `fig_2_topic_effects`              | Figure 2: Estimated effects of each topic on both outcomes      |
| `fig_3_single_predictors`          | Figure 3: Single-predictor regression panels                    |
| `fig_4_cross_predictor_comparison` | Figure 4: Cross-predictor comparison of effect sizes            |
| `fig_S4_balanced_samples`          | Figure S4: Sample balance across experimental conditions        |
| `fig_S5_change_histograms_kde`     | Figure S5: Outcome distributions (KDE)                          |
| `fig_S6_no_conversation_control`   | Figure S6: Test-retest reliability from no-conversation control |
| `fig_S7_disagreement_by_topic`     | Figure S7: Effect of dyadic disagreement broken out by topic    |
| `fig_S8_manipulation_check`        | Figure S8: Partner party recall (manipulation check)            |

#### From `analyze_topics_pretest.ipynb`

| File                                                  | Description                                                           |
| ----------------------------------------------------- | --------------------------------------------------------------------- |
| `fig_S1_example_topics_polarization_contentiousness`  | Figure S1: Example topics from the full pool                          |
| `fig_S3_selected_topics_partisanship_contentiousness` | Figure S3: Selected topics plotted on partisanship vs contentiousness |

### Tables

All tables are rendered as pandas DataFrames within the notebook:

| Table     | Description                                                                            |
| --------- | -------------------------------------------------------------------------------------- |
| Table 1   | Primary regressions with cluster bootstrap inference (resampling topics)               |
| Table 2   | Pre-treatment individual attributes (attitudes, personality, demographics)             |
| Table 3   | Political attitude predictors of attitude change                                       |
| Table 4   | Conversation dynamics predictors with topic fixed effects and dyad-clustered SEs       |
| Table 5   | Discussion topics and their positions on topic-level dimensions                        |
| Table S1  | R-squared values by category of predictors                                             |
| Table S2  | Scaling ranges for cross-predictor comparison                                          |
| Table S3  | Bayesian ROPE analysis for single-predictor regressions                                |
| Table S4  | Effect of primary predictors on secondary outcomes (single regressions, BH-corrected)  |
| Table S5  | Primary regressions excluding floor-effect participants                                |
| Table S6  | Floor effects on political attitude predictors                                         |
| Table S7  | Balance check: pretest measures regressed on primary dimensions (per-IV BH correction) |
| Table S8  | Primary regressions controlling for pre-discussion affect                              |
| Table S9  | Comparison of attritters and non-attritters on individual-level predictors             |
| Table S10 | Primary regressions with attritters included (worst-case imputation)                   |

### Data Files

#### Topic Definitions

- `topic_list.csv`
  Contains full topic texts and short name identifiers used in code and figures.

- `topic_moments.csv`
  Summary statistics for topic-level dimensions.

#### Pretest Data

- `topic_pretest_identity_threat_responses.csv`
  Qualtrics survey data capturing participants' fear of judgment (identity threat) for each topic.

- `topic_pretest_responses.csv`
  Main pre-survey dataset used to estimate contentiousness and partisanship for topic selection.

#### Study Data

- `topic_study_responses.csv`
  Follow-up topic feature responses collected during the study to refine feature estimates.

- `study_data.csv`
  Final merged and cleaned dataset from the experiment, ready for analysis.

- `no_conversation_control_data.csv`
  Test-retest control data from participants who completed pre- and post-test measures without a conversation.

## Citation

Please cite the study as:

> Houghton, J., Cooney, G., Watts, D. "The Role of Topic Choice in Cross-Partisan Conversations." 2026.
