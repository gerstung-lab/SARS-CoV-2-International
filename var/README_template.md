# International SARS-CoV-2 genomic surveillance

This repository uses the `genomicsurveillance` model to estimate daily growth rates of a variety of SARS-CoV-2 lineages in selected countries.

It pulls data from `cov-spectrum.org` on a daily basis.

Latest update: {date}.

## Growth rates
![Growth rates](plots/growth-rate-latest.png)

### In tabular form, per country

{growth_rate_tab}

Shown is the daily growth advantage over {baseline} in percent.

## Variant share by country

![Variant share by country](plots/variant-share-latest.png)

### In tabular form, per country

{var_prop_tab}

Shown is the estimated variant proportion on {date} in percent. 

Values in parentheses mean that the variant has not been detected in the specific country and are imputed instead.
