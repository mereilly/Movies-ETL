# M. Reilly's ETL Pipeline, topic Movies 
[Links are working, and images are formatted and displayed where appropriate (2 pt).]

A README.md that describes the purpose of the repository. Although there is no graded written analysis for this Challenge, it is encouraged and good practice to add a brief description of your project.

## Project Overview 
### Background
<!-- Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Britta needs your help to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. You’ll need to refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database. -->

The ETL_function_test.ipynb file
The ETL_clean_wiki_movies.ipynb file
The ETL_clean_kaggle_data.ipynb file
The ETL_create_database.ipynb file
The Resources folder with the wikipedia.movies.json, movies_metadata.csv, movies_query.png, and ratings_query.png files.


Deliverable 1: Write an ETL function to read three data files
Deliverable 2: Extract and Transform the Wikipedia Data
Deliverable 3: Extract and Transform the Kaggle Data
Deliverable 4: Create the Movie Database


You will earn a perfect score for Deliverable 4 by completing all requirements below:

The data from the movies_df DataFrame replaces the current data in the movies table in the SQL database, as determined by the movies_query.png. (5 pt)
The data from the MovieLens rating CSV file is added to the ratings table in the SQL database, as determined by the ratings_query.png. (5 pt)
The elapsed time to add the data to the database is displayed in the ETL_create_database.ipynb file. (5 pt)


	•The client Louise just barely came short on her fundraising goal. Thus, we are tasked with using a dataset derived from Kickstarter to interpret especially what variables 	led to successful outcomes for various campaigns of similar natures to that of Louise. Louise's project was in the theater category, as she was fundraising for a play 		(entitled "Fever"). After reformatting and converting certain elements from the original dataset, we will produce the following deliverables for her to receive in addition 	to the enclosed report: There will be a file will ".png" files that include charts made to help visualize the campaign outcomes based on their launch dates as well as the 	outcomes relative to the funding goals. 


    In this challenge, you’ll edit, or refactor, the Module 2 solution code to loop through all the data one time in order to collect the same information that you did in this module. Then, you’ll determine whether refactoring your code successfully made the VBA script run faster. Finally, you’ll present a written analysis that explains your findings.

<!-- Refactoring is a key part of the coding process. When refactoring code, you aren’t adding new functionality; you just want to make the code more efficient—by taking fewer steps, using less memory, or improving the logic of the code to make it easier for future users to read. Refactoring is common on the job because first attempts at code won’t always be the best way to accomplish a task. Sometimes, refactoring someone else’s code will be your entry point to working with the existing code at a job.
This new assignment consists of one technical deliverable and a written report to deliver your results. You will submit the following:

Deliverable 1: Refactor VBA code and measure performance
This deliverable will include an updated workbook and a folder with PNGs of the pop-ups with script run time
Deliverable 2: A written analysis of your results (README.md) -->


### Purpose
	•The purpose is to establish relevant metrics of outcomes and parameters of different fundraising attempts on Kickstarter for Louise to have better guidance on what 		scenarios would improve her overall chances for success with a similar fundraising attempt. One would have to filter most similar projects based on category-type based 	variables to create a more relevantly comparable analysis for Louise to reference once the analysis is properly interpreted. We're using subcategories, specifically that 	of "plays" to further that aim.

## Results
### The analysis with screenshots and code  


## Summary 
### Advantages and Disadvantages of Refactoring Code 
	•Using our graph we can see that the lowest curve is outright canceled projects, we can follow the "successful" outcomes curve and see that overall it remains above the 	failed and canceled attempts. Further, there appears to be a correlation with successful projects and May start dates, but we do not have more information on this specific 	graph on the duration of those projects or the different variables associated with them. For instance we know from working with the data that they use different start years, 	yet the graph does not distinguish that variable nor others like the amount of backers. This graph does not even discriminate between goal amounts, treating success equally 	even if it came at a larger or smaller amount.  
	•Second, we notice a data gap for canceled projects between September and November months. It does not provide evidence of any hypothesis, but it is an interesting 		observation potentially worthy of future investigation.

### Advantages and Disadvantages of the original and refactored VBA script 
	•Using this data and that in the Subcategory statistics, we can infer that the theater category, the success rate of fundraising efforts for plays is more than double of 	that of the failures of such efforts for this specific subgroup. 

### Challenges and Difficulties Encountered
	• Working with a unix time stamp for the first time reminded me of the need to constantly be looking up terms and relying on my ability to quickly look for answers and 	solutions. The first challenge without a doubt was simply getting over that hurdle and determining the date conversion formula. It was also imperative to have a keen and 	flexible understanding of terms used in the downloaded data when compared to instructions given for the analysis (e.g. understanding that the launch date year was the year 	needed for work in the next spreadsheet following the title of the assignment to gain understanding of the variable needed to complete the objective).
	• When working with the "Outcomes Based on Goals" Sheet it became very tedious to manually input changes to the formula, albeit for only 13 rows. The manual editing makes it 	easy for errors to slip through the cracks even with constant review. 
	• Further, while formatting certain equations, I encountered a few syntax issues and error codes. 

## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?
	•Potentially we could say that based on the graph derived there is a history of successful projects if your project launch date is in May, but a significantly lower one if 	you wait to launch in December. While its a correlative relationship and not a causal one, we can potentially state an outright higher probability based on these statistics.
	•Second,
- What can you conclude about the Outcomes based on Goals?
	•Using this data (of the "Outcomes Based on Goals" and that in the "Subcategory Statistics"), we can infer that the theater category, the success rate of fundraising efforts 	for plays is more than double of that of the failures of such efforts for this specific subgroup. This bodes well for Louise. Still, she must consider the limitations of the 	dataset as a whole in terms of limited representation.  
	•Also, it is note worthy that the projects had the goal less than 1000 a higher chance of success.
 
- What are some limitations of this dataset?
	• First, organizing the data by month in out pivot tables creates unequal comparisons when considering Kickstarter projects started in the same month but different year. 	Knowing that the annual contexts held different trends and scenarios calls into question any comparisons made across year variables, even if projects belonged to the same 	parent category or subcategory. 
	
	• Louise should also consider that this data is being drawn from a limited source (i.e. the Kickstarter platform). There are other variables or trends we may not be 		accounting for or aware of because of the limited scope of this data even if the sampling size may seem large at first glance. In reality, a few thousand projects across 	this many years and categories is not a full representation of the general entrepreneurial attempts. 
	

- What are some other possible tables and/or graphs that we could create?
	•We could create a histogram to further visualize and account for any outliers, thereby further clarifying trends. We could also create a pie chart in the category of 		theater to show how large of its successes are attributed to fundraising for "plays"-- this however may be skewed because of the nature of the larger representation of such 	projects within the subgroup. 
	•To that end, we may want to create a tale to keep focusing on that subcategory or even in that parent category and establish what minimum fundraising goals had the best 	chances for success, given Louise narrowly missed her goal. We could also do other tables that take a deeper look at the average percent funded by each individual backers to 	figure out what is a realistic metric to ask of donors to set and aspire for accounting for further variables not explored above.   



