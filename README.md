README.md

## Table of Contents
1. [Motivation](#Motivation)
2. [Questions](#Questions)
3. [Results](#Results)
4. [File Descriptions](#file-descriptions)
5. [Libraries](#libraries)
6. [Licensing, Authors, Acknowledgements](#licensing-authors-acknowledgements)

# Motivation:
In the chemical processing industry, liquid mixtures are often separated into their components using a process called distillation and is carried out in tall cylindrical columns. The temperature falls as the mixture ascends inside the column and heavy (high boiling point) components condense out of the mixture. A light (low boiling point) product is produced at the top of the tower. The level of impurity in the top product is measured to determine whether the product meets specifications.

Measuring the impurity level can be time consuming resulting in production of off-spec product before a problem is detected. There is a need for a quick and reliable method to estimate the impurity level.

Distillation columns are often instrumented to measure flow rates and temperatures at multiple locations. Flow and temperature measurements are usually fast. A model relating the impurity level to the temperature and flow measurements may provide an acceptable solution.

# Questions:
1.	Might it be possible to predict the impurity level based on measurements of other operating parameters of the distillation column?
2.	Flow and temperature measurements are unavailable from time to time. How can estimates be made when data are missing?
3.	Is the estimator good enough for deployment?

# Results:
The main findings of the analysis are:
1. The impurity level has good correlations with other operating parameters, and it should be possible to predict the ipurity level using the other parameters;
2. Missing values can be replaced using the mean for that column (measurement);
3. The linear model does not have the accuracy required for deployment.

Possible avenues for exploration (not part of this analysis:
1. Try other methods of imputing missing values;
2. Try using the log of the impurity;
3. Use a more general nonlinear model such as a neural net;
4. Ue the estimator developed here and offset it from time to time when an accurate impurity analysis is available.

# File Descriptions:
There are two files in this repository associated with the above work:
1. An Excel spreadsheet, "Distillation Data 2020-08-20 for Blog.xlsx" containing the data set used to build the model. Label variable is: 'Impurity'. Feature variables are: 'Reflux ratio', 'D/F', 'Pressure', 'T1', 'T2', 'T3', 'T4', 'T5', 'T6', 'T7', 'T8', 'T9', 'T10', 'T11', 'T12', 'T13', 'T14', 'T15'.
2. A Jupyter notebook, "Distillation.ipynb" that carries out the exploratory analysis and modeling.

# Libraries
No libraries are used beyond those in an Anaconda installation.

# Licensing, Authors, Acknowledgements
1. The data set used to create the model was generated using an Excel model of a distillation column developed by A. A. Patwardhan.
2. The distillation column is as described in Example 8.11 in the textbook "Principles of Unit Operations", 2nd ed. by A. S. Foust, L. A. Wenzel, C. W. Clump, L Maus and L. B. Andersen. Publisher John Wiley & Sons, 1980.
3. You may use the two files provided above as you wish.
