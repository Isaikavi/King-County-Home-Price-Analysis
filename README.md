A Machine Learning Project for Real Estate Valuation

Objectives
  1. Analyze residential real estate in King County, Washington to identify the attributes that most influence house prices
  2. Build predictive models to estimate market value for a Real Estate Investment Trust (REIT). 

Dataset
  Home sales from May 2014 to May 2015, including attributes such as square footage, bedrooms, floors, condition, grade, location, and more.

Actions performed
  1. Cleaned the dataset and handled missing values.
  2. Conducted exploratory data analysis to understand distributions, outliers, and correlations.
  3. Compared several regression approaches (simple, multiple, polynomial, Ridge).
  4. Evaluated each model using R² to measure predictive strength.
  5. Identified the features that most strongly influence housing prices.

Key Results
  Strongest Predictors of Price
  1. Location variables (latitude, longitude, waterfront) are the most influential.
  2. Home quality metrics (grade, view, condition) significantly boost predictive power.
  3. Living area (sqft_living) is important but only explains ~50% of price variation on its own.

  Price Behavior
  1. Homes with waterfront views have dramatically higher prices and more extreme outliers.
  2. Above-ground living space (sqft_above) is positively correlated with price.
  3. Uncommon floor counts (e.g., 3.5, 4 floors) represent unique or unusual properties.

  Model Performance
  Model	                                        R² Score	            Notes
  Simple Linear Regression (sqft_living only)	  ~0.50	                Square footage alone is not enough.
  Multiple Linear Regression (11 features)	    ~0.70	                Adding more features greatly improves accuracy.
  Polynomial Pipeline	                          ~0.75–0.80	          Captures complex relationships; best performance.
  Ridge Regression	                            ~0.69–0.73	          Strong generalization; reduces overfitting.

Conclusion
  1. Machine learning can support real estate investment decisions by revealing the key drivers of price and providing accurate price predictions.
  2. Polynomial models offered the best results, and location-based features proved to be the most critical for valuation.
