# Bayesian Data Analysis for Crossover-Design Experiments

This repository contains the replication package of the study, where we investigate how Bayesian data analysis (including Bayesian modeling) can address threats to validity of experiments using a crossover design at analysis time.

## Structure

This repository contains the following items:

* data/ : directory for all raw data
  * state-of-practice/ : data connected to the evaluation of the state of practice
    * `data-extraction.xlsx` : extracted data
    * `data-extraction-ira.xlsx` : extraction overlap for inter-rater agreement
* src/ : directory for all code and scripts
  * `reproduction.Rmd` : reproduction of the study by Vegas et al.[^1]
  * `sop-interrater-agreement.Rmd` : calculation of the inter-rater agreement of the data extraction
  * `sop-visualization.Rmd` : visualization of the results from the data extraction
  
## Usage

To use the artifacts in this repository, conduct the following steps:

1. Obtain the data from the reproduced study[^1] by reaching out to the authors.
2. Place this data in the directory `data\tse-2016-vegas` and rename it to `data.sav`.
3. Execute the `reproduction.Rmd` file.
  
[^1]: Vegas, S., Apa, C., & Juristo, N. (2015). Crossover designs in software engineering experiments: Benefits and perils. IEEE Transactions on Software Engineering, 42(2), 120-135.