# pandas-challenge
given access to every student's math and reading scores, as well as various information on the schools they attend. I'm tasked with aggregating the data to showcase obvious trends in school performance.

## Challenges
given then sample code: 
# Minor data wrangling
reading_scores_by_grade = reading_scores_by_grade[["9th", "10th", "11th", "12th"]]

I assumed we were to prepare a data frame, named reading_scores_by_grade that did not have properly named columns initially, but would be formatted to have the correct ones with the above code. I tried preparing the data frame but ran into a the error message: 
mergeError: Passing 'suffixes' which cause duplicate columns {'reading_score_x'} is not allowed.

assumming the assignment had a predetermined way for us to go about it, I just could not see the approach. I found that relabeling my series before passing them to a merge function worked like a charm so that was the method I used. This made the renaming code a bit redundant, but I left it in.