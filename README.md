# Massachusetts Traffic Stop Analysis

**Tools:** R, dplyr, ggplot2, tidyverse

## Overview

This project examines the relationship between driver race and gender and police traffic stop outcomes in Massachusetts. Using data from the Stanford Open Policing Project, the analysis investigates differences in search rates, arrest rates, contraband discoveries, and traffic stop escalation.

The study analyzes approximately 3.4 million Massachusetts traffic stops recorded between December 2006 and December 2015.

## Research Questions

- Are search and arrest rates different across racial and gender groups?
- Do disparities become more pronounced when race and gender are considered together?
- How do contraband discovery rates compare with search rates across demographic groups?
- What patterns emerge in the progression from traffic stops to searches, contraband discoveries, and arrests?

## Methods & Analysis

### Exploratory Data Analysis

- Examined the distribution of traffic stops across racial and gender groups.
- Calculated and visualized search, arrest, and contraband discovery rates.
- Compared outcomes across combined race and gender categories.

### Statistical Inference

- Constructed 95% confidence intervals for differences in stop proportions and demographic search and arrest rates.
- Used logistic regression to examine the relationship between driver demographics and search outcomes.
- Developed an interaction model to investigate the combined relationship between race and gender and the likelihood of a search.

### Extended Analysis: Search-Efficiency Index

Developed a custom index comparing search frequency with the rate of contraband discovery.

**Search-Efficiency Index = Search Rate / Contraband Hit Rate**

The index was calculated across race and gender groups to examine whether higher search frequencies corresponded to proportionally higher contraband discovery rates. It provided an additional descriptive perspective on differences in search outcomes.

This index is an exploratory measure developed for this project, not a standardized or validated measure of discriminatory policing.

## Key Findings

- Male drivers experienced higher search and arrest rates than female drivers.
- Hispanic and Black drivers had higher observed search and arrest rates than White drivers.
- Black and Hispanic male drivers showed particularly high search rates when race and gender were examined jointly.
- The extended index highlighted differences in the relationship between search frequency and contraband discovery across demographic groups.

These findings describe associations in observational data and do not establish that race or gender directly caused differences in police stop outcomes.

## My Contributions

This was a collaborative course research project. I worked with another team member on data handling and preparation. I independently developed the analytical reasoning and statistical approach, conducted the analysis and interpretation, and wrote the research paper.

My work included developing the research questions, selecting and applying statistical methods, interpreting confidence intervals and logistic regression models, developing the custom search-efficiency index, and communicating the findings.

## Technologies

- **R:** Statistical computing and analysis
- **dplyr:** Data manipulation, filtering, grouping, and summarization
- **ggplot2:** Data visualization
- **tidyverse:** Data analysis workflow

## Data Source

Stanford Open Policing Project  
https://openpolicing.stanford.edu/data/

The original Massachusetts traffic-stop dataset is not included in this repository. Refer to the source above for access to the data.

## Reproducing the Analysis

The analysis was conducted in R using the tidyverse, dplyr, and ggplot2 packages.

To reproduce the analysis:

1. Download the Massachusetts traffic-stop dataset from the Stanford Open Policing Project.
2. Install the required R packages.
3. Open `analysis/traffic_stop_analysis.Rmd` in RStudio.
4. Update the dataset path to point to your downloaded CSV file.
5. Knit the R Markdown file to run the analysis and generate the output.

## Limitations

The analysis is observational and cannot establish causation. Additional factors, including traffic-stop reasons, geographic differences, socioeconomic conditions, and individual police department policies, may help explain the observed patterns.

The custom search-efficiency index is an exploratory measure developed for this project, not a standardized measure of discriminatory policing.

## Repository Contents

- `README.md` — Project overview, methodology, findings, and contributions.
- `analysis/` — R Markdown analysis and supporting code.
- `report/` — Final research paper, if included.

## Reproducing the Analysis

The analysis was conducted in R using the tidyverse, dplyr, and ggplot2 packages.

To reproduce the analysis:

1. Download the Massachusetts traffic-stop dataset from the [Stanford Open Policing Project](https://openpolicing.stanford.edu/data/).
2. Create a folder named `data` in the root directory of this repository.
3. Place the downloaded CSV file (`ma_statewide_2020_04_01.csv`) inside the `data` folder.
4. Open the R Markdown file in the `analysis/` folder using RStudio.
5. Set the working directory to the R Markdown file's location using **Session → Set Working Directory → To Source File Location**.
6. Knit the R Markdown file to generate the PDF report.
