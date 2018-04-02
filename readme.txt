Exploratory analysis

Adding location which will be used to combine all datasets together.

info shows that most the variables are of string type. We have to convert some variables into int or float type to do the analysis.

describe shows that most of the videos have 0 likes and 0 dislikes.
The views, likes, and dislikes have 1 row less as compared to video_id etc. This will create some problem  in analysis so we will remove that row.

Checking the number of missing values confirmed that there are missing values in the data.

I changed 'view','likes','dislikes', and 'comment_count' into numeric type.

Correlation matrix shows that there is a strong correlation between comment_count and dislikes.
From which we can infer that people comment more often on videos they don't like.

As we show in the output of the videos with highest views there were many duplication of the rows.
We will remove those rows and will only keep the most recent views and other details.

Most viewed video: The Shape of 2017
Most liked video: The Shape of 2017
Video with most comments: So Sorry
Video with most dislikes: So Sorry

It is important to let user to see the stats of a video(or a list of video). And that is why we created two functions one which let you see the stats based on video_id and title.
We are displaying multiple bar graph which has 4 bars.
 