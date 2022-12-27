# This repository contains 
1. a report in PDF format 
2. an ipynb file corresponding to the PDF generated for the purpose of placement Assessment.
3. Data used for price prediction

# Home.LLC-Assessment
Stage 1 - Assessment Question.  What are all the factors that could influence residential home prices across the United States over the next decade? And how? Organize your output in a MECE framework


link for the report in pdf format: https://drive.google.com/file/d/1XZJ2Vd1WsgHR_z4VZNwp0D9ABuiPKyGH/view?usp=sharing



The approach chosen is Supply Vs Demand.


 



Where the Data comes from?
Data with respect to the above mentioned features were resourced from FRED(Federal Reserve Economic Data).
ID	Features	Details	Link
BOGZ1FL073165103Q
	Interestrate_priceindeces	Interest Rates and Price Indexes; Contract Rate on 30-Year, Fixed-Rate Conventional One-to-Four-Family Residential Mortgage Commitments, Level
	    https://fred.stlouisfed.org/series/BOGZ1FL073165103Q

UNRATE
	Unemployment_rate	Unemployment Rate
	https://fred.stlouisfed.org/series/UNRATE

MSPUS	Median_salesprice	Median Sales Price of Houses Sold for the United States 
	https://fred.stlouisfed.org/series/MSPUS

MSACSR	Monthly_supply_of_newhouses	Monthly Supply of New Houses in the United States 
	https://fred.stlouisfed.org/series/MSACSR

HSN1F
	New_onefamily_houses_sold	New One Family Houses Sold: United States 	https://fred.stlouisfed.org/series/HSN1F

GDP
	Gross_domestic_product	Gross Domestic Product 	https://fred.stlouisfed.org/series/GDP


               
How is the Data framed?
The downloaded data was pre-processed and cleaned using pandas and NumPy library.
The steps involved in pre-processing along with the codes for prediction can be referred in the  Home. LLC Prelims Assessment.ipynb file.

Why were these features chosen?
Based on the previous history (from 1970s till present), these features showed to have strong influence in the House Price prediction of any nation.
A common family’s decision to buy or not to buy a residential property will relies majorly on the family’s financial stability and nation’s financial stability, which in turn reflects In the supply and demand of the commodity (Residential property in our case).
Each feature chosen are linearly independent (i.e.., Mutually exclusive) and have a positive or negative correlation with the target-House price (i.e.., Collectively exhaustive) 
The trend in each feature from 1972 till present can be seen from the plots below.
Even though the unemployment rate fluctuates throughout the decades, the GDP is constantly on a raise. This might help us predict the trends in the upcoming years, we can expect the US Economy to not have visible influence based on the current recession phase ongoing worldwide.
 
    




How is Feature Importance identified?
Decision Tree Regressor is used for house price prediction and Gross Domestic Price was found the most important feature even though there is unemployment during the time period selected. 

 



Conclusion
In this approach, we can find the important  features that influence the residential house prices in the US, when we get to use more features than the ones used here. 












