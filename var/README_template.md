# International SARS-CoV-2 genomic surveillance

This repository uses the [genomicsurveillance](https://github.com/gerstung-lab/genomicsurveillance) model to estimate daily growth rates of a variety of SARS-CoV-2 lineages in selected countries. It fits a logistic linear model to daily lineage counts using a Dirichlet-Multinomial model. The growth rates are modelled in a hierarchical Bayesian fashion using stochastic variational inference. 

The model is described in detail in our publication [Genomic reconstruction of the SARS-CoV-2 epidemic in England](https://www.nature.com/articles/s41586-021-04069-y).

The current code pulls aggregated data from [cov-spectrum.org](cov-spectrum.org); the underlying data is proved by GISAID. Case data is from [Our World in Data](https://ourworldindata.org/explorers/coronavirus-data-explorer).

Latest update: {date}, based on {n_genomes} genomic sequences.

![Map](plots/variant-map.png)

## Growth rates
![Growth rates](plots/growth-rate-latest.png)

Each dot represents a country (MAP estimate). Bars denote the shared mean, errorbars are the 90% posterior interval.

### In tabular form, per country

Other countries are grouped into geographic regions.

<small>{growth_rate_tab}</small>

Shown is the daily growth advantage over {baseline} in percent. Errors are standard errors.

## Variant share by country

The variant share is extrapolated from the last day with observed data. In countries where a variant hasn't been detected yet, it is assumed to be introduced at levels of 1% of the international average. 

![Variant share by country](plots/variant-share-latest.png)

Latest estimated variant proportion.

![Variant share by country](plots/variant-share-bar.png)

### In tabular form, per country

<small>{var_prop_tab}</small>

Shown is the estimated variant proportion on {date} in percent. 

Values in parentheses mean that the variant has not been detected in the specific country and are imputed instead.
