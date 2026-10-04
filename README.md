# final_project_dataset_selection_Christensen
Link to Notebook: https://colab.research.google.com/drive/1kpXBRRmlnGi35t5vSTy79G8q8rc_3yaf?usp=sharing
## Purpose
#### To propose the Thoracic Surgery Data from the UC Irvine Machine Learning Repository as my dataset for the final project and to explore the dataset and perform an initial assessment of the quality of the dataset.
## Brief description of exploratory analysis
The included analysis is an initial exploration of the Thoracic Surgery Data intended for Binary Classification of patient survival one year after lung surgery. The predictors include a few continuous variables, like measurements for lung health, with the remaining categorical variables, the majority are binary. The counts were calculated for each category, and descriptive statistics were calculated for the numerical variables. Distributions of the lung health measurements were compared by survival group. 
#### 
## Dataset Source and Provenance
#### Dataset: Thoracic Surgery Data from the UC Irvine Machine Learning Repository, donated on 11/12/2013. The data comes from the Wroclaw Thoracic Surgery Centre and includes 470 patients who had major lung surgeries due to lung cancer between 2007 and 2011. The binary target variable is "Risk1Yr", with T(rue) if patient died within a year of the surgery and F(alse) is the patient survived the one year after the surgery. https://archive.ics.uci.edu/dataset/277/thoracic+surgery+data
Lubicz, M., Pawelczyk, K., Rzechonek, A., & Kolodziej, J. (2014). Thoracic Surgery Data [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5Z60N.
## Required packages and libraries
#### Libraries and versions (when applicable):
- pandas  version: 2.2.3
- seaborn version: 0.13.2
- matplotlib.pyplot
- scipy.io with arff
  
## Setup and Installation
#### Load the specified libraries and packages. A message will print when completed successfully.
#### Upload the data file from the link provided above and load into the notebook runtime. A message will print when completed successfully.
## Instructions for executing notebook
#### Go through each chunk of code in order (or select 'Run all' at the beginning.
Beginning with the initial data review, check for missing values and duplicates. Identify the data types for each variable, and the number of rows and columns present. Then review the counts or proportions of each categorical variable, especially the target binary variable to understand how balanced each variable is.  Then load the code for the descriptive statistics to see a summary of the initial variable distributions. This highlights potential outliers in the PRE5 variable, which represents FEV1 or the volume of air exhaled at the end of the first second of a forced expiration. 
## Expected Outputs
During the initial exploratory analysis, the output should include three visualizations: 
- Figure 1 Boxplots of One year Survival Outcome Post Surgery and the Forced Vital Capacity distributions,
- Figure 2 Boxplots of One year Survival Outcome Post Surgery and the distributions of the Forced Exhalation Volume at 1 second,
- Figure 3 Scatterplot Matrix looking at the relationships between the 3 numerical variables, FVC, FEV1, and age at the surgery, and colored by the survival outcome.
- Figure 4 Barplot comparing the counts of each survival outcome for each tumor size group.

## Assumptions and limitations
There are limitations with not having the units for some of the numerical variables, especially as one has a few outliers that should not make sense if they are assumed to be using the same units. If these are nonsensical, they could be missing values, but they might also be real with different units, or be improperly coded in a different way.
