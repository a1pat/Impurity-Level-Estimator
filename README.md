README.md

## Table of Contents
1. [Motivation](#motivation)
2. [Questions](#questions)
3. [Results](#results)
4. [File Descriptions](#file-descriptions)
5. [Libraries](#libraries)
6. [Licensing, Authors, Acknowledgements](#licensing-authors-acknowledgements)

# Motivation:
If you drive past a petrochemical plant, you will probably wonder what the tall shiny structures are. It is likely that they are distillation columns used to obtain purified liquids from mixtures. For example, distillation is used to produce alcoholic beverages, gasoline and distilled water.
In the distillation, as with other processes, the goal is to produce a product that the customer wants — profitably. The customer requires that the concentration of impurity in the product be within a specified limit. If the impurity is outside the limit, the product must be thrown away or recycled. If the impurity is well within the limit, there is “give away” of quality and processing costs are higher than necessary. Thus, the ability to measure the impurity quickly is essential for meeting customer requirements at minimum cost.

Measuring the impurity level accurately using an instrument called an “analyzer” can be time consuming resulting in production of off-spec product before a problem is detected. There is a need for a quick and reliable method to estimate the impurity level.
Distillation columns are often instrumented to measure other operating parameters — pressures, flow rates and temperatures at multiple locations. These measurements are almost instantaneous. A model relating the impurity level to the temperature and flow measurements may provide a fast and acceptable solution for quickly estimating the impurity level.

# Questions:
1.	Distillation columns are often instrumented to measure other operating parameters — pressure, flow rates and temperatures at multiple locations. Might it be possible to estimate the impurity level based on other operating parameters?
2.	Could the impurity level be estimated even if some of the other parameters are occasionally unavailable?
3.	Will the impurity-estimation method be accurate enough for deployment?

# Results:
The main findings of the analysis can be found here.

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
