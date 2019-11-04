# DATA-ANALYSIS-ON-SPEED-DATASET
Perform analysis of a dataset containing vehicle speed information

Dataset columns are: 
latitude, longitude,timestamp, speed, speedLimit, functionalClass (a description of the road type), controlledAccess (if yes, this is a controlled-access road, like a highway), isHighway (a different kind of road classification scheme), state (the state in which we put this road), vehicle_id, vehicle_type, driver_id (if null: missing ID)

1.  Read the data. Find out number of rows(records) and columns(attributes).
2.  Glancing at the data and analysing whether numerical or categorical data
3.  Finding maximun and minimum values in each numerical attribute to analyse Range.
4.  DESCRIPTIVE ANALYSIS of Dataset.
    It represents mean, std deviations, quantiles,min and max values.
5.  Finding the number of NULL VALUES in each attribute 
    These null values might sometimes influence while training model. If so, such records need to be dropped or null values have to be         replaced appropriately.
6.  Unique values in 'IsHighway', 'FunctionalClass', 'State' are extracted.
    State is a Categorical Data. Its unique values with count are extracted.
    PIE CHART is used to visulise the percentage of each unique value presnt in State attribute.
7.  DATA CONVERSION:Longitude Values are negative. Converted to positive.
    Because it decreases the Euclidean distance in a dimensional feature space wrt to other attributes.
8.  DATA CONVERSION: Categorical data is converted to Numerical data.
    Because categorical data cannot be evaluted while training model.
9.  Finding the number of OUTLIERS by IQR METHOD.
    Outliers impact(during summations, mean etc) the model training sometimes. Hence in such cases, they need to be dropped.
10. Box plots for numerical data attributes.
    They help to visualise symmetry and data spread and also max, min values, range, outliers.
11. HISTOGRAM PLOTS.
    They provide a visual representation of data distribution. They display a large amount of data and the frequency of the data values.       The median and distribution of the data can be determined by a histogram. It also shows any outliers or gaps in the data.
12. PEARSON CORRELATION
    Pearson's correlation coefficient is a number between -1 and 1.It measures the statistical relationship, or association, between two       continuous variables.If two variables are highly correlated, one of them can be dropped since their contribution in model training is
    almost same.
13. INDEXING : An appropriate attribute can be considered as index value for each record.
14. AVERAGE SPEED OF DRIVER : can be found by group-by driver_id and finding the mean for each driver_id.This can be used to analyse the 
    driver's driving and the speed that he maintains on an average.
15. AVERAGE SPEED OF VEHICLE : can be found by group-by vehicle_id and finding the mean for each vehicle_id. Average speed of vehicle
    can be analysed.
16. SCATTER PLOTS: for 'LATITUDE vs SPEEDLIMIT ' and 'LONGITUDE vs SPEEDLIMIT' is plotted.
    They reprsent the scattering of data in 2-dimensional feature space.
    
#### (.ipynb file is attached that contains codes and results for the above)
