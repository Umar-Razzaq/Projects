# Data Analysis with Pandas

## Part 1: Olympics Data
The following code loads the olympics dataset (olympics.csv), which was derrived from the Wikipedia entry on [All Time Olympic Games Medals](https://en.wikipedia.org/wiki/All-time_Olympic_Games_medal_table), and does some basic data cleaning. 

The columns are organized as # of Summer games, Summer medals, # of Winter games, Winter medals, total # number of games, total # of medals. 

In part 1, I will use this dataset to answer the questions below:

- What is the first country in df?
- Which country has won the most gold medals in summer games?
- Which country had the biggest difference between their summer and winter gold medal counts?
- Which country has the biggest difference between their summer gold medal counts and winter gold medal counts relative to their total gold medal count?
- What are the total points for each country?


## Part 2: Census Data
Will be using census data from the [United States Census Bureau](http://www.census.gov/popest/data/counties/totals/2015/CO-EST2015-alldata.html). Counties are political and geographic subdivisions of states in the United States. This dataset contains population data for counties and states in the US from 2010 to 2015. [See this document](http://www.census.gov/popest/data/counties/totals/2015/files/CO-EST2015-alldata.pdf) for a description of the variable names.

The census dataset (census.csv) should be loaded as census_df. Answer questions using this as appropriate.

In part 2, I will use pandas to answer the following question:
- Which state has the most counties in it?
- What are the three most populous states?
- Which county has had the largest absolute change in population within the period 2010-2015?
- Find counties with specific properties.