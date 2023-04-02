# Movie Project
 
 
 This was my Third and final projec twhilst attending Coding Dojo. For this project, I was required to produce a MySQL database on Movies from a subset of IMDB's publicly available dataset. Ultimately, I used this database to analyze what makes a movie successful and provided recommendations to the stakeholder on how to make a successful movie. There were serveral steps to completing this project and I split them up into separate notebooks since the file is so large.
 
Part 1: Download several files from IMDB’s movie data set and filter out the subset of moves requested by the stakeholder.

Part 2: Use an API to extract box office revenue and profit data to add to your IMDB data and perform exploratory data analysis.

Part 3: Construct and export a MySQL database using your data.

Part 4: Apply hypothesis testing to explore what makes a movie successful.

## **Hypothesis Testing:**

Null Hypothesis:There is no difference in revenue generation between different movie ratings

Alternate Hypothesis:There will be a statistical difference between revenue generation between movie certification

For this particular section I took a look at the outliers of the revenue column and assesd them to get a closesr look.

The barplot below represents the revenue for each of the certification categories (PG-13, PG, R, G)


![image](https://user-images.githubusercontent.com/117705408/229327093-7f61d1c3-38bd-415c-b742-1558d9726e3a.png)

To take this one step further, this is likely do to larger crowd appeal due to lack of age restrictions of lower certifications, meaning more people view these movies. Also parents must buy tickets for both their children, and themselves when going to see a G movie (potentially, more overall tickets sold) Our result is < (less than) our Alpha of 0.05, which means we: REJECT the Null Hypothesis (There is no difference in revenue generation between different movie ratings) SUPPORT the Alternate Hypothesis (There will be a statistical difference between revenue generation between movie certification) The stakeholder's SECOND question is: Do movies with a runtime of 2 hours or more have higher budgets? Null Hypothesis: There is no difference in budget amounts for movies of 2 hours or more than movies shorter than 2 hours Alternate Hypothesis: There will be a statistical difference between budget amounts for movies of 2 hours or more than movies shorter than 2 hours Alpha = 0.05 We will be using an 2 sample T-test

Below is a Visualization of  average budget differences between short (<120min) movies and long (>=120min) movies

![image](https://user-images.githubusercontent.com/117705408/229327008-b6884f20-461a-4a69-9012-35f485153350.png)

To take this one step further, this is likely do to larger crowd appeal due to lack of age restrictions of lower certifications, meaning more people view these movies. Also parents must buy tickets for both their children, and themselves when going to see a G movie (potentially, more overall tickets sold) Our result is < (less than) our Alpha of 0.05, which means we: REJECT the Null Hypothesis (There is no difference in revenue generation between different movie ratings) SUPPORT the Alternate Hypothesis (There will be a statistical difference between revenue generation between movie certification) The stakeholder's SECOND question is: Do movies with a runtime of 2 hours or more have higher budgets? Null Hypothesis: There is no difference in budget amounts for movies of 2 hours or more than movies shorter than 2 hours Alternate Hypothesis: There will be a statistical difference between budget amounts for movies of 2 hours or more than movies shorter than 2 hours Alpha = 0.05 We will be using an 2 sample T-test
