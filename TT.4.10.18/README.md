#TidyTuesday 4-10-18

4-10-18

Started with a simple scatter plot. I used facet wrap to group the plots by position. I wanted to get a look at the data. The hardest part was getting averages of each position based on the year. I'm having trouble applying RColorBrewer palettes to these #TidyTuesday challenges. I've used RColorBrewer in the past but it hasn't been clicking for me lately. Code is scatter.facet.Rmd. Plot is scatter.facet.pdf.

In an effort to try something new, I googled ggplot2 images. I had forgotten about these ridgeline plots. I've always wanted to do one but never seemed to have data that worked with it. I did this one more for looks than anything else. I did two side by side plots: one shows the distribution of average salaries, the other shows the distribution of the intial data. I thought it might be an interesting comparison. Code is ridges.Rmd. Plot is ridges.avg.vs.norm.pdf. ridges.pdf is the original plot of the average salary distribution. I like how it looks so I left it up here. 

4-12-18

I really like heat maps. I like how they look. I like how data looks clustered. I used pheatmap to create a clustered heat map of the average salary by position for each year. I clustered based on position. This exercise reminded me how diffiuclt some packages can be to work with. I couldn't fix the legend labels into dollar amounts. I used a function I had found previously to angle the column labels, which makes them infinitely more readable. 

I was trying to view the .tiff file that was the output for the heat map. Github says it's too big. I'm trying it again as a .png. After trying it as a .png, I realized that the labels are being cut off at the end of the graphic. I'm going to assume this is because I used a custom function to change the labels. I set the height & width manually in the pheatmap function.

My next goal is to try something that plots all the data instead of the averages. I'm trying to decide what visualization would be best for that. 

Data

Raw data: https://github.com/rfordatascience/tidytuesday/blob/master/data/tidy_tuesday_week2.xlsx <br />
Article: https://fivethirtyeight.com/features/running-backs-are-finally-getting-paid-what-theyre-worth/ <br />
Data source: http://www.spotrac.com/rankings/ <br />
Original graphic: https://espnfivethirtyeight.files.wordpress.com/2017/05/morris-nflrb-1.png?w=575&h=488&quality=90&strip=info <br />
