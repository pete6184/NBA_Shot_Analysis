# NBA_Shot_Analysis

# Requirements & Summary

In this project, our group used Jupyter Notebook. We used Python and Pandas to write the code and clean the data.

Our initial hypothesis was that pressure effects performance, and therefore, field goal percentages would go down when there was less time left on the shot clock, game clock, and when shooters had a defender within 6 ft of them. 

My portion of the project focused on the field goal percentage as it pertains to the time remaining on the shot clock. I started by creating a dataframe that grouped the number of shots attempted and shots made for each timepoint (24.0, 23.9, 23.8, etc...).

![FG%1](https://user-images.githubusercontent.com/74940976/118900909-eb8f3b00-b8c6-11eb-9d98-c31a5d6e3b4a.png)

I decided to then break down the data even further and run the same analysis on both 2-point and 3-point shots. For this I simply split the data by shot type and ran the same analysis I mentioned above. 

I then created scatter plots to visualize our findings. The data turned out as expected in that we found that field goal percentage dropped with the time remaining on the shot clock and was at its lowest with less than 5 seconds remaining on the shot clock. 

![FG%2](https://user-images.githubusercontent.com/74940976/118900926-f34edf80-b8c6-11eb-8f3c-27acdd5701d0.png)

![FG%3](https://user-images.githubusercontent.com/74940976/118900928-f5b13980-b8c6-11eb-856d-62b4a414f83f.png)

Lastly, I created a dataframe that put the shot clock times into five separate bins to confirm the data we were seeing on the scatter plots.

![shot_clock_bins](https://user-images.githubusercontent.com/74940976/118901061-3a3cd500-b8c7-11eb-820c-c2e6d3b971a1.PNG)
