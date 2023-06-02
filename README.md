# **Movie Prediction Project**
 
 ![image](https://github.com/JoeBwonKenobi/Movie-Project-3/assets/117705408/ec8610f9-9ce9-4fea-a857-ffd4e5013b64)

# **Project Overview**
 
I produced a MySQL database of movies from a subset of IMDB's publicly available dataset. I used this database to analyze what makes a movie successful and provided recommendations to the stakeholders on how to make a successful movie. There were several steps to completing this project, and I split them up into separate notebooks since the files are so large.
 
Part 1: Download several files from IMDB's movie dataset and filter out the subset of movies requested by the stakeholders.
-Below is the link for the notebook for this part of the project:
https://github.com/JoeBwonKenobi/Movie-Prediction-Project/blob/main/Movie_project_3.part_1.ipynb
Part 2: Use an API to extract box office revenue and profit data to add to your IMDB data and perform exploratory data analysis.
-Below are the links for the notebooks associated with this part of the project:
https://github.com/JoeBwonKenobi/Movie-Prediction-Project/blob/main/Movie_project_3.part_2_A.ipynb
https://github.com/JoeBwonKenobi/Movie-Prediction-Project/blob/main/Movie_Project_part_2.B.ipynb
Part 3: Construct and export a MySQL database using your data.
-Below is the link for the notebook for this part of the project:
Part 4: Apply hypothesis testing to explore what makes a movie successful.
-Below is the link for the notebook for this part of the project:
Part 5: Produce a linear Regression model tp predict movie performance.
# **Hypothesis Testing**
This part of the project contained three questions from a stakeholder using hypothesis testing and statistics knowledge to answer three questions about what makes a successful movie.

# **#1:Does the MPAA rating of a movie (G/PG/PG-13/R) affect how much revenue the movie generates?**

**Null Hypothesis:**
There is no difference in revenue generation between different movie ratings

**Alternate Hypothesis:**
There will be a statistical difference between revenue generation between movie certifications.

For this particular section I took a look at data WITH the outliers of the revenue column and assesd them to get a closesr look.

![image](https://user-images.githubusercontent.com/117705408/229327831-3d07b7ba-b9d4-4bbd-8fdb-a424d1a9450c.png)


The barplot below represents the revenue for each of the certification categories (PG-13, PG, R, G) WITHOUT Outliers to show the difference.


![image](https://user-images.githubusercontent.com/117705408/229327093-7f61d1c3-38bd-415c-b742-1558d9726e3a.png)


# **#2:Do movies with a runtime of 2 hours or more have higher budgets?**

**Null Hypothesis:** There is no difference in budget amounts for movies of 2 hours or more than movies shorter than 2 hours.

**Alternate Hypothesis:** There will be a statistical difference between budget amounts for movies of 2 hours or more than movies shorter than 2 hours. Alpha = 0.05. We will be using a 2-sample T-test.

Below is a Visualization of  average budget differences between short (<120min) movies and long (>=120min) movies

![image](https://user-images.githubusercontent.com/117705408/229327008-b6884f20-461a-4a69-9012-35f485153350.png)

To take this one step further, this is likely due to larger crowd appeal due to the lack of age restrictions of lower certifications, meaning more people view these movies. Also, parents must buy tickets for both their children and themselves when going to see a G movie (potentially, more overall tickets sold).

Our result is less than our alpha of 0.05, which means we REJECT the Null Hypothesis (There is no difference in revenue generation between different movie ratings) and SUPPORT the Alternative Hypothesis (There will be a statistical difference between revenue generation between movie certifications).

# **#3:Does the certification (G, PG, PG-13, R) of a movie affect the movie's average rating?**

**Null Hypothesis:**There is no difference in ratings between movie certifications.

**Alternate Hypothesis:**There will be a statistical difference in ratings between movie certifications.

The barplot below is WITH outliers in the ratings column.

![image](https://user-images.githubusercontent.com/117705408/229327945-d3009623-a742-43cb-a27b-936d6ab2aff6.png)

The barplot below is WITHOUT any outliers in the ratings column.

![image](https://user-images.githubusercontent.com/117705408/229327962-dbbce61c-22c9-4528-a292-e70b916fbae2.png)


Our result is less than our alpha of 0.05, which means we REJECT the Null Hypothesis (There is no difference in ratings between movie certifications) and SUPPORT the Alternative Hypothesis (There will be a statistical difference in ratings between movie certifications).

