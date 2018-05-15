#TidyTuesday 5-15-18

5-14-18

STAR WARS!!! I loaded the data into a tibble to get a look at it. Looks like there are two rows that are headers. I renamed the columns & removed the "first" row (aka the second header row). One question asked for a ranking of all 6 movies. I renamed the columns based on the rating. "Rating_6" is the highest, "Rating_1" is the lowest. Another question asked for a response to a specific characters. I renamed the columns with the character's name. Unfortunately, I couldn't figure out how to do this without renaming them all indiviudally. <br />

First I looked at was how many people rated each movie as the best. I grouped it by gender to see if there was a difference between males & females. <br />
Code - fave.movie.gender.Rmd <br />
Graphic - fave.movie.gender.png <br />

Next I did a dot plot of character ratings. I'm a little obsessed with dot plots lately. I used a count of each rating for character. I also did the same plot broken down by gender. <br />
Code - char.rating.Rmd <br />
Graphic - char.rating.2.png <br />
Graphic - char.rating.gender.png <br />

I'm looking forward to doing more with this data. 

Raw data - https://github.com/fivethirtyeight/data/blob/master/star-wars-survey/StarWars.csv <br />
Article - https://fivethirtyeight.com/features/americas-favorite-star-wars-movies-and-least-favorite-characters/ <br />
Data Source - https://github.com/rudeboybert/fivethirtyeight<br />
