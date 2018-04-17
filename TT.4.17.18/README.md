#TidyTuesday 4-17-18

4-16-18

I started with a basic plot with all the data. Massive amount of data but I kept the plot because I thought it looked neat. Overall, not a very informative plot. The labels on the y-axis are difficult to read but I didn't want to spend time playing with them because I wanted to move on to other plots. This exercise was mostly to give me a general idea of what I was working with data wise. Code - all.data.RMD Plot - all.data.png

I moved on to trying to recreate the original graphic. I did a pretty good job. Major differences between my plot and the original graphic are the colors & the labels. Some of the labels in the original graphic are '>0.01', which I didn't want to mess with. I used this plot to try to remember how to use RColorBrewer palettes with ggplot2. Code - US.2016.Rmd Plot - US.2016.png

Instead of recreating the Kenya plot. I focused on Guatemala. Same as before, different colors & slightly different labels. Code - Guat.2016.Rmd Plot - Guat.2016.png

I wanted to do my own original graphic. I used Guatemala again. This time I focused on the trends in each disease in the specified time frame. I filtered the diseases, using only those with an average percent higher than 1.5%. This was a random cut off value that I chose mostly because it gave me an even number of plots. I really like this graphic. I think it looks really good! Code - Guat.all.Rmd Plot - Guat.all.png

Source:
Data - https://github.com/rfordatascience/tidytuesday/blob/master/README.md <br />
Article - https://ourworldindata.org/what-does-the-world-die-from <br />
Blog - https://thomasmock.netlify.com/post/tidytuesday-a-weekly-social-data-project-in-r/ <br />
