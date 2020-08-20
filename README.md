# Make More On-spec Product
 A model to estimate product impurity level using process operating variables.
 
 ## Table of Contents
 1. [Motivation](#Motivation)
 2. [Questions](#Questions)
 3. [Results](#Results)
 4. [File Descriptions](#file-descriptions)
 5. [Licensing, Authors, Acknowledgements](#licensing-authors-acknowledgements)

# Motivation:
In the chemical industry, liquid mixtures are often separated into their components using a process called distillation and is carried out in tall cylindrical columns. The temperature falls as the mixture ascends inside the column and heavy (high boiling point) components condense out of the mixture. A light (low boiling point) product is produced at the top of the tower. The level of impurity in the top product is measured to determine whether the product meets specifications.

Measuring the impurity level can be time consuming resulting in production of off-spec product before a problem is detected. There is a need for a quick and reliable method to estimate the impurity level.

Distillation columns are often instrumented to measure flow rates and temperatures at multiple locations. Flow and temperature measurements are usually fast. A model relating the impurity level to the temperature and flow measurements may provide an acceptable solution.

# Questions:
1.	Might it be possible to predict the impurity level based on measurements of other operating parameters of the distillation column?
2.	Flow and temperature measurements are unavailable from time to time. Can the model be fit and used for prediction when data are missing?
3.	How “good” is the model?

# Results:
The main findings of the analysis can be found here.

# File Descriptions:
There are two files in this repository associated with the above work:
1. An Excel spreadsheet, "Distillation Data 2020-08-20 for Blog.xlsx" containing the data set used to build the model. Label variable is: 'Impurity'. Feature variables are: 'Reflux ratio', 'D/F', 'Pressure', 'T1', 'T2', 'T3', 'T4', 'T5', 'T6', 'T7', 'T8', 'T9', 'T10', 'T11', 'T12', 'T13', 'T14', 'T15'.
2. A Jupyter notebook, "Distillation.ipynb" that carries out the exploratory analysis and modeling.

# Licensing, Authors, Acknowledgements
1. The data set used to create the model was generated using an Excel model of a distillation column developed by A. A. Patwardhan.
2. The distillation column is as described in Example 8.11 in the textbook "Principles of Unit Operations", 2nd ed. by A. S. Foust, L. A. Wenzel, C. W. Clump, L Maus and L. B. Andersen. Publisher John Wiley & Sons, 1980.
3. You may use the files provided above as you wish.
