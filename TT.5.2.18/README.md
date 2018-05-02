#TidyTuesday 5-2-18

5-1-18

The first plot is a break down of gender & race as percentages for all counties in Illinois. I used Illinois because I live here. The weird thing about this data is that the race values are percentages but the gender values are total number of people. The percentage for genders had to be calculated. I added an extra variable to the data frame to use facet_wrap & break down by gender & race. Not my favorite graphic. Looked exactly as expected.<br />
Code - IL.pop.Rmd<br />
Plot - IL.pop.png<br />

5-2-18

The second plot is the percentage of each race of the top 10 states by population (Population Data Source below). This required calulating the number of people in each race for each county in the states. The percentage was then calculated based on the total population of the state. The size of the point is the precentage. I also labeled them just for clarity. <br />

After I did this plot, I realized I could've used the total population from the data to determine my top 10. Silly mistake on my part! <br />
Population Data Source - https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_population <br />
Code - top10.pop.Rmd<br />
Plot - top10.pop.png<br />

I redid the Illinois plot with the New Jersey data. I wanted to see what it would look like with fewer counties. New Jersey was selected based on the number of counties.<br />
Code - NJ.pop.Rmd<br />
Plot - NJ.pop.png<br />

I decided I didn't like any of the previous plots. They just weren't interesting. I made a new plot that compares the average income of counties and the percent of poverty. I used the top 10 states by population. I made a data frame with the top 10 states by population. I made two separate data frames: one for income & one for poverty. I filtered them using the data fram with the top 10 states. Then I joined the income & poverty data frames. <br />
Code - top10.income.poverty.Rmd<br />
Plot - top10.income.poverty.png<br />

I did the same plot with the bottom 10 states by population.<br />
Code - bottom10.income.poverty.Rmd<br />
Plot - bottom10.income.poverty.png<br />

Data - https://github.com/rfordatascience/tidytuesday/blob/master/data/acs2015_county_data.csv <br />
Data source - https://factfinder.census.gov/faces/nav/jsf/pages/index.xhtml <br />
Kaggle source - https://www.kaggle.com/muonneutrino/us-census-demographic-data <br />
