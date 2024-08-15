# NBA Workforce Analytics - Final Python Project

## Project Overview
This project focuses on analyzing the dataset of NBA team employees to extract valuable insights. Through data preprocessing, analysis, and visualization, we aim to understand the distribution of employees across teams and positions, identify predominant age groups, determine salary expenditures, and explore the correlation between age and salary.

## Data Preprocessing

### Data Loading
The dataset is loaded directly from a Google Sheets link using the `pd.read_csv()` function from the pandas library.

### Data Correction
The "height" column is corrected by generating random values between 150 and 180 cm using the `np.random.randint()` function from the numpy library, ensuring realistic height data for the analysis.

## Analysis Tasks

### Team Distribution
The distribution of employees across different NBA teams is calculated using `value_counts(normalize=True)` on the "team" column. This analysis provides a percentage breakdown of employees per team.

### Position Distribution
Employee segregation based on positions is achieved using `value_counts()` on the "position" column, helping to understand the composition of the workforce in terms of their playing positions.

### Predominant Age Group
To determine the predominant age group among employees, age bins are created using `pd.cut()` to categorize employees into age groups, followed by `value_counts()` to count occurrences. This analysis reveals the most common age group in the dataset.

### Salary Expenditure Analysis
The highest salary expenditure by team and position is calculated by grouping the data using `groupby()` and summing the salaries. This identifies which team and position have the highest financial investment.

### Correlation Between Age and Salary
The relationship between age and salary is explored using a scatter plot generated with `sns.scatterplot()` from the seaborn library. This visualization helps to identify any correlation between an employee's age and their salary.

## Graphical Representation

- **Bar Charts**: Visualize the distribution of employees across teams and positions.
- **Pie Charts**: Display the proportion of employees in different teams.
- **Histograms**: Show the distribution of age groups among employees.
- **Scatter Plots**: Illustrate the correlation between age and salary.

## Data Story

1. **Distribution of Employees Across Teams**: 
   The analysis reveals that teams like the New Orleans Pelicans, Memphis Grizzlies, and Utah Jazz have the highest proportion of employees, each contributing significantly to the league's workforce.

2. **Segregation of Employees Based on Positions**: 
   Shooting Guards (SG) and Power Forwards (PF) are the most common positions among employees, with 102 and 100 employees, respectively.

3. **Predominant Age Group Among Employees**: 
   The majority of employees fall within the 20-29 age group, highlighting a younger workforce in the NBA.

4. **Salary Expenditure Analysis**: 
   The Cleveland Cavaliers are identified as the team with the highest salary expenditure, particularly investing heavily in the Center (C) position.

5. **Correlation Between Age and Salary**: 
   A slight positive correlation is observed between age and salary, indicating that older employees generally tend to earn higher salaries.


## this is my out put and its analysis:
 Distribution of Employees Across Teams:
## 1 Team
New Orleans Pelicans      4.148472
Memphis Grizzlies         3.930131
Utah Jazz                 3.493450
New York Knicks           3.493450
Milwaukee Bucks           3.493450
Brooklyn Nets             3.275109
Portland Trail Blazers    3.275109
Oklahoma City Thunder     3.275109
Denver Nuggets            3.275109
Washington Wizards        3.275109
Miami Heat                3.275109
Charlotte Hornets         3.275109
Atlanta Hawks             3.275109
San Antonio Spurs         3.275109
Houston Rockets           3.275109
Boston Celtics            3.275109
Indiana Pacers            3.275109
Detroit Pistons           3.275109
Cleveland Cavaliers       3.275109
Chicago Bulls             3.275109
Sacramento Kings          3.275109
Phoenix Suns              3.275109
Los Angeles Lakers        3.275109
Los Angeles Clippers      3.275109
Golden State Warriors     3.275109
Toronto Raptors           3.275109
Philadelphia 76ers        3.275109
Dallas Mavericks          3.275109
Orlando Magic             3.056769
Minnesota Timberwolves    3.056769
Name: proportion, dtype: float64

## 2. Segregation of Employees Based on Positions:
Position
SG    102
PF    100
PG     92
SF     85
C      79
Name: count, dtype: int64

## 3. Predominant Age Group Among Employees: 20-29

## 4. Team with the Highest Salary Expenditure: Cleveland Cavaliers
   Position with the Highest Salary Expenditure: C

## 5. Correlation between Age and Salary:
   There seems to be a slight positive correlation between age and salary, indicating that older employees tend to have higher salaries.
   
## Conclusion
This analysis of NBA team employees provides valuable insights into workforce distribution, salary expenditures, and trends within the league. By understanding these factors, teams can make informed decisions regarding their human resources and financial planning.

