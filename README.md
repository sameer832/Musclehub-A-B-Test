# Musclehub-A-B-Test


# About
Currently, when a visitor to MuscleHub is considering buying a membership, he or she follows the following steps:

- Take a fitness test with a personal trainer
- Fill out an application for the gym
- Send in their payment for their first month’s membership
Janet, the manager of MuscleHub, thinks that the fitness test intimidates some prospective members, so she has set up an A/B test.

Visitors will randomly be assigned to one of two groups:

- Group A will still be asked to take a fitness test with a personal trainer
- Group B will skip the fitness test and proceed directly to the application
- Janet’s hypothesis is that visitors assigned to Group B will be more likely to eventually purchase a membership to MuscleHub

# Languages
- python(pandas,matplotlib,scipy)
- SQL

# Step 1 Investigate the A and B groups
- Using Pandas to add another column to the dataset, to help distinguish between people in group A, and B
- Using groupby to make sure that both groups contain around the same number of people. Also created a pie chart using matplotlib for visulization

# Step 2 Who picks up an Application?
- Added another column which distinguishes between people who ended up filling out an application and those who didnt
- We want to calculate the percent of people who complete an application, so I pivoted the data, and split the two groups between A and B, and as we can see more people
from group B filled out an application.
- Completed a chi-square test to see if the results were significant, and since our p-value is less then 0.05, we can conclude the results were significant

# Step 3 Who purchases a membership?
- created a new column which distinguished betweeen people who ended up filling out an application and purchased a membership, and those who didnt
- Came to the conclusion that people who took the fitness test were more likely to purchase a membership, however, after conducting a chi-square test our p-value was
greater then 0.05, so the results were not significant
- Finally, when considering all people who visited MuscleHub split between groups A and B, from the last table in this section we can see a higher pecent of people proceeded
to purchase a membership in group B. When conducting a chi-square test to check the significance, I got a p-value < 0.05 therefore concluding that the results were significant

# Step 4 Summarize the acquisition funel with a chart
- lastly to display my findings, using matplotlib I created 3 different bar charts for the different scenerios. The first plot covers those filled out an application,
the second plot covers those who filled out an application and purchased a membership, and the last plot covered all vistors who purchased a membership. 
- I can come to the conclusion that Janet's hypothesis was correct, visitors assigned to group B are in fact more likely to purchase a membership



