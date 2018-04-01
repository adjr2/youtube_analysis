Exploratory analysis

Adding location which will be used to combine all datasets together.

info shows that most the variables are of string type. We have to convert some variables into int or float type to do the analysis.

describe shows that most of the videos have 0 likes and 0 dislikes.
The views, likes, and dislikes have 1 row less as compared to video_id etc. This will create some problem  in analysis so we will remove that row.

Checking the number of missing values confirmed that there are missing values in the data.

I changed 'view','likes','dislikes', and 'comment_count' into numeric type.

Correlation matrix shows that there is a strong correlation between comment_count and dislikes.
From which we can infer that people comment more often on videos they don't like.