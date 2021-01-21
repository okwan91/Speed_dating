# Speed Dating - How do you fare?
## Introduction 
Singles today have a plethora of options to help them find their future partner ranging from the traditional meet-cute method to online/social media platforms. Dating is often seen as "shopping" for a potential partner, and like shopping, there is a value associated with potential partners that each individual encounters. It is likely at some point, an individual has wondered what their value is in the dating market. 

The data collected from a series of speed dating events allows me to see how accurate participants self assessments are in comparison to how others rated them. 

## Exploration
The dataset provided by Columbia Business School on Kaggle had 195 columns containing information such as age, ethnicity, income, place of origin, gender, hobbies, and key focus attributes that were collected between 2002 and 2004 during 21 speed dating events. I placed my focus on sets of columns that asked the following:
  1. Attributes their partner possessed
  2. What are the most important attributes to you?
  3. How do you rate yourself? (Self Rating)
  4. How do you think others rate you? (Perceived Market Rating)

The dataset provided each partner each participant met and how they ranked. First, I wanted to explore trends across different ethnicities by gender. 

The below graphs show the top attributes desired by gender and ethnicity. For example, "Attributes Desired in Women by Ethnicity" displays how the shown attributes are ranked by ethnicity for men. AKA, "What attributes do men find most important in women?" Each attribute is allocated 15-20 points (some waves would have 5 attributes and some had 6) and the below shows the average of high each attribute fared.

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Desired%20Attributes%20for%20Men.png?raw=True "Desired Attributes for Males")

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Desired%20Attributes%20for%20Women.png?raw=True "Desired Attributes for Females")

#### As shown in the above graphs:
Women tend to find intelligence the most important attribute in a potential partner with fun and sincerity clsoe behind. In contrast men found attractiveness most important, followed by intelligence.

  * Females prioritized attributes:
    1. Intelligence
    2. Fun/Sincerity
    3. Attractiveness
    4. Ambition/Shared Interests
  * Males prioritized Attributes:
     1. Attractiveness
     2. Intelligence
     3. Fun/Sincerity
     4. Shared Interest
     5. Ambition 

#### Female Preferences vs Male Preferences by Age on Average
The below graphs are organized by highest priority for these age groups and ethnicity. Specifically for the attractiveness attribute, I expected the priority of that attribute to decrease as the age of our participants increased. However you can see below that for some groups of females, it is the opposite. 

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/f_attr1_1.png?raw=True "Female attractiveness priority") 
![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/m_attr1_1.png?raw=True "Male attractiveness priority") 

More graphs for each attribute can be found [here](https://github.com/okwan91/Speed_dating/tree/main/images).

### Self Rating vs Self Market Rating
The dataset provided data on how participants rated themselves and how they think others rate them. I defined these two points as their self rating and market rating. What is the difference between self rating and self market rating? Self rating would be "I think I am a 8 out of 10" while self market rating is "I think others would score me at a 7 out of 10." While exploring the data, 99% of participants provided a self rating while only 55% provided a market rating. More males gave a market rating than females, but not significantly more. 

When looking into correlations between self and market ratings and their attributes, all the attributes have about the same amount of weight towards market ratings. Factoring in our above statement involving the disparity between participants giving themselves a self rating vs market rating, this can be perceived as those who are confident enough to provide a market rating would give themselves a higher score in general.

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Corr_Market.png?raw=True "Market Correlation") 

While analyzing the correlation between self ratings and their attributes, intelligence and attractiveness had a higher correlation and sincerity being the lowest.

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Corr_Self.png?raw=True "Self Correlation") 

### You vs Everyone Else
Utilizing the mean absolute percentage of error between participant's self ratings, perceived market ratings, and their partner given ratings. Those who provided a market rating had a 26.5% average percent of error while their self ratings had a 25.4% average percent of error. 

## Conclusion
People are able to guess within the range of their market value. However due to each date's individual preferences, you could score above or below your market rating. While exploring the data, one participant could be given a score of 95 out of 100 points with one date, and then given a score of 14 by another. In the future I would like to dive deeper into these figures, such as seeing how inflated participant's market ratings were vs their self ratings and if there are any trends according to age, gender, or ethnicity. While I had used the percentage of error for this project, it would also be interesting to apply a linear regression model to this dataset to see if individuals, based on their attributes or other characteristics, are able to predict their market value. 


## Future Questions
* How much did participants over or under rate themselves? Would there be certain demographics that had better rates of accuracy?
* Can other attributes such as age, income, educational background influence how participants rated themselves?
* Obtain a more recent data set to see if there are generational changes in what attributes are seen as most desirable. 
* Observe if there were any changes in participant’s self ratings after their matches were revealed.

