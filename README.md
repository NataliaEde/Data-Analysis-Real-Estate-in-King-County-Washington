# Data Analysis: Real Estate in King County, Washington
## Phase 2 Project, Flatiron

![image](https://user-images.githubusercontent.com/44559346/191543006-8b0a9ec2-f677-47f4-9acf-8bfd5004d9af.png)


### Overview

I conducted a case study to examine the housing market in King County , Washington. The purpose of this project is to advise a real estate investment firm in King County, Washington. 

King County’s real estate data study will help the firm predict the market value of a given house, while the conclusions offer recommendations for future investments.

### Method

I coded the analysis using Python using Scikit-learn. The data came from the King County House Sales dataset (2014–2015) provided by Flatiron. 

In my analysis, I followed the following steps:

* Clean the data
* Explore the data  (EDA)
* Prepare for the model 
* Model the data & evaluate the model
* Interpret results


### Exploratory Data Analisys 

My analysis determined that the following four features are most impactful (have the highest correlation) to house prices: square footage, grade, number of bathrooms, and view. 

*Note: I removed redundant data (e.g. square footage above & basement.) Also, when calculating the correlation I removed zip codes since it has the number do not  follow a meaningful order. Zip codes will be added back when I model the data.*

![image](https://user-images.githubusercontent.com/44559346/196205445-0a110e5d-9c83-4ece-bce5-acdc9191c7e0.png)

#### Living space:
Square footage is directly related to the price of a house, but only up to a certain point. Houses larger than 6,000 sq ft do not show a commensurate increase in price. Nonetheless, the few houses larger than 7,500 sqft range between $3 to $7 million. 

![image](https://user-images.githubusercontent.com/44559346/196205547-3ff455c5-9106-45f9-bbb7-a8d4cb790f10.png)


#### Grade:

Grade refers to the quality of the materials and appliances used throughout the structure. Grade is directly related to house prices. Houses with a grade rated higher than 10 range from roughly $1.5 to $4 million.

<img width="326" alt="Screen Shot 2022-10-17 at 10 36 34 AM" src="https://user-images.githubusercontent.com/44559346/196205890-d9258f75-f830-4b57-9495-d726ebe8a18f.png">


#### View:

Having a view, which is characterized by natural features such as water, mountains, and greenery, showed to have a significant impact on housing value. Only 7% of houses have what is considered a “good” or “excellent” view, and these range from $800K to $2 million in value. By comparison, 83% of houses do not have a view, and these range from $350K-$500K in value.

<img width="618" alt="Screen Shot 2022-10-17 at 10 38 45 AM" src="https://user-images.githubusercontent.com/44559346/196206464-7680ab49-9d95-4b1a-a8c0-1d8733b9f83f.png">


### Predicting Prices Using Linear Regression

I predicted prices using linear regression. I used a stepwise selection function on the independent variables to determine which features to use for the linear regression model. The model showed R Squared as 79% in house prices, as explained by 82 housing features. 


### Conclusions and Recommendations

Using the leaner regression model and data analysis, I have determined that the most valuable assets of a house in King County are certain zip codes, view, grade  and square footage. Below are my investment recommendations:


**LOCATION:** Consider investing in zip codes 98125, 98115, 98144, 98178, 98199, 98116,98136 whose market value is currently low to mid-range but also include some of the most profitable housing features.

<img width="427" alt="Screen Shot 2022-10-14 at 6 47 08 PM" src="https://user-images.githubusercontent.com/44559346/196208283-e74b590b-cc2e-4ee8-a749-767c2810962d.png">


**VIEW:** Prioritize a house with a great view, particularly if it has a waterfront.


**GRADE:** Grade is more important than house age. Investing in high quality materials will lead to a profitable outcome.

**SIZE:** Prioritize the size of the indoor, living area rather than the size of the lot. Houses ranging from 2,500 sqft to 5,000 sqft have a high correlation to house prices.


### Next Steps

* Gather more data from previous years
* Focus on profitable transactions (buy/ sell) with the new data.
* Create a racking system for the housing features already mentioned above in order to see which are the most influential on house prices.



### Repository's Navigation  

Jupyter Notebook Code: King County Data Analysis.ipynb

Presentation: presentation.pdf

Data: king_county.csv

