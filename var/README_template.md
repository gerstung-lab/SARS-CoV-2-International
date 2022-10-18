# International SARS-CoV-2 genomic surveillance

This repository uses the `genomicsurveillance` model to estimate daily growth rates of a variety of SARS-CoV-2 lineages in selected countries.

It pulls data from `cov-spectrum.org` on a daily basis.

Latest update: {date}.

## Growth rates
![Growth rates](plots/growth-rate-latest.png)

### In tabular form, per country

<small><pre>{growth_rate_tab}</pre></small>

Shown is the daily growth advantage over {baseline} in percent. Errors are standard errors.

## Variant share by country

![Variant share by country](plots/variant-share-latest.png)

Latest estimate variant proportion

![Variant share by country](plots/variant-share-bar.png)

### In tabular form, per country

<small><pre>{var_prop_tab}</pre></small>

Shown is the estimated variant proportion on {date} in percent. 

Values in parentheses mean that the variant has not been detected in the specific country and are imputed instead.
