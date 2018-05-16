#TidyTuesday 5-15-18

5-14-18

STAR WARS!!! I loaded the data into a tibble to get a look at it. Looks like there are two rows that are headers. I renamed the columns & removed the "first" row (aka the second header row). One question asked for a ranking of all 6 movies. I renamed the columns based on the rating. "Rating_6" is the highest, "Rating_1" is the lowest. Another question asked for a response to a specific characters. I renamed the columns with the character's name. Unfortunately, I couldn't figure out how to do this without renaming them all indiviudally. I dropped all NAs. <br />

First I looked at was how many people rated each movie as the best. I grouped it by gender to see if there was a difference between males & females. <br />
Code - fave.movie.gender.Rmd <br />
Graphic - fave.movie.gender.png <br />

Next I did a dot plot of character ratings. I'm a little obsessed with dot plots lately. I used a count of each rating for character. I also did the same plot broken down by gender. <br />
Code - char.rating.Rmd <br />
Graphic - char.rating.2.png <br />
Graphic - char.rating.gender.png <br />

I'm looking forward to doing more with this data. 

5-15-18

I just have too many ideas! My newest idea was to do a choropleth filling in the state by color based on the favorite movie. The location in this data is broken down by region. I couldn't find a pacakage with the US map by regions. I made a separate file that lists the state in the first column & the region in the second column. I got the data to make that file here: https://simple.wikipedia.org/wiki/List_of_regions_of_the_United_States. Final state/region file is state.region.csv. I dropped all NAs. The choropleth shows favorite movie by state & least favorite movie by state. Not my fave graphic but interesting!<br />
Code - location.fave.Rmd <br />
Graphic - Location.fave.png <br />

Next I changed it up & did a different choropleth for favorite movie by state. I used age to create 4 different choropleths.  I was lazy & let R break the ties for me. <br />
Code - location.age.fave.Rmd <br />
Graphic - location.age.fave.png <br />

Next I did a plot of the favorability rating of Darth Vader broken down by age. I originally wanted to do a plot of all the bad guys but there weren't that many in the survey. Instead I just used the Darth Vader data. I used an image as the background. Pretty easy with the ggpubr package! Link to the picture: http://getdrawings.com/vinyl-drawing. I played with the color in Preview to lighten the picture up. I used gray scale cuz I figured it went well with the Darth Vader theme. <br />
Code - bad.guy.Rmd <br />
Graphic - bad.guy.png <br />

Raw data - https://github.com/fivethirtyeight/data/blob/master/star-wars-survey/StarWars.csv <br />
Article - https://fivethirtyeight.com/features/americas-favorite-star-wars-movies-and-least-favorite-characters/ <br />
Data Source - https://github.com/rudeboybert/fivethirtyeight<br />
