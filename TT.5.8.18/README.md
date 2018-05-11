#TidyTuesday - 5-8-18

5-8-18

Made my first chloropleth, mostly because I've never done one before. This chloropleth shows the percent of Starbucks in each state. California is an outlier so I also did a version where I adjusted the percent with a log2 transformation. This makes the differences between states more noticeable but the scale with the log2 transformation makes the graphic difficult to understand. <br />

I used the fiftystater library. An interesting point with this library is the states have to be the full name in all lowercase for the graphic to work. I also dropped DC (District of Columbia) from the graphic. <br />
Code - chlorpleth.Rmd<br />
Graphic - pct.Sbux.state.png (percent graphic)<br />
Graphic - pct.Sbux.state.log2.png (log 2 transformation graphic)<br />

The next graphic I did was a pretty simple bar graph showing the percent of each type of ownership for all the Starbucks. Then I did the same thing with time zones. Too many time zones make the graphic hard to understand. In looking at the time zone visual, I realized they are all assigned to a region. For the next graphic, I split the time zone column to get the region. Then I calculated the percent of stores in each region.<br />
Code - 2.Rmd <br />
Graphic - own.type.png <br />
Graphic - timezone.png <br />
Graphic - region.png <br />

Data - https://github.com/rfordatascience/tidytuesday/blob/master/data/week6_coffee_chains.xlsx <br />
Article - http://flowingdata.com/2014/03/18/coffee-place-geography/ <br />


