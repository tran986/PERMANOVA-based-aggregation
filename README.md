<!-- R package badges -->
![broom](https://img.shields.io/badge/R-broom-blue?style=flat&logo=r)
![ggplot2](https://img.shields.io/badge/R-ggplot2-orange?style=flat&logo=r)
![plotly](https://img.shields.io/badge/R-plotly-green?style=flat&logo=r)
![vegan](https://img.shields.io/badge/R-vegan-purple?style=flat&logo=r)

# Descriptions:
To accommodate for some disadvantages in the current pathway enrichment analytical approaches -  Gene Set Enrichment Analysis or GSEA and Over-Represented Analysis or ORA, we are building a PERMANOVA-based pathway aggregation and analysis pipeline. By utilizing a non-parametric method that is independent from the pathway definition, we has proven that our tool performed better than the older approaches in terms of sensitivity and false positive-controlling.

# Motivation:
1. To evaluate whether our method outperforms GSEA and ORA, we simulate data that not only reflects the complexity of high-dimensional omics but also includes challenging scenarios where traditional methods may fail. We also simulate a scenario that our method may also do not work as well under a statistical assumption.
   Scenario a: Small effect size (biological difference) in gene counts between 2 sample groups.
   Scenario b: Genes in pathways that indicates multi-colinearity (or multivariate property) (e.g, gene A and gene B negatively or positively correlate to one another)
   Scenario c: Genes that have conflicting changes within a sample group (e.g, gene A increased in 5 samples AND decrease in 5 other samples in test groups, compared to controls)
   Scenario d: Test group and control group have unbalanced designs (e.g, unequal sample size, or unequal variances across 2 groups) that potentially can harm PERMANOVA performance

2. To assess our method's performance, we run the mentioned simulated data with our developed tool and compare power and type 2 error with GSEA and ORA

3. We run a real dataset (Type 2 diabetes dataset) on our tool, GSEA and ORA and see if the biological hits are improved in our method

# Results Figure:
<img width="754" height="464" alt="image" src="https://github.com/user-attachments/assets/2a928c3e-d809-493f-a703-ebf968c951cd" />

<img width="1032" height="475" alt="Screenshot 2025-10-02 at 12 05 11 PM" src="https://github.com/user-attachments/assets/70a6d316-be3a-4df8-95b3-44c810cfbc30" />

<img width="709" height="380" alt="Screenshot 2025-10-02 at 12 05 54 PM" src="https://github.com/user-attachments/assets/44928f0c-7d8d-413e-a1c5-5d2d416bbc97" />

<img width="516" height="328" alt="image" src="https://github.com/user-attachments/assets/c2f9febe-2480-412e-86e9-5551ff888d33" />

<img width="868" height="506" alt="Screenshot 2025-10-02 at 12 07 12 PM" src="https://github.com/user-attachments/assets/fc1bbf4b-a328-442f-b16d-d63db33f3c0b" />

<img width="945" height="486" alt="Screenshot 2025-10-02 at 12 07 38 PM" src="https://github.com/user-attachments/assets/1dfe6b23-37d7-491c-816e-b152e7d530fc" />

# Conclusions, Limitations and Future Directions:

# Citations:
