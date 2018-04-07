#TidyTuesday 4-3-18

4-6-18

This data is the average tuition (USD) broken down by state & year. 

Hardest part of this was stripping the "$" and "," from the tuition values. I didn't use as much tidyverse for the data manipulation as I would've liked.

I'm a big fan of heat maps for investigating trends. The heat map allows you to see the trends across each state but then also compare them to the overall cost. I like the blue to red color palette for heat maps. heatmap.Rmd is the code. heatmap.avg.tuition.pdf is the visualization.

I might revisit this data again. I have a couple ideas for uses of facet_wrap & better color schemes.

4-7-18

I created multiple scatter plots grouped by year. Not super readable but the color scheme shows the trend nicely. 50 y axis labels makes the fint size a bit of a challenge. I made the pdf larger than the default to increase readability. scatter.facet.Rmd is the code. scatter.facet.pdf is the visualization.  
