# An Analysis of Political Contributions During the 2020 House of Representatives Election

In this part, you will obtain as much data as you can on the campaign contributions received by each candidate. This data is avaiable through the website https://www.opensecrets.org/.

### Part 1: Data Gathering
1. Start by scraping the data from the summary page for Tennessee's 7th District, which is available at https://www.opensecrets.org/races/candidates?cycle=2020&id=TN07&spec=N.
    * Make a DataFrame showing, for each candidate:
        * the candidate's name
        * the candidate's party
        * state
        * district number
        * whether the candidate was an incumbent
        * whether the candidate won the race
        * the percentage of the vote that candidate received
        * the total amount raised by that candidate (as a numeric variable)
        * the total amount spent by the candidate (as a numeric variable)
2. Once you have working code for Tennessee's 7th District, expand on your code to capture all of Tennessee's districts.
3. Once you have working code for all of Tennessee's districts, expand on it to capture all states and districts. The number of representatives each state has can be found in a table on this page: https://www.britannica.com/topic/United-States-House-of-Representatives-Seats-by-State-1787120

### Part 2: Exploratory Data Analysis
Using your scraped data, investigates different relationships between candidates and the amount of money they raised. Here are some suggestions to get you started, but feel free to pose you own questions or do additional exploration:  
    a. How often does the candidate who raised more money win a race?  
    b. How often does the candidate who spent more money win a race?  
    c. Does the difference between either money raised or money spent seem to influence the likelihood of a candidate winning a race?  
    d. How often does the incumbent candidate win a race?  
    e. Can you detect any relationship between amount of money raised and the incumbent status of a candidate?

### Part 3: Statistical Modeling
Fit a logistic regression model to see if the amount spent has a statistically significant impact on the probability of winning an election.  
Feel free to brainstorm ways to set up your model, but a suggestion to get started would be to calculate, for each candidate, the percentage of to total amount spent in their race that was spent by them and use this as your predictor variable of interest. Hint: you may find the `transform` method (https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.transform.html) in combination with `groupby` useful to find the total spending by race.  
Don't forget to include the incumbent variable in your model.  
After fitting your model, interpret the meaning of the coefficients you get.  


## Deliverable

Prepare a 10-12 minute presentation of your findings. This presentation should focus on the exploratory analysis and statistical modeling portions of this project and not on the webscraping components. Thus, you should not include any code in your presenation. Your presentation should be done using PowerPoint/Google Slides or other presentation software.

Presentations will take place on Saturday, 10/21 at noon.