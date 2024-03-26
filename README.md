# pandas-challenge
In this week's challenge, I am to analyze a district-wide standardize test results and help the mayor and school board make strategic decisions regarding future school budgets and priorities. 

To do do this, two csv files, schools_complete.csv and students_complete.csv, are stored in variables and merged to give a complete break down of important information including of every students' name, their grades in math and reading, what school they attend, and whether that school is a district or charter school.

Given these various information, I'm tasked with showcasing obvious trends in school performance.

## Going about the Challenge
This challenge relied heavily on turning data series into data frames and merging in various series into said frame. Furthermore, the data was manipulated to calculate various averages such as average grades per school and average passing rates per school. By generating and displaying new data frames with the calculated results, you begin to see trends such as Charter schools outperforming District schools or district schools having a relatively low percentage of students passing both math and reading.

After reviewing the data, I am then tasked with providing an analysis the provides two conclusions that can be drawn from the data.


## In Closing 
There wasn't many challenges within this assignment. The bulk of it could be solved looking at sample code provided within the assignement along with trial and error using codes practiced in class. That said, I did run into one error that I wasn't sure how the assignment intended for us to overcome.
given then sample code: 
##Minor data wrangling
reading_scores_by_grade = reading_scores_by_grade[["9th", "10th", "11th", "12th"]]

I assumed we were to prepare a data frame, named reading_scores_by_grade that did not have properly named columns initially, but would be formatted to have the correct ones with the above code. I tried preparing the data frame but ran into a the error message: 
mergeError: Passing 'suffixes' which cause duplicate columns {'reading_score_x'} is not allowed.

assumming the assignment had a predetermined way for us to go about it, I just could not see the approach. I found that relabeling my series before passing them to a merge function worked like a charm so that was the method I used. This made the renaming code a bit redundant, but I left it in.