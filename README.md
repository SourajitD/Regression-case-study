# Regression-case-study
Regression - Predicting price of pre-owned cars

This project is a case study performed as part of NPTEL Online Certification NOC:Python for Data Science, IIT Madras (Jan-Feb 2023).

Problem Statement and Objective:
- Storm Motors is an e-commerce company who act as mediators between parties interested in selling and buying pre-owned cars.
- For the year 2015-2016, they have recorded data about the seller and car including-
		1. Specification details
		2. Condition of car
		3. Seller details
		4. Web advertisement details
		5. Make and model information
		6. Price
- Storm Motors wishes to devlope an algorithm to predict the price of the cars based on various attribute associated with the car.

Dataset Description:
- The dataset contains 19 columns and 50001 rows.

Variable Description: Numerical-6, Categorial-13
1. dateCrawled (date) - date when the ad first crawled, all field values are taken from this date
2. name (string) - string consisting of car's name, brand, model etc.
3. seller (string) - nature of seller
4. offerType (string) - whether the car is on offer or not
5. price (int) - price on the ad to sell the car
6. abtest (string) - two version of ad
7. vehicleType (string) - type of cars
8. yearOfRegistration (int) - year in which car was registered
9. gearbox (string) - type of gearbox
10. powerPS (int) - power of the car (in HP)
11. model (string) - model type of cars
12. Kilometer (int) - No. of kilometer the car have travelled
13. monthOfRegistration (int) - month of registartion
14. fuelType (string) - type of fuel car use
15. brand (string) - make of car
16. notRepairedDamaged (string) - Status of repairing of daamges if yes damages have not been rectified; if no damage were taken care of
17. dateCreated (date) - date at which the ad at storm motor was created
18. postalCode (int) - postal code of seller
19. lastSeen (date) - when the crawler saw this ad last online

Solution Conceptualization:
1. Identify if data is clean
2. Look for missing values
3. Identify variables influencing price and look for possible relationships between variables
4. Identify outliers
5. Identify if categories with meagre frequencies can be combined
6. Filter data based on logical checks
7. Reduce number of data

Method Identification:
- Linear Regression
- Random Forest

Realization of solution:
- Assumption checks using regression diagnostics
- Evaluate performance metrics
- If assumptions are satisfied and solutions acceptable than model is good
- If performance metrics are not reasonable then a single model is not able to capture the variation in price as a whole
	- In such cases, it would be better to subset data and build seperate models
