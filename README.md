# Bainite Start Prediction – Supplementary Material

This repository contains the supplementary material for the paper:

**"Predictive modeling of the bainite start temperature using Bayesian inference"**  
*Bernd Schuscha, Dominik Brandl, Lorenz Romaner, Ernst Kozeschnik, Reinhold Ebner, Aurélie Jacob, Peter Presoly, Daniel Scheiber*
📄 DOI: [10.1016/j.actamat.2025.121131](https://doi.org/10.1016/j.actamat.2025.121131)

For related datasets used in other work, see:

**CFB Steel Datasets Repository**  
📎 [https://github.com/BerndSchuscha/cfb-steel-datasets](https://github.com/BerndSchuscha/cfb-steel-datasets)



### Dataset: data_Bs.csv

This dataset includes bainite start temperature (`Bs`) and the corresponding alloy compositions from various literature sources.

#### Columns:

- `Nr`: Sample ID or serial number
- `Source`: Citation or dataset source
- `C / wt.%`, `Mn / wt.%`, ..., `Al / wt.%`: Chemical composition in weight percent
- `Bs`: Observed bainite start temperature in °C

#### Notes:
- All values are assumed to be in equilibrium or experimentally measured under well-defined conditions.
- Use with caution if doing regression — some elements (e.g., `V`, `Co`) may be zero or sparse across rows.

## 📈 Posterior Samples: `Model_TDB.csv`
**Location:** `Posterior_Samples/Model_TDB.csv`

This files contain posterior samples of regression coefficients obtained via Bayesian inference, representing the influence of each element on bainite start temperature.

### Columns

- `a_i`: Coefficients in **atomic percent**
- `C0`: Intercept of the model

Each row corresponds to a sample from the posterior distribution, enabling posterior predictive analysis and credible interval estimation.


### 📄 Supplementary: Supplemental_Material.pdf

- Details on data curation
- Model specification
- Posterior analysis
- Additional figures and tables
