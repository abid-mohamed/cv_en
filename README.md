# Mohamed ABID

# SKILLS

|&emsp;**R** &emsp;&emsp;&emsp;&emsp;|&emsp;**JSON**&emsp;&emsp;&emsp;&emsp; &emsp; |&emsp;**Ensemble Model**&emsp;&emsp;&emsp;|&emsp;**Survival Analysis** <br/>
|&emsp;**Python** &emsp; |&emsp;**Neo4j**&emsp;&emsp;&emsp;&emsp;&emsp; |&emsp;**Machine Learning** &emsp; &emsp;|&emsp;**Data Visualization** <br/>
|&emsp;**SQL**&emsp;&emsp;&emsp;|&emsp;**MatLab** &emsp;&emsp;&emsp;&emsp; |&emsp;**Time Series Analysis**&emsp;|&emsp;**Data Manipulation** <br/>
|&emsp;**NetLogo**&emsp;|&emsp;**MSSQL Server**&emsp;|&emsp;**Probability Statistics**&emsp;|&emsp;**Data Cleaning** <br/>

# INTERNSHIP

## King Abdullah University of Science and Technology (KAUST) <br/> _Data Scientist_
**_12/2022 - 05/2023_**

Conducted a comprehensive analysis of a raster-based dataset encompassing spatio-temporal information on forest fires in the Amazon from 2001 to 2020. <br/>
Utilized **R** and key packages such as ***terra***, ***raster***, and ***h2o*** for data processing, exploratory data analysis, and ensemble modeling.

**Key Contributions:** 
- **Exploratory Data Analysis:** Conducted exploratory analysis on a high-resolution dataset (500m) with ten variables, capturing factors related to fires, land use, environment, and climate. <br/> 
- **Class Imbalance and Missing Data:** Addressed class imbalance and missing data challenges, significantly improving model performance. <br/>
- **Data Downsampling:** Implemented a down-sampling approach, reducing the dataset to 550 million observations, and dividing it into 11 zones for improved efficiency.<br/>
- **Machine Learning Models:** Developed and evaluated machine learning models such as : <br/>
&emsp;◆ Distributed Random Forest (**DRF**)&emsp;&emsp;◆ Generalized Linear Models (**GLM**) <br/>
&emsp;◆ Gradient Boosting Machines (**GBM**)&emsp;◆ eXtreme Gradient Boosting (**XGB**). <br/>
- **Ensemble Modeling:** Created an ensemble model by combining the strengths of individual models within each zone, enhancing predictive accuracy, leveraging **AUC** and **AUCPR** metrics. <br/>
- **Visualization:** Visualized the results through dynamic monthly maps and time trend charts, providing insights into fire probabilities in the Amazon over the 20-year period. 

**Tools:** Executed the project using **R** and employed various packages, including ***terra***, ***raster***, ***h2o***, ***rsample***, ***recipes***, ***data.table***, ***tidyverse***, ***pROC***, ***doParallel***, ***doSNOW***, ***ggplot2***, ***tidyterra***.

# PROJECTS

## Electricity Consumption Forecasting <br/>_(Time Series Analysis)_

Developed predictive models for daily “electricity consumption” in a building based on 47 days of historical data. The dataset included “outdoor air temperature”, influencing two distinct approaches:

- **Temperature-Agnostic Model:** Utilized **HoltWinters**, **Auto ARIMA**, **SARIMA**, and **NNET** to forecast electricity consumption, disregarding outdoor temperature. Model selection based on RMSE.<br/>
- **Temperature-Informed Model:** Incorporated the impact of “outdoor air temperature” using time series regression models (**SARIMA**, **Auto ARIMA**, **NNET**, **VAR**). Selected the best-performing model through RMSE evaluation.

**Tools:** Implemented in **R** using ***forecast***, ***keras***, ***vars***, ***xts***, ***ggplot2***, ***openxlsx*** packages.

**Outcome:** Applied selected models to forecast “electricity consumption” using the entire dataset, showcasing the impact of temperature information on predictive accuracy

> **NOTE:** For more details GitHub [*link*](https://github.com/abid-mohamed/DSTI-Time_Series_Analysis)

## Covariate Impact Analysis and Variable Selection <br/> _(Machine Learning)_

The objective of this project was to assess the influence of covariate variables on a continuous response variable within two distinct datasets.

**Datasets:**
- Data1: <br/>
  - Comprises 12 observations of the response variable and 2 categorical covariates.<br/>
  - Variable Selection Methods: **ANOVA**, **Step-wise Forward**, **Step-wise Backward**, **Lasso**.<br/>
  - Applied **lm** function to determine weights for selected variables.<br/>
- Data2:<br/>
  - Consists of 16 observations of the response variable and 4 continuous covariates.<br/>
  - Mitigated small dataset issues using **Bagging** to reduce variance error.<br/>
  - Variable Selection Methods: **Adjusted R-squared**, **Step-wise Forward**, **Step-wise Backward**, **Lasso**, Variable Selection Using Random Forests (**VSURF**).<br/>
  - Calculated associated errors for each selection method.<br/>
  - Identified the **best model by averaging coefficients** from the lowest error procedures.

**Tools:** Executed the project using **R** and employed various packages, including ***glmnet***, ***MASS***, ***leaps***, ***VSURF***, ***ggplot2***, ***ggpubr***, and ***dplyr***.

**Outcome:** The project resulted in a comprehensive understanding of covariate impacts through rigorous variable selection methods. The utilization of diverse techniques showcased my proficiency in statistical modeling and data analysis using the **R** programming language.

## Database Synchronization using Python and *pyodbc* <br/> _Data Wrangling with SQL_

This project involves creating a **Python** script to interact with a database server and retrieve the latest version of a specified table. 
The script uses the ***pyodbc*** package for secure connections to an **MSSQL Server** and communicates with the database by executing queries.

**Key Steps:**
- ***pyodbc* Connection:** Establishes a secure connection to the database server using the ***pyodbc*** package.
- **Query Execution:** Communicates with the database by sending and executing queries to extract the necessary data.
- **Local Comparison:** Compares the database table with the last saved version on the hard drive to detect any changes.
- **Dynamic View Update:** Generates an updated table view only if modifications are identified during the comparison.

This project streamlines the process of keeping a local copy of a specific database table current, enhancing efficiency in data retrieval and utilization.

## Data Retrieval from MSSQL Server <br/> _Data Wrangling with SQL_

This project focuses on extracting five types of information from a large **MSSQL Server** database through well-designed SQL queries. 

**Key Features:**
- **Data Extraction Goals:** The project aims to obtain five distinct types of information from the extensive MSSQL Server database.
- **Query Techniques:** Standard **SQL** Queries, **Division SQL** Queries, and **Dynamic SQL** Queries with **T-SQL stored procedure**.

## Photon Propagation Simulation <br/> _Agent Base Modeling_

Developed a simulation model to study photon behavior in a water tank and assess the influence of water characteristics on energy propagation.

**Simulation Features:**
  - Implemented a light source emitting photons with random directions, simulating barrier hits, surface reflections, and particle collisions.
  - Explored four water types (“Pure-Sea”, “Clear-Ocean”, “Coastal”, and “Turbid-Harbor”) with distinct absorption and scattering coefficients.

**User Interface:** 
  - Designed an intuitive interface for water type selection, photon count adjustment, and photo-detector positioning.
  - Real-time visualization provided immediate insights into photon behavior and total received energy.

**Parameter Exploration:** Enabled experimentation through sliders for adjusting parameters like beamwidth and photo-detector position.

**Tools:** Implemented using NetLogo programming language for an interactive and accessible user experience.
