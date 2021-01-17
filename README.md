# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
1. Get a complete list of candidates who received votes.
1. Calculate the total number of votes each candidate received.
1. Calculate the percentage of votes each candidate won.
1. Determine the winner of the election based on popular vote.

## Resources
* Data Source: election_results.csv
* Software: Python 3.7.6, Visual Studio Code, 1.52.1

## Summary
The analysis of the election show that: 
* There were 369,711 votes cast in the election.
* The candidates were:
  * Charles Casper Stockham
  * Diana DeGette
  * Raymon Anthony Doane
The candidate resulsts were:
  * Charles Casper Stockham received 23.0% of the vote and 85,213 total votes.
  * Diana DeGette received 73.8% of the vote and 272,892 number of votes.  
  * Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
The winner of the election was:
  * Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.
  
## Challenge Overview

We were asked to audit the results of the Colorado election to verify the election results. In order to verify the results, we were asked to calculate the following:

  1. The voter turnout for each county
  1. The percentage of votes from each county out of the total count
  1. The county with the highest turnout
  1. The total number of votes
  1. Each candidate's total votes and percentages of votes
  1. The winner of the election, winning vote count, and winning percentage of votes.

We were provided with a CSV file and asked to create a Python scrip that would read through this document and calculate the above. Once the Python scrip calculated the above numbers, we were asked to have the Python scrip to also write those numbers into a text file.

## Challenge Summary

Overview of Election Audit: Explain the purpose of this election audit analysis.

# Election-Audit Results: Using a bulleted list, address the following election outcomes. Use images or examples of your code as support where necessary.

  1. How many votes were cast in this congressional election? 
  * 369,711 votes were cast in this congressional election.

  2. Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.

![alt text](https://github.com/Anthony-Hendrickson/Election_Analysis/blob/main/Resources/Votes_and_percentages_by_county.PNG)

  3. Which county had the largest number of votes?
  * Denver county had the largest number of votes with a total of 306,055


  4. Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

![alt text](https://github.com/Anthony-Hendrickson/Election_Analysis/blob/main/Resources/Votes_and_percentages_by_candidate.PNG)

  5. Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
  * Diane DeGette won the election with 272,892 votes, which translated to 73.8% of the total votes.
    
# Election-Audit Summary:

The script is very versitile. It could be used for congressional elections in other districts quite easily.

If you had another csv election file from another state with a similar structure it would be as easy changing the numeric values in "candidate_name" and "county_name" assignment statements in order to correctly identify the position of the column that contains the relevant values. See a screenshot of these assignment statements below:

![alt text](https://github.com/Anthony-Hendrickson/Election_Analysis/blob/main/Resources/Targeting_county_and_candidate_values_in_csv.PNG)

If the structure of the CSV was identical you wouldn't need to change the script at all. 

This script could also be repurposed for national elections. Renaming some of the lists and variables within the scrip as well as some of the printed statements could make this count results by state instead of by county. You may also need to follow the change in the numeric values within assignment statements pointed out above. Renaming the variables in some of the assignment statements/lists would make the script legible. See below for an example where "county_name" and "county_votes" would become "state_name" and "state_votes":

![alt text](https://github.com/Anthony-Hendrickson/Election_Analysis/blob/main/Resources/county_to_state_repurpose.PNG)

Most importantly, you would need to change the text in the print statements would achieve the same output for states as opposed to counties. See the screenshot below which produces the "Largest County" print statement now. It would be as simple as changing the text values in the f-string from "Largest county turnout:" to "Largest state turnout." See this statement in its current form below:

![alt text](https://github.com/Anthony-Hendrickson/Election_Analysis/blob/main/Resources/county_to_state_repurpose_outputs.PNG)

As we can see, this script is very versitile and could be very useful for election auditing purposes beyond the congressional elections we are measuring now.
