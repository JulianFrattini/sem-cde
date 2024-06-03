# Crossover Designs in Software Engineering Experiments: State of Practice

This repository contains the replication package of the study where we investigate the state of practice of analyzing data obtained from crossover design experiments in software engineering research.
The investigation serves as a reflection on the impact of the guidelines written by Vegas et al.[^1]

## Structure

This repository contains the following items:

* data/ : directory for all raw data
  * state-of-practice/ : data connected to the evaluation of the state of practice
    * `data-extraction.xlsx` : extracted data
    * `data-extraction-ira.xlsx` : extraction overlap for inter-rater agreement
    * `study-inclusion.xlsx` : results from the inclusion phase
* figures/ : directory for all figures
  * graphml/ : subdirectory for all raw `.graphml` files of figures
* material/ : directory for all supplementary material for replicating the study
  * `guidelines-extraction.pdf` : guidelines dictating the data extraction phase
  * `guidelines-inclusion.pdf` : guidelines dictating the study inclusion phase
* src/ : directory for all code and scripts
  * html/ : pre-compiled PDF versions (using `knitr`) of all `.Rmd` files for easier access
  * `reproduction.Rmd` : reproduction of the original study by Vegas et al.[^1]
  * `sop-interrater-agreement.Rmd` : calculation of the inter-rater agreement of the data extraction
  * `sop-visualization.Rmd` : visualization of the results from the data extraction
  
## Usage

This repository aims to support several use cases.
The following subsections provide instructions for each use case.

### Replicating the original Study

To replicate the data analysis presented in Section 7 of the guidelines by Vegas et al.[^1], conduct the following steps.

1. Obtain the data from the study[^1] by reaching out to the authors. Since the data is sensitive, we cannot publish it in this repository.
2. Place this data in the directory `data\tse-2016-vegas` and rename it to `data.sav`.
3. Execute the `reproduction.Rmd` notebook.

If you cannot obtain the data at this point, look at the `html` version of the notebook contained in the respective subdirectory.
This version is pre-compiled with the original data and still showcases the data analysis steps.

### Investigating Details of this Study

To understand our study in more detail, consider the follow steps.

1. Review the `guidelines-inclusion.pdf` to understand our study inclusion phase and compare them to the results in the `data-inclusion.xslx` sheet.
2. Review the `guidelines-extraction.pdf` to understand our data extraction phase and compare them to the results in the `data-extraction.xslx` sheet.
3. Find the data extraction overlap in the `data-extraction-ira.xlsx` sheet. The inter-rater agreement is calculated in the `sop-interrater-agreement.Rmd` file.
4. Find the generation of figures from the raw data in the `sop-visualization.Rmd` file.

### Replicating this Study

To replicate the study which this replication package refers to, conduct the following steps.

1. Review the `guidelines-inclusion.pdf` and apply them to a set of primary studies. You can use the `data-inclusion.xslx` sheet as inspiration for collecting the data,
2. Review the `guidelines-extraction.pdf` and apply them to the included primary studies. You can use the `data-extraction.xslx` sheet as inspiration for collecting the data,
3. Use the `sop-visualization.Rmd` to generate figures from the extracted data.
  
[^1]: Vegas, S., Apa, C., & Juristo, N. (2015). Crossover designs in software engineering experiments: Benefits and perils. IEEE Transactions on Software Engineering, 42(2), 120-135.