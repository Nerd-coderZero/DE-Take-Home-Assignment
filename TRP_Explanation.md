# TRP Priority Calculation for Cricket Matches

## 1. How I Combined the Priority Parameters
- To figure out the TRP priority, I combined different factors that seemed important for predicting how much interest a cricket match might generate. I looked at things like the type of series, the teams playing, the time of the match, and any special rivalries, like India vs Pakistan. Each of these got a score based on how important they seemed.

### For example:

- Series Type: World Cup matches are a big deal, so I gave them higher points. Other series got fewer points.
- Teams: Teams like India, Australia, and England usually draw more viewers, so they got higher scores too.
- Rivalry: Matches with big rivalries, like India vs Pakistan, were given a lot of points because they tend to attract more attention.

I combined all these scores to come up with a final TRP score for each match, which basically tells us how important that match is in terms of viewership.

## 2. Assumptions and Simplifications
- Since I didn't have all the details about the matches, I made some assumptions:(Internet tools helped with those)

- Unknown Values: If I didn't know something, like the time of the match or the rivalry, I either left it out or gave it a default score.
- Time Slot Simplification: The time slots weren't always clear, so I just picked some general ranges and assigned scores based on that.
- Simplified Rivalries: Not every match had a clear rivalry, so if there wasn't one, I just gave it a default low score.

## 3. Handling Edge Cases and Conflicting Priorities

- Sometimes the data had missing or weird values. For instance, if the match time or team names were missing, I gave them a default value or ignored them to avoid errors. When there were conflicting priorities (like two equally important teams playing), I just added their scores together and let the final number decide. [OfCourse I had to trial and check multiple times by running the output to see if there is still some mising/wierd value or case left]


```python

```
