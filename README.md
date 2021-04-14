# NBA_Shot_Analysis

# Requirements & Summary

In this project, our group used Jupyter Notebook. We used Python and Pandas to write the code and clean the data.

We started by pulling in a .csv file from Kaggle.com of all the shots taken during the 2014-15 NBA season. We created a dataframe and then dropped the columns we didn't need. We ran into one of our biggest challenges at the beginning of cleaning the data. There were several instances where the shot clock column was showing 0 seconds. This is due to the game clock being under 24 seconds (in each quarter) and the shot clock being turned off. Since there was a game clock time recorded for these instances, we decided to simply copy the time remaining on the game clock over to the shot clock column. This should've been an easy fix, but we quickly found out that these two columns were not holding the same data types. The game clock was listed as an object, and the shot clock as a float. After a lot of brainstorming, we decided to split the game clock on the ':' and convert it to an integer. With this issue finally resolved we were able to start looking into the effects the time remaining on the shot (and game) clock had on player performance. 

Our initial hypothesis was that pressure effects performance, and therefore, field goal percentages would go down when there was less time left on the shot clock, game clock, and when shooters had a defender within 6 ft of them. 

My portion of the project focused on the field goal percentage as it pertains to the time remaining on the shot clock. I started by creating a dataframe that grouped the number of shots attempted and shots made for each timepoint (24.0, 23.9, 23.8, etc...).

I decided to then break down the data even further and run the same analysis on both 2-point and 3-point shots. For this I simply split the data by shot type and ran the same analysis I mentioned above. 

I then created scatter plots to visualize our findings. The data turned out as expected in that we found that field goal percentage dropped with the time remaining on the shot clock and was at its lowest with less than 5 seconds remaining on the shot clock. 

Lastly, I created a dataframe that put the shot clock times into five separate bins to confirm the data we were seeing on the scatter plots.

![shotClock](output_data/Images/FG%1.png)

![2ptShots](output_data/Images/FG%2.png)

![3ptShots](output_data/Images/FG%3.png)
