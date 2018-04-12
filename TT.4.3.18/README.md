#TidyTuesday 4-3-18

4-6-18

This data is the average tuition (USD) broken down by state & year. 

Hardest part of this was stripping the "$" and "," from the tuition values. I didn't use as much tidyverse for the data manipulation as I would've liked.

I'm a big fan of heat maps for investigating trends. The heat map allows you to see the trends across each state but then also compare them to the overall cost. I like the blue to red color palette for heat maps. heatmap.Rmd is the code. heatmap.avg.tuition.pdf is the visualization.

I might revisit this data again. I have a couple ideas for uses of facet_wrap & better color schemes.

4-7-18

I created multiple scatter plots (scatter.facet.Rmd) grouped by year. Not super readable but the color scheme shows the trend nicely. 50 y axis labels makes the font size a bit of a challenge. I made the pdf (scatter.facet.pdf) larger than the default to increase readability. 

For a different project, I was looking to make 55 heatmaps using a generic R script that I could run inside a bash script. I wanted those heatmaps to have a clustering algorithm applied to them. When I did this with ggplot2, I had to adjust the dendrogram by hand for each one. That was not an acceptable solution. I found a package called pheatmap that I ended up using for all the heat maps. 

I really like what clustering your data can do as far as identifying similar trends among different groups. I decided to go ahead & try pheatmap on this data. pheatmap requires a matrix. I found a bit of code online that I used to convert the dataframe to a matrix & still keep the row names associated with the data. Code can be found in pheatmap.Rmd. Visualization is pheatmap.tiff. 

4-12-18

Raw data: https://github.com/rfordatascience/tidytuesday/blob/master/data/us_avg_tuition.xlsx  
Data source: https://onlinembapage.com/average-tuition-and-educational-attainment-in-the-united-states/ <br />  
Original graphic: https://onlinembapage.com/wp-content/uploads/2016/03/AverageTuition_Part1b.jpg . 
