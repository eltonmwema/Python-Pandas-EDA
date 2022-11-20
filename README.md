# Phase 1 project.
# 1.BUSINESS UNDERSTANDING
## 1.1.Business Problem
Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies.I am charged with exploring what types of films are currently doing the best at the box office. i will then translate those findings into actionable insights that the head of Microsoft's new movie studio will use to help decide what type of films to create.

## 1.2. Success Metric
This project will be considered a success if :

  1.The best selling and most produced films are identified
  
  2.The market gap is clearly identified
  
  3.Possible challenges likely to be encountered,e.g competitors are outlined
# 2.DATA UNDERSTANDING
## 2.1.Importing relevant libraries
Here all the relevant usefull libraries are imported for easier computations

## 2.2.Reading the datasets
Here we look at the datasets and decide on the most relevant to our analysis data sets imported include :
                    1. Movies data set  
                    2. Budget dataset 
                    3. The movie basics dataset

## 2.3 Exploring the datasets
We are describing these 3 data frames to understand on which sets we can combine to work on in order of  
                    a. 2.3.1 
                    b. 2.3.2

#### 2.3.2.1 Tidying
we are tidying the budget data set as we notice null values and odd data types that could affect our analysis after realizing that it has alot of ubnormalities

# 3. DATA PREPARATION
After having the relevant information about the Data sets,i have decided to use two of them by merging. They are the movies dataset and the Budget dataset as the contain all relevant questions

## 3.1 Selecting and Merging
We merge the two dataset that have been decided on

The merge() function is used and the resultant dataset is larger and more relevant

data_set = Movies.merge(Budget ,how = 'inner',on = 'title')

## 3.2 Data cleaning
On data cleaning we check on the following: 
                      1. Uniformity 
                      2. Completeness 
                      3. Consistency 
                      4. Validity

# 4. DATA ANALYSIS
Here we make usefullness of ur cleaned data set through visual insights and other descriptive statistics.

I also did several plottings for easier interpretations,as viewed in the main notebook indicating relationships between various factors

Bar graph indicating popularity of the studios
This bargraph however keeps changing with execution as the sample data is randomized but the output drives equivalent conclussions on the B.V studios
![image](https://user-images.githubusercontent.com/87186427/202922790-d452a1eb-c1e8-4dcd-a705-d98d9cb0e202.png)

scatter plot showing the relationship between the income and progression over the years
![image](https://user-images.githubusercontent.com/87186427/202922929-f277a8cc-d123-4087-83fa-d350af62b028.png)

# 5. CONCLUSIONS
1.English movies have the highest ratings and popularity based on our datasets and visualizations

2.Movies production has declined over the years whereas potential consumers increase due to worldwide population increase possibly due to monopolistic competition hence some dtudios end up downscaling

3.B.V studio offers the greatest competition based on production of the most popular english movies

4.There is no correlation between what is earned at home and internationally and also intwenational income and the progressive years

# 6. RECOMMENDATIONS
1.That there is a market gap that needs to be filled on the production and microsoft studios could utilize that opportunity by massive venture as production has dropped over time.

2.The best benchmark studio is B.V studios as it is the greatest and the best based on the current market gap.

3.The gross average income of every studio depends on its efforts to produce popular movies with an average vote count of above 7.0 and no other factors based on our scatter plots hence the microsoft studio will have no option but to give the best for optimum income
