# Speed Dating - How do you fare?
## Introduction 
Singles today have a plethora of options to help them find their future partner ranging from the traditional meet-cute method to online/social media platforms. Dating is often seen as "shopping" for a potential partner, and like shopping, there is a value associated with potential partners that each individual encounters. It is likely at some point, an individual has wondered what their value is in the dating market. 

The data collected from a series of speed dating events allows me to see how accurate participants self assessments are in comparison to how others rated them. 

## Exploration
The dataset provided by Columbia Business School on Kaggle had 195 columns containing information such as age, ethnicity, income, place of origin, gender, hobbies, and key focus attributes that were collected between 2002 and 2004 during 21 speed dating events. I placed my focus on sets of columns that asked the following:
  1. Attributes their partner possessed
  2. What are the most important attributes to you?
  3. How do you rate yourself?
  4. How do you think others rate you?

The dataset provided each partner each participant met and how they ranked. First, I wanted to explore trends across different ethnicities by gender. 


![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Desired%20Attributes%20for%20Men.png?raw=True "Desired Attributes for Males")

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Desired%20Attributes%20for%20Women.png?raw=True "Desired Attributes for Females")

#### As shown in the above graphs:
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

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/f_attr1_1.png?raw=True "Female attractiveness priority") 
![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/m_attr1_1.png?raw=True "Male attractiveness priority") 

More graphs for each attribute can be found [here](https://github.com/okwan91/Speed_dating/tree/main/images).

### Self Rating vs Self Market Rating
The dataset provided data on how participants rated themselves and how they think others rate them. I defined these two points as their self rating and market rating. 99% of participants provided a self rating while only 55% provided a market rating. More males gave a market rating than females, but not significantly more. 

When looking into correlations between self and market ratings and their attributes, all the attributes have about the same amount of weight towards market ratings. While analyzing the correlation between self ratings and their attributes, intelligence and attractiveness had a higher correlation and sincerity being the lowest.

![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Corr_Market.png?raw=True "Market Correlation") 
![alt text](https://github.com/okwan91/Speed_dating/blob/main/images/Corr_Self.png?raw=True "Self Correlation") 

### You vs Everyone Else
How I tested how accurate participant's self ratings was by utilizing self ratings, market ratings, and partner ratings to calculate a percentage of error between each self rating against how each participant's partner rated them. 
