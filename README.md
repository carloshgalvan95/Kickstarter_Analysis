## Overview of Project

### Background

Louise is planning a theater play “Fever”. The estimated budget is over \$10,000 and she already came close to its fundraising goal in a short amount of time.

### Setting up goals

The purpose of the analysis is to determine whether there are specific factors that makes a crowdfunding campaign successful and compare how different campaigns fared in relation to their launch dates and their funding goals.

## Analysis and Challenges

### Defining our tools

The tool utilized to perform the analysis will be Microsoft Excel. Excel allows us to organize, sort and analyze crowdfunding data to determine whether there are specific factors that makes a crowdfunding campaign successful as well as gaining a greater understanding of crowdfunding campaigns from start to finish and mirror other successful campaigns in the same category.

### Organizing data

To accomplish our project goal, we first need to organize our data in a way that allows us to better analyze the exact variables we want to evaluate to determine the possible correlation between them, in this case, the launch dates and funding goals of the comparable Kickstarter projects.

#### Kickstarter campaigns outcome based on launch dates

As the title indicates, our two variables to analyze here will be the outcomes of the Kickstarter projects vs their launch dates. As any other marketing, selling, fundraising, etc. campaign, the interest of the target demographic fluctuates throughout the year depending on a variety of factors and ends up being one of the most important things to determine on any campaign. Based on the data we gathered, on what time of the year is our target demographic most interest in Theater? Will be our main question to ensure success.

##### Evaluating the fluctuations throughout the year

To do this, we must be able to easily look over the outcomes for every month of the year, as well as every year available using a PivotTable and PivotChart.

We are going to filter the data based on parent category to focus on theater plays and years to be able to observe how the trends change depending on the year. Our rows are going to be every month of the year to define patterns of interest given our target demographic (theater plays). Finally, the columns are going to be every possible outcome of the Kickstarter campaigns: canceled, failed and successful.

##### Data Visualization

Finally, we can better visualize how the month of the year correlates to the outcome of the Kickstarter campaign using a line chart with a data point for each month and outcome.

![Theater_Outcomes_vs_Launch](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

#### Kickstarter campaigns outcome based on Goals

To evaluate this correlation we will need to use the function COUNTIFS() to collect the outcome and goal data for the “plays” subcategory.

##### How to organize the data to determine correlation?

Using a chart, we will be able to evaluate the correlation between the two variables. Our columns will be the number of successful, failed and canceled products for better data visualization we will define them by percentages of the total number of projects. The rows that will define the parameter groups will be the Goal amount in groups of \$5000 all the way up to \$50,000 or more, also defining a group with a range of 0 to \$1000 to evaluate smaller Kickstarter campaigns.

##### Data Visualization

Just as we did with our launch dates vs outcomes comparison, to better visualize the information at hand we will be using a line chart to compare and contrast the successful, failed and canceled Kickstarter campaigns with the set goal amount targeted.

![Outcomes vs Goals](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Possible challenges to overcome

#### Too much or too little?

The safe assumption would be, the more data we have, the better we can compare each variable and correlation. But this is ultimately determined by the target demographic to be evaluated, our data gathered provides us with information for a variety of Kickstarter campaigns with very different parent categories and subcategories but also with different countries, which means different cultural context and even more important, different target demographic.

We must question whether including more information that doesn’t necessarily correlates with our range of study would be beneficial and when does broadening our range for the sake of having more data to analyze ends up being counterproductive.

#### Theater enthusiasts

Let’s start with the more obvious classification, in our data we have information for a wide range of categories, ranging from film & video and television, videogames all the way to technology and wearables. Are these categories relevant for our project, possibly but also not completely, It always depends on what the purpose of our analysis is and in this particular case, is safe to assume that we can interpret better correlation patterns if we narrow our range to just theater and plays as the category and subcategory.

The main reason to do this is given that the behavior or the target demographic that is going to possibly pledge to our cause is going to be very different to the average person, organization or company that will become interested in for example, Naptime: the first baby monitor that takes care of parents campaign which we also gathered data from.

![Parent Category Outcomes](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Parent%20Category%20Outcomes.png)

#### Biscuits and cookies

Another important factor to determine is the cultural context of our project. A perfect example to this is simply trying to see the top 3 most popular Netflix series in different countries.

![Top 10 Netflix shows UK](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Top10Netflix_UK.jpg)

![Top 10 Netflix shows US](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Top10Netflix_US.jpg)

We can quickly realize how the country is a relevant variable to take into account, even if the top 10 for just a week doesn’t vary a lot, if we start gathering more data it could be surprising to see the differences in appeal from one country to another.

So, let’s put things into context and see how it compares if we add one more filter to our first PivotTable to compare UK and worldwide Kickstarter campaigns to see how things could go for Louise in the UK.

We can see that even thought there are some differences between both charts, is safe to assume that in order to get more data samples, it would be beneficial to broad the data range to not just one country.

![GB Theater Outcomes vs Launch Date](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/GB_Theater_Outcomes_vs_Launch.png)

## Results

### Is the launch date a relevant variable to consider for our Kickstarter campaign?

TL: DR; yes. As previously mentioned, as for any other campaign, no matter the category or subcategory interest levels vary throughout the year. Now let’s see how this affect our Kickstarter campaign.

#### F is for flowers, spring and “Fever”

From a quick glance to our line chart, we can clearly see that there seems to be a trend for the overall interest in Theater Kickstarter campaigns. Days are brighter during spring and summer and so is our probabilities of success, apparently…There are an incredible number of variables that we would need to take into consideration to be able to explain why this increase in popularity directly correlates with those months, It may be due to the summer break, may be due to an increase in free time available or a plethora of other factors to take into account. But the most important thing is that, our best opportunity to success lays in the months of May, June, July and August, the probability of success reduces during the subsequent months from September to March so it would be in our best interest to avoid those rainy, cold seasons in UK.

We can also see that the actual results vary quite a lot throughout the years, the year where we launch our Kickstarter may be way different than the results we are expecting to accomplish but the best bet would still be for our campaign launch date to fall into the months we already discussed.

### What about our Goal amount?

We can clearly see a trend in every Kickstarter campaign we evaluated. A campaign that looks dauting to accomplish is also a campaign scary to back. We can see two main attractive ranges to set our goal to:

-   \$1000 to \$5000: We can see that this could be our potential goal to adjust the campaign for, the current objective is set to \$10,000 but we can clearly see that the probability of success quickly descends as we look at more ambitious campaigns, the ratio percentage of successful vs failed campaigns goes from a margin of 46% to a difference of 10% for the range of campaigns with a goal amount between \$5000 to \$10,000 and makes us question if not adjusting our budget is worth the potential risk of failures.
-   \$25,000 to \$30,000: we can see a wider margin between the percentage of failed to successful campaigns in this range, but we would have to evaluate more variables like the possibility that the few campaigns that have higher budgets and goals could be coming from established companies or backed by an average pledged amount much higher than for our previous potential range. Also, given that our goal is \$10,000 this information ends up being irrelevant to our project.

### More data, more information, better results…

This affirmation is something that may not be true in all cases, sometimes we can benefit from narrower data, or specific segmented samples to measure every demographic. But in this case, gathering more data specifically taking into consideration both the country where we are intending to launch our campaign and the specific category and subcategory could give us more reliable results.

### Complex is not always better…

Even thought we can rely on tables and raw data, the easier way for us to analyze the information we have been given is to present it in an easy-to-understand format. We already saw how helpful it is to use line charts to recognize patterns and take better decisions and we can further the observable data with the use of different tables and graphs.

One perfect example of would be to use scatter chart to determine if there's any noticeable correlation between two variables. As we can see here using the tendency line we can easily determine if two variables have a positive or negative correlation, or no correlation at all.

![Successful Campaigns Scatter Chart](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Successful_scatter_chart.png)

We can see here that based on our Scatter plot of the two variables, Goal amount of the Kickstarter campaings vs Outcome, for our successful campaigns there is a negative correlation to the probability of success when the Goal amount increases.

![Failed Campaigns Scatter Chart](https://github.com/carloshgalvan95/kickstarter-analysis/blob/main/Failed_scatter_chart.png)

On the opposite side, we can see that there is a clear positive correlation to the probability of failure when the Goal amount increases. To sum things up, the bigger the goal, the higher the probability of failure.
