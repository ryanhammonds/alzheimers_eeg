---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Model Use

## Appropriate & Inappropriate Use

Once a classification model is trained, it will be deployed to help doctors diagnose and treat individuals developing AD. Although there is no cure for AD, early interventions and diagnosis could extend or improve quality of life. This could provide opportunities for future research in protecting or slowing the progression of AD, starting in the preclinical phase. Insights may also be gained from the sparse interpretable model, such as which brain regions and spectral features are disrupted over the course of AD. This could subsequently be used to evaluate the efficacy of novel treatments.

Appropriate model use requires consent from those who are to be subject to the model. Some people may prefer to not know that their future will be impacted with AD. Concerns have also been raised regarding the use of models by insurers to deny coverage or charge high premiums to those at risk for developing AD (Davis 2011). To safeguard against this, trained models will only be provided to doctors, researchers, or other authorized individuals to ensure consent is obtained prior to subjecting people to the model.

## Interpretability

As previously discussed, interpretability will be provided through the use of a risk calibrated, sparse logistic regression (RiskSLIM; Ustun & Rudin, 2016). This method incorporates feature selection through sparsity, or promoting many of the linear weights to be zero through loss function penalties. The output of RiskSLIM is an interactive risk prediction table with a small number of features used to make the AD prediction (Fig. 4). This method provides improved interpretability compared to neural networks, or even standard logistic regression, as there would be greater number of non-zero weights and more nuanced interpretation of feature importance.

 ![](figures/04_model_use.png) *Figure 4. Model interpretability provided as a risk table for predicting AD disease. Each row is a single spectral feature’s contribution to the overall risk score and predicted risk.*
