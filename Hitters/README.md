## Salary Prediction Model
### Description

Major League Baseball Data from the 1986 and 1987 seasons.

### Format:

AtBat: Number of times at bat in 1986
Hits: Number of hits in 1986
HmRun: Number of home runs in 1986
Runs: Number of runs in 1986
RBI: Number of runs batted in in 1986
Walks: Number of walks in 1986
Years: Number of years in the major leagues
CAtBat: Number of times at bat during his career
CHits: Number of hits during his career
CHmRun: Number of home runs during his career
CRuns: Number of runs during his career
CRBI: Number of runs batted in during his career
CWalks: Number of walks during his career
League: A factor with levels A and N indicating player's league at the end of 1986
Division: A factor with levels E and W indicating player's division at the end of 1986
PutOuts: Number of put outs in 1986
Assists: Number of assists in 1986
Errors: Number of errors in 1986
Salary: 1987 annual salary on opening day in thousands of dollars
NewLeague: A factor with levels A and N indicating player's league at the beginning of 1987

### Needed python libraries:
Pandas, matplotlib, seaborn, filterwarnings, missingno, numpy, sklearn, statsmodels, re, lightgbm.

### Processes:
1. Data understanding
2. Data preprocessing
3. Cleaning outliers
4. Creating different scenarios
5. Apply regression algorithms to all scenarios
6. Model tuning

### Scenarios:
1. Dropping NULL values, min-max sclae numeric columns, encode object columns with label 
and one hot encoder depending on unique values in these colums.

2.Filling NULL values with mean, based on categories. 

3.Min-max scale numeric colums, encode object columns, filling NULL values with KNN imputer adding new_year column.

4.Filling Missing Data with KNN and Suppressing Outliers to create 'df4' and cleaning outliers with LOF(Local Outlier Factor).

5.Creating new variables and filling NULL values with knn imputer. New variables were created with the most appropriate variables according 
to their proportions. The data set includes the data obtained by the players in 1986 and throughout their 
careers and how many years of experience they have. The annual averages of these data and the ratio of the 1986 
data to the overall performance were added.
