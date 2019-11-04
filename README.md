# Data_incubator_project
# proposed project for Facebook Followers

Facebook Followers Project
Wenqin You

1	Background
It’s very interesting and powerful to analyze the real feedback data from the Facebook follower. It’s probably not obvious to generate some relationship at first glances. But detailed follower analysis is important for each company to help them know their economic performance and predict the future trends. This interesting and diverse data is worth further and deeper investigation. It’s highly possible to give strategic plans to help them improve income or avoid the lost. 

2	Data Description & Challenge
Facebook provide a myriad of data points about companies such as customer traction, foot traffic, and brand awareness among others and explain the analysis you are performing.
This big dataset contains information from more than 1 million cases with 14 columns describing their properties. This dataset contains more than 3163 companies from 2015 to 2018. Facebook followers provide the information about ‘checkins’, ‘were_here_count’, ‘likes’, ‘talking_about_count’ and ‘facebook_id’, which are defined as the feature vectors in my analysis. Additionally, the moving averaging model is needed for the time-series data. 

3	Hypotheses/Goals

Goal 1: Exploratory data analysis
1.	For the same company, whether these feature vectors are correlated. Correlation matrix and principle component analysis can be conducted. Whether more checkins or likes represent higher ‘talking about count’. 
(The preliminary result shows each company has unique performance. Case-by-case analysis is required for the interested company)

2.	For each feature vector, plot feature vector V.S. time for top 15 companies in one figure; aim: to understand the different behavior of the companies for each feature vector. (top: largest data available). 

3.	If we find some feature vectors are interesting, studying it deeper. For example, Compare companies with highest volatility of “talking about count” — who they are – and use any information online to see if this metric overlaps with highly publicized events and marketing campaigns.

4.	Facebook check-ins as a metric for foot traffic for restaurant, hospitality and retail businesses. Who are the winners in attracting customers to physical locations.

5.	Facebook followers and which companies are the most successful at growing social media traction

6.	Using moving averaging model to analyze the popularity of a series of companies. The preliminary curve is not smooth and the moving averaging model is needed for this time-series data. 

7.	Using domain knowledge to pick out the semi-conductor and oil/chemical/manufacturing companies, it’s interesting to know whether they showed any cyclic effect. 
Goal 2: Develop model of company classification
It’s interesting to classify the types of companies based on these feature vectors. For example, what companies have the top five likes; what’s the types of these companies? The types can probably be high-tech, grocery, hospital, school or fast-food-chain.

Goal 3: Establish model for some companies to predict their 2019 ‘likes’ & ‘talking about counts’ & ‘checkins’ by data training
It will be helpful if we can predict their future popularity. For goal 3, the dataset was split into training sets (data before 2018-01-01) and test set (data after 2018-01-01) . Different regression models will be tried here to improve their accuracy. Finally, the model will be used to predict their future performance. 


4	Definition of Success
Success is defined as a complete workflow that achieves all four of the goals of the project. The lowest level that can be deemed a success is producing a working code to finish all the exploratory data analysis, to classify the companies into k categories, and to build a model that can predict the feature vector of each selected companies. An expected level of success is that code will utilize a verification and validation strategy, and be able to predict future performance of company with R2 no less than 0.75.  (The performance means ‘likes’, ‘checkins’ or ‘talking_about_counts’).  
For example, each company can know and predict its popularities among the social media by ‘likes’ or ‘talking_about_count’. For the food or grocery companies etc., they can know their economic performance by ‘checkins’ or ‘were_here_count’. 

5	Deliverables
The key deliverable will be a Jupyter notebook that contains:
●	Appropriately organized data set
●	Exploratory data analysis
●	Code to reproduce all analyses
●	Documentation of inputs/outputs of all functions
●	Quantitative and visual assessment of regression accuracy
●	Quantitative and visual assessment of prediction accuracy
●	Written critical analysis of success/failures of the model
