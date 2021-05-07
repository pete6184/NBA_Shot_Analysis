# NBA_Shot_Analysis

# Requirements & Summary

In this project, our group used Jupyter Notebook. We used Python and Pandas to write the code and clean the data.

Our initial hypothesis was that pressure effects performance, and therefore, field goal percentages would go down when there was less time left on the shot clock, game clock, and when shooters had a defender within 6 ft of them. 

My portion of the project focused on the field goal percentage as it pertains to the time remaining on the shot clock. I started by creating a dataframe that grouped the number of shots attempted and shots made for each timepoint (24.0, 23.9, 23.8, etc...).

I decided to then break down the data even further and run the same analysis on both 2-point and 3-point shots. For this I simply split the data by shot type and ran the same analysis I mentioned above. 

I then created scatter plots to visualize our findings. The data turned out as expected in that we found that field goal percentage dropped with the time remaining on the shot clock and was at its lowest with less than 5 seconds remaining on the shot clock. 

Lastly, I created a dataframe that put the shot clock times into five separate bins to confirm the data we were seeing on the scatter plots.
