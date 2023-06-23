# Replicathon 2022 (IQ BIO REU, UPR-RP)

## Schedule

*Friday*

|Starts | Ends  | Activity                                                               |
|-------|-------|------------------------------------------------------------------------|
| 10    | 11    | Welcome and presentation on the subject                                |
| 11    | 11:15 | Team building & team names                                            |
| 11:15 | 12    | Github setup, discussion of reinforcement q's, basic tutorials (0a-1b) |
| 12    | 1     | Lunch + networking + q's about data and problem                        |
| 1     | 2     | Tutorials 2a + 2b                                                     |
| 2     | 3:15  | Exploratory data analysis + module selection                           |
| 3:15  | 3:30  | EDA discussion                                                         |
| 3:30  | 4:30  | Work on module analysis                                                |
| 4:30  | 5:00  | Brief regroup + Ice Cream                                              |


*Saturday*

|Starts| Ends | Activity                            |
|------|------|-------------------------------------|
| 10   | 11   | Continue (& finish) Module analysis |
| 11   | 12   | Teams will work on presentations    |
| 12   | 1    | Lunch + networking                  |
| 1    | 2:30 | Presentations                       |
| 2:30 | 3    | Regroup and final thoughts          |

## Getting Started

Check out the [**introduction slides**](https://speakerdeck.com/merci/replicathon-2022) to review the goals and context for the event! If you're interested in learning more, links to relevant papers are included in the [Useful Links](#useful-links) section below. There are a couple ways that you can get started.

1. **If you have R already installed and ready to go**, clone or download [this repository](https://github.com/kstreet13/PR2021replicathon) to your computer and open the `.Rmd` files with [RStudio](https://rstudio.com/) or any other editor that you're comfortable using.
2. **If you don't have R installed on your computer**, create a free account with [RStudio Cloud](https://rstudio.cloud/), click the blue dropdown arrow next to **[New Project]**, select **[New Project from Git Repo]**, and enter this GitHub repo URL: https://github.com/Mercedeh66/PR2022replicathon

## Reinforcement Questions

After going over the introductory slides and presentation, work through these *reinforcement questions* to make sure you and your team has a good understanding of replicability and the problem.

- [`reinforcement questions`](tutorials/00_reinforcement_questions.md)

## Main Analysis Template

* [`analysis_template.Rmd`](analysis_template.Rmd) : R markdown template which each team will use to create a fully reproducible analysis with the goal of assessing and interpreting the replicability of two pharmacogenomic experiments. This document will contain all of the text and code of their analyses, which are guided by a series of questions. The tools and concepts needed to answer the questions are explored in the tutorials.

## Datasets

Data files are included under the `data` folder.

* `rawPharmacoData.rds` : raw data file generated by `downloadData.R` that contains drug response data at every dose for each cell line and drug used in both studies. 

* `summarizedPharmacoData.rds` : summarized data file generated by `downloadData.R` that contains drug response data (combined over all doses) for each cell line and drug used in both studies.

* `modelSummarizedPharmacoData.rds` : summarized data file generated in the `supplement_dose_response.Rmd` tutorial that contains recomputed drug response data (combined over all doses) for each cell line and drug used in both studies.

## Tutorials

Tutorials are included under the `tutorial` folder.

Each tutorial contains text and code that explores various aspects of data science, replicability, and reproducibility. Tutorial `0a` provides a gentle introduction to R for those with limited programming experience, and Tutorial `0b` introduces some of the main functions in the `dplyr` and `tidyr` packages. Tutorials `1a` and `1b` get us started with exploring the two original datasets from the CCLE and GDSC studies, `rawPharmacoData.rds` and `summarizedPharmacoData.rds`. Tutorials `2a` and `2b` dig deeper into specific issues that can impact replicability and provide ideas for things to look into for this Replicathon. Finally, the Supplementary Tutorials provide more details that are useful but not immediately necessary for getting started.

* [`0a_R_basics.Rmd`](tutorials/0a_R_basics.Rmd) : "Introduction to R Basics"

* [`0b_R_tidyverse.Rmd`](tutorials/0b_R_tidyverse.Rmd) : "Introduction to the Tidyverse"

* [`1a_explore_rawData.Rmd`](tutorials/1a_explore_rawData.Rmd) : "Exploring Pharmacological Data with the `rawPharmacoData` Dataset"

* [`1b_explore_summarizedData.Rmd`](tutorials/1b_explore_summarizedData.Rmd) : "Exploring Replicability with the `summarizedPharmacoData` Dataset"

* [`2a_deeper_subgroups.Rmd`](tutorials/2a_deeper_subgroups.Rmd) : "Digging Deeper with Cell Line and Drug Subgroups"

* [`2b_deeper_summarization.Rmd`](tutorials/2b_deeper_summarization.Rmd) : "Digging Deeper with Drug Response Summarization"

**Supplementary Tutorials**

* [`supplement_correlation.Rmd`](tutorials/supplement_correlation.Rmd) : "Correlation Measures"

* [`supplement_dose_response.Rmd`](tutorials/supplement_dose_response.Rmd) : "Dose-Response Modeling"

* [`supplement_PCA_clustering.Rmd`](tutorials/supplement_PCA_clustering.Rmd) : "Exploring High Dimensional Data with PCA and Clustering"

## Code to generate data files (You do not need to use this)

For full reproducibility, this is the script to generate the `RDS` files. This step has already been done for you, and the data files should be available as part of this repository without running the script.

* [`downloadData.R`](downloadData.R) : a script that uses the [PharmacoGx](http://bioconductor.org/packages/PharmacoGx/) package to format two datasets (raw and summary level) and save them as `RDS` files. 

## Useful Links

* [CCLE (Cancer Cell Line Encyclopedia) Study](https://www.ncbi.nlm.nih.gov/pubmed/22460905) from March 2012

* [GDSC (Genomics of Drug Sensitivity in Cancer) Study](https://www.ncbi.nlm.nih.gov/pubmed/22460902) from March 2012

* [Reanalysis of CCLE and GDSC](https://www.ncbi.nlm.nih.gov/pubmed/24284626) from December 2013

* [Commentary 1 on the reanalysis](https://www.ncbi.nlm.nih.gov/pubmed/27905415) from December 2016

* [Commentary 2 on the reanalysis](https://www.ncbi.nlm.nih.gov/pubmed/27905421) from December 2016

* [Commentary 3 on the reanalysis](https://www.ncbi.nlm.nih.gov/pubmed/27905419) from December 2016

* [Revisiting the reanalysis](https://www.ncbi.nlm.nih.gov/pubmed/28928933) from August 2017

## Code of Conduct

To ensure a safe, enjoyable, and friendly experience for everyone who participates, we have a strict [code of conduct](code_of_conduct.md) that all participants are expected to follow.


