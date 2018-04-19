#TidyTuesday 4-17-18

4-16-18

I started with a basic plot with all the data. Massive amount of data but I kept the plot because I thought it looked neat. Overall, not a very informative plot. The labels on the y-axis are difficult to read but I didn't want to spend time playing with them because I wanted to move on to other plots. This exercise was mostly to give me a general idea of what I was working with data wise. <br />
Code - all.data.RMD <br />
Plot - all.data2.png <br />

I moved on to trying to recreate the original graphic. I did a pretty good job. Major differences between my plot and the original graphic are the colors & the labels. Some of the labels in the original graphic are '>0.01%', which I didn't want to mess with. I used this plot to try to remember how to use RColorBrewer palettes with ggplot2. <br />
Code - US.2016.Rmd <br />
Plot - US.2016.png <br />

Instead of recreating the Kenya plot. I focused on Guatemala. I'm half Guatemalan so this seemed like a good choice! Same as before, different colors & slightly different labels. <br />
Code - Guat.2016.Rmd <br />
Plot - Guat.2016.png <br />

I wanted to do my own original graphic. I used Guatemala again. This time I focused on the trends in each disease in the specified time frame. I filtered the diseases, using only those with an average percent higher than 1.5%. This was a random cut off value that I chose mostly because it gave me an even number of plots. I had a tough time ordering the facets alphabetically. I finally ended up reordering the columns in the original tibble. Overall, I really like this graphic. I think it looks really good! <br />
Code - Guat.all.Rmd <br />
Plot - Guat.all.png <br />

I started doing all the plots in .png format. I noticed last week that when you navigate to Github through Twitter, you can't view .pdf or .tiff. I start using .png to make it more accessible. 

4-18-18

I got the idea to to a mosaic plot with this data. After playing with the data a bit, I realized that most of the countries percentages don't add up to an even 100%. I end up choosing 7 countries based on population size & how close the total was to 100. I got the populations from https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population. These are all 2017 or 2018 population numbers. Population data can be found in population.csv.

I tried to use ggmosaic for this plot. I worked through the ggmosiac vignette to get an idea how they work. I got an error ```Error in is.finite(x) : default method not implemented for type 'list'```. I was able to solve it by using ```devtools::install_github('cran/ggplot2')```, a solution I found here: https://github.com/haleyjeppson/ggmosaic/issues/9. I ended up not using ggmosaic because I didn't really understand how the data needed to be manipulated correctly.

The majority of this code follows the tutorial here: https://learnr.wordpress.com/2009/03/29/ggplot2_marimekko_mosaic_chart/. Some of the precentages are really small, so drawing a border around each category made the graphic look bad. I finally settled for a line to separate each country using geom_segment. I'm not a fan of the country labels. I played around with them but geom_text wasn't as flexible as I'd like. I'm also don't like how the legend is ordered but that is more due to the color scheme I chose than anything else. Not sure how I feel about the color scheme but this one looked the best out of the different ones I tried.

Overall, this mosaic plot was a lot harder than I thought it would be. I'm spoiled by ggplot being fairly intuitive. This required a lot more manipulation to give ggplot2 the correct parameters. Not a bad graphic for my first mosaic plot. 
Code - mosaic.Rmd <br />
Plot - mosaic.png

Source: <br />
Data - https://github.com/rfordatascience/tidytuesday/blob/master/README.md <br />
Article - https://ourworldindata.org/what-does-the-world-die-from <br />
Blog - https://thomasmock.netlify.com/post/tidytuesday-a-weekly-social-data-project-in-r/ <br />
