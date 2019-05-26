# House_Price_Prediction

For this project, we were given the dataset from Kaggle https://www.kaggle.com/marklvl/bike-sharing-dataset/home containing information about the houses in King County. The dataset contains 19 house features plus the price and the id columns, along with 21613 observations. The aim of the project is to build a regression model to predict house price with minimal MAPE. 

The following variables are included in the data:

  1. ida:  notation for a house
  2. date: Date house was sold
  3. price: Price is prediction target
  4. bedrooms: Number of Bedrooms/House
  5. bathrooms: Number of bathrooms/House
  6. sqft_living: square footage of the home
  7. sqft_lot: square footage of the lot
  8. floors: Total floors (levels) in house
  9. waterfront: House which has a view to a waterfront
  10. view: Has been viewed
  11. condition: How good the condition is ( Overall )
  12. grade: overall grade given to the housing unit, based on King County grading system
  13. sqft_above: square footage of house apart from basement
  14. sqft_basement: square footage of the basement
  15. yr_built: Built Year
  16. yr_renovated: Year when house was renovated
  17. zipcode: zip
  18. lat: Latitude coordinate
  19. long: Longitude coordinate
  20. sqft_living15: Living room area in 2015(implies-- some renovations) This might or might not have affected the lotsize area
  21. sqft_lot15: lotSize area in 2015(implies-- some renovations)
  

### Conclusion

Since the test dataset does not contain target variable, I partition the train dataset into 80% train_set and 20% test_set. I first build a base model with Linear Regression and later attempted more robust algorithm. I have tried both Random Forest and XGBoost. The tree based model seems to better capture the non linearity aspect of the data. 

Initially, I have a Baseline model with MAPE of 0.25, however, after performing multiple data preparation steps and transformations we achieved a MAPE of 0.124, which proves that our predicting capabilities improved immensely. 


  
