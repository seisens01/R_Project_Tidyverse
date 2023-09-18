# August2.2023
# R_Tidyverse_Exercises_NHANES_drug_use_by_gender
Plots and descriptive statistics for NHANES data on self-reported drug use in men and women from 2010-2016

The purpose of this project is to apply lessons learned about dplyr and ggplot2 from the DataCamp Interactive Course, "Introduction to the Tidyverse" (https://app.datacamp.com/learn/courses/introduction-to-the-tidyverse), taught online by David Robinson, to explore a dataset containing real data. The R dplyr package allows one to manipulate data in R by filtering, sorting, and summarizing a dataset and the ggplot2 package allows for visualization of data with various types of plots. I completed the course in July 2023.

I am interested in being a public health data analyst, with special interest in substance use and psychiatric disorders. I chose to download demographic and questionnaire data from the National Health and Nutrition Examination Survey (NHANES; see citation at end of document) public use data files. The NHANES is a set of studies used to assess health and nutritional status of adults and children in the United States. The NHANES survey has been a continuous program since 1999, examining a nationally representative sample of ~5000 people per year.

For the current project, I focused on adults 18+ years, from cross-sectional cohorts assessed at 4 different time points (2009-2010, 2011-2012, 2013-2014, 2015-2016). Demographic ("Demographic Variables and Sample Weights" data file) and questionnaire ("Drug Use" data file) data were downloaded as SAS Xport Transport file types, viewed in the freely available SAS Universal Viewer and saved as .csv files. .CSV files were merged (inner join) on the "SEQN" participant unique id code field and cleaned (removal of duplicates and fields of non-interest) using Power Query Editor in Excel. As the current project focuses on R tidyverse exercises, I do not include visual demonstration of these processes but may add snapshots at a future time. The resulting csv file with merged demographic and drug use fields was loaded into R Studio for manipulation and visualization with dplyr and ggplot2 tools, respectively. As I continue my journey in learning hot to use R in data analytics, I will likely update this repository and improve the plot aesthetics. So stay tuned!

**Important disclosures/caveats:** As the current project is for demonstration of R tidyverse methods of manipulating and visualizing data only, no statistical analyses are performed. Descriptive statistics and plots are for demonstration of tool use only and sample data is not weighted as it would be for statistical analysis (https://wwwn.cdc.gov/nchs/data/nhanes/analyticguidelines/11-16-analytic-guidelines.pdf). The unweighted data shown in this project may therefore not be representative of the U.S. civilian non-institutionalized population and no inferences should be drawn from these visualization or descriptive statistics.  I intend to weight the data properly and update this project in the near future. This repository is not a guide to using R but rather reflects my learning how to apply basic tidyverse concepts to real data concerning drug use patterns in the U.S.

**NHANES Data Reference:**
Centers for Disease Control and Prevention (CDC). National Center for Health Statistics (NCHS). National Health and Nutrition Examination Survey Data. Hyattsville, MD: U.S. Department of Health and Human Services, Centers for Disease Control and Prevention, 2023, https://wwwn.cdc.gov/nchs/nhanes/.
