Identifying and Recommending Best Restaurants
1.	Background:  Main goal of the project is to analyze the data and identify best restaurants and generate recommendations
2.	Approach: Preliminary data inspection needs to be performed and any missing values, duplicate data needs to be reported.
3.	Data-processing performed: 
-	Two data files are provided, one with restaurant data with country code and second file with Country code/ country information
-	Merged both the files to get the country information for grouping purpose
-	Added proper format for column names
-	Verified for records with null values
-	Dropped one record without Restaurant_name
-	Cuisines column has 9 records with null values, changed them to ‘Other’
-	Saved the cleaned file to use in Tableau for Dashboard creation
4.	Performing EDA Analysis:
-	Restaurant data provided has presence all over the world but highest in India followed by USA. India has 8651 records and USA has 434
-	Identified the cities with most restaurants. Majority of them are in India:
New Delhi 5473, Gurgaon 1118, Noida 1080 and Faridabad 251
-	Since majority of the restaurants are in India, selected data for this country in my analysis. Explored the franchise with most national presence, which is Café Coffee Day. Checked information such as ratings, average cost per day and price ranges for this franchise.
-	Found out ratio between restaurants with and without Table booking. Only 13% are allowed table booking and 87% does not.
-	Only 28% of restaurants have online delivery option and 72% do not.
-	Cuisines column has multiple entries combined, so split them to get the individual cuisine information to a list and retrieved top 10 cuisines from the list. 
North Indian, Chinese, and Fast food are top 3 in the list
-	Identified the most served cuisine in cities. ‘Café’ is most served and is in 57 restaurants. 
-	Checked restaurant counts with specific ratings in India. Majority (3678) of them have Average rating and 2139 are Not rated. Verified data for restaurants with Excellent and very good ratings and researched on the driving factors for these.
-	Verified the distribution cost across the restaurants considering Agg rating, price range and average cost for 2. 
I observed that there is no linear relation between cost and rating. For instance, 
most of the restaurants with good rating (4–5) seem to be in 1000 or less average cost, so  we cannot say  that rating will be higher if cost is more. Restaurants with good rating (like 4–5) have restaurants with all price ranges and spread across.
-	Identified the relation with ratings with other factors like cost, delivery option etc
Having online delivery or table booking does not seem to be necessarily influence rating of a restaurant as we can see from the data that these options are available for less rating restaurants. 
-	There is no single variable that influences the rating  strongly. Correlation is 0.40 for Price range and Aggregate rating which is little higher than the rest. This could be because people who visit these restaurants may be educated folks and can afford the cost and provide feedback.  People who visit low price restaurants don't care about ratings. Social media presence and advertisement may influence ratings to go up for these.
