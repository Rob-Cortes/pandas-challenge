# pandas-challenge

In this exercise, we create and manipulate Pandas DataFrames to analyze school and standardized test data.

## Set-Up
After importing Pandas, we store the school data in the form of a Pandas DataFrame. The raw data is found in CSV format in the 'Resources' folder.

## District Summary
In this section, we create a high-level snapshot of the district's key metrics, including:

Total number of unique schools
Total students
Total budget
Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

## School Summary
In this section, we summarize school performance with the following information:

School name
School type
Total students
Total school budget
Per student budget
Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

We identify the highest-performing schools by sorting the schools according to % Overall Passing and displaying the top 5 rows. These results are saved in a DataFrame called "top_schools". We repeat this process for the worst-performing schools. 

Next, we create DataFrames that list the average math and reading scores for students of each grade level (9th, 10th, 11th, 12th) at each school.

## Performance Metrics vs. School Spending, Size, and Type
To assess performance across different school metrics, we make use of pd.cut().

First, we create a table that breaks down school performance based on average spending ranges (per student). We use pd.cut to categorize spending in terms of ranges (aka bins). Now that we have spending bins, we create a DataFrame with test scores and passing rates for each bin. 

![image](https://github.com/Rob-Cortes/pandas-challenge/assets/124944383/e2425663-496f-4f30-ab64-76d9b440aca0)

This process is repeated for school size (i.e., number of students).

![image](https://github.com/Rob-Cortes/pandas-challenge/assets/124944383/eb0f7dbe-5c37-4f5b-baed-f45eff9d32f4)

Lastly, we creete a final DataFrame that shows school performance based on the type of school (charter or district). This DataFrame does not require the use of pd.cut(). 

![image](https://github.com/Rob-Cortes/pandas-challenge/assets/124944383/85fed634-3a34-41f4-9ed3-e041fe9ce807)

