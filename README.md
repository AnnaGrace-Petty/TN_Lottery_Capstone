# TN Lottery Capstone

## Table of Contents
* [Motivation](#motivation)
* [Data Questions](#data-questions)
* [Data Sources and Tools](#data-sources-and-tools)
* [Process](#process)
* [Link to Dashboard Presentation](#link-to-dashboard-presentation)

## Motivation
As a kid my parents always bought my siblings and I scratch off tickets. I have passed the lottery billboards all my life. The lottery has always been something that was around, but it was never something I understood. I personally have never been big on taking chances when it comes to money because most of my life the only money I personally had came from saving up my allowance and holiday money. But after the largest Powerball jackpot in history was won on November 7th of this past year, I had some questions. And while I have been attending the wonderful Nashville software school, I have learned ways to answer some of my questions.

When I first started this project, I planned on focusing on drawing style games such as the Powerball because of the record setting jackpot. But as I dove into the data, I realized that instant games or scratch offs as a lot of people call them are a big part of the lottery. With some instant games you don’t have to pay a lot of money for a chance to win big.

## Data Questions
1.	What stores have sold winning tickets in Tennessee?
2.	What are the poverty rates for the locations of winning tickets?
3.	What is the median amount of winnings people receive for each game?
4.	What instant games are the ones to take a chance on?

## Data Sources and Tools
### Data Sources
* https://tnlottery.com/
* https://data.census.gov/
### Technology Tools
#### - Python
* Jupyter Notebook
* Pandas
* Cloudscraper
* BeautifulSoup
#### - Tableau
#### - Excel

## Process
### Getting the Data
The poverty data for Tennessee counties was very easy to get. I just went to https://data.census.gov/ and filtered the website for it to give me options of charts I could use. I pick a chart and imported it to Python to get cleaned.

The Tennessee Lottery data was another story. I had a few days of not knowing if I was going to be able to find a Python library that I would be able to use to web-scrap. After some help from my teachers at Nashville Software School I was able to web-scrap the website. Once I imported the cloudscaper library I was able to pull all the data I would need within 20 minutes. I was very glad to have been able to find all the data I needed that fast for the fact I felt i had spent too much time on getting the data but everything worked out just fine.
### Cleaning Data
The first data I cleaned was the poverty data because it was the easiest to get done while I was still researching libraries I could use to web-scrap the lottery website. The poverty data came in the form of a chart so I had to remove the columns and rows I did not need. I changed the name of the column names to just the name of the county instead of county, state format since I was only looking in the state of Tennessee. I then used ".melt" so that all my county name would become one row instead of them being column names. I then divided the amount of people in poverty by the population for each county then multiplied by hundred which gave me poverty percentage.

When it came time to clean the lottery data I believed it was going to be really easy, oh was I wrong. This project has taught me that no matter how clean the data looks when you pull it in there is always something to be cleaned and fixed. First thing I wanted to find was the location of where a winning ticket was bought. I did figure that out but I soon found out only about 55 people had a location on the website. So it made me have to come of with more things to look for which was fun and hard. I started realizing instant games had way more winners than drawing style games so I went for it by separating the data into different charts so I could easily put it graphic charts in Tableau. I then went to clean the price of instant game charts so we could compare cost to play vs. median winnings. I noticed game names were typed different of the instant game page and the winners page so I had to change both pages font to all uppercase letters. A major of the text were exactly the same so I was able to merge the charts and then work on the games that were not merge. I quickly found out a lot of the games that weren't merge were actually games I had not data for the cost to play chart. These games were not on the cost to play chart because they were game no longer be played which was a nice thig to find out because I believed I messed my data up. Lucky everything got cleaned and ready so I could put it tableau and make a presentation to present.
### Creating Presentation
Once I pulled all the charts into Tableau it was easy. I love Tableau but I admit it can be a little difficult at time for me to get tableau to do what I want to do. I first based my color palette on the Tennessee Lottery color palette then when I need more colors I just added ones to compliment. I first made all my charts that I wanted to be presented. I then added buttons to dashboards for views to explore more on their own. I added links for views to go visit some websites relating to the project. Lastly I changed the place holder cover page and "thank you" slide to slides that are more my style, I especially love the "thank you" slide.

# Link to Dashboard Presentation
https://public.tableau.com/views/TNLotteryCapstone/Story1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link
