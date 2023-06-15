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

# Justice

Minimizing bias was discussed in the data analysis section. This is a form of fairness as all participants should be treated the same under the model, regardless of race, sex, or socioeconomic status. Justice extends this notion to treating all model subjects as they ought to be treated. For example, a model could be fair but unjust if the model produced equally inaccurate predictions across all groups of interest. Justice requires ethical decision across data collection, data analysis, and model use or deployment. In general, this requires maximizing benefits and minimizing harms across these stages.

Justice during data collection includes fairness when recruiting participants. This effort should attempt to collect a diverse sample. Data collection should also obtain informed consent and protect the privacy of participants. When modeling data, care should be taken to minimize biases, promote interpretability, and ensure accurate predictions across all subgroups of interest. In the model use stage, justice includes equal access to the model and consent of those who will be subject to the model.

![](figures/05_justice.png)
*Figure 5. Fairness and justice as balanced subgroup model performance.*
