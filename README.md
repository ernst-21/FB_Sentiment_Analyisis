# FB_Sentiment_Analyisis

Official Cuban Media posted in Facebook a sort of poll about the acceptance of a TV space from a Cuban journalist. 

Although people should evaluate the journalist's TV space rating it from 1 (negative) to 10 (positive), opinions and reviews observed in the comments had a qualitative nature rather than a value from 1 to 10 that would have made our work easier.

Comments were then extracted using GRAPH API through FacePager Software (all content is public and according to Facebook privacy rules).

Data was pre-processed in Excel. We added a 'review' column that classifies comments in 'negative' or 'positive'.

We observed there was a frequency of keywords that were present in negative comments and not so frequent in positive ones. The other way around occured the same, people who wrote positive reviews about the journalist used keywords that were hard to find in negative reviews.

We use the the following formula in Excel to classify comments in negative or positive: =IF(SUM(COUNTIF(B2,{"*keyword_1*","*keyword_2*"...})),"neg","pos"). Keywords were added until there was no significant changes in the proportion bewtween negatives and positives reviews.

We would like to apply ML algorithms to check if the criteria follwed to classify those Facebook comments was accurate and predict the nature of future comments.

Since it is a Cuban poll, extracted comments are in Spanish language. So the examples we will use to test our predictions will be in Spanish as well. Of course we will translate the exemples for our readers have proof of the accuracy of the algorithm.
