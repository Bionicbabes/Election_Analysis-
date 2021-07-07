# Election_Analysis-

## Project Overview 
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election,  

* The voter turnout for each county
* The percentage of votes from each county out of the total count
* The county with the highest turnout

## Resources 
- Data Source: election_results.csv
- Software: Python 3.9.6 64 bit Visual Studio Code 1.57.1

## Election-Audit Results: 
* How many votes were cast in this congressional election?

Election Results
-------------------------
Total Votes: 369,711
-------------------------

* Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.

County Votes:
-------------------------
Jefferson: 10.5% (38,855)
Denver: 82.8% (306,055)
Arapahoe: 6.7% (24,801)
-------------------------

* Which county had the largest number of votes?
-------------------------
Largest Count Turnout: Denver
-------------------------

* Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
-------------------------
Charles Casper Stockham: 23.0% (85,213)
Diana DeGette: 73.8% (272,892)
Raymon Anthony Doane: 3.1% (11,606)
-------------------------
* Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
-------------------------
Winner: Diana DeGette
Winning Vote Count: 272,892
Winning Percentage: 73.8%
-------------------------

## Election-Audit Summary:
In conclusion this analysis can be used in future election and is not limited to just the 3 key indexes for analysis.  If additional data was provided for future election the code could be modified to look at districts instead of counties by changing the index in this line of code and futhur analysis could be run by changing the associated variable names to keep the code organized. 
        # Get the candidate name from each row.
        candidate_name = row[2]

        # 3: Extract the county name from each row.

        county_name = row[1]
Furthermore is you would like to change the way the winner is determined the code could be modified to your needs by looking more deeply into this code, this code looks at the popular vote in each county.  If we were to get the presidential race we could use this code as a template and also include electoral college votes to the analysis to help predict the winner.
   if (number_of_county_votes > winning_county_count) and (county_vote_percentage > winning_percentage):
            # If true then set winning_count = votes and winning_percent =
            # vote_percentage.
            winning_county_count = number_of_county_votes
            county_winning_percentage = county_vote_percentage
            # And, set the winning_candidate equal to the candidate's name.
            winning_county_name = county_name
