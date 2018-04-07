#TidyTuesday 4-13-18

This data is the average tuition (USD) broken down by state & year. 

Hardest part of this was stripping the "$" and "," from the tuition values. I didn't use as much tidyverse for the data manipulation as I would've liked.

I'm a big fan of heat maps for investigating trends. The heat map allows you to see the trends across each state but then also compare them to the overall cost. I like the blue to red color palette for heat maps. heatmap.Rmd is the code. heatmap.avg.tuition.pdf is the visualization.

I might revisit this data again. I have a couple ideas for uses of facet_wrap & better color schemes.
