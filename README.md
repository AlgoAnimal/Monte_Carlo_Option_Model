# Monte_Carlo_Option_Model
Uses statistical models to run simulations on American options and predicts a price given a time to expiry. 

To change model parameters, please go to the 'run_model' function at the bottom. Parameters that are changeable are:
- universe: What stocks you wish to analyze
- option_premium: What is the strike price? Note that this is in relation to the stock's current price, so -0.1 would be a strike price that is 90% of the stock's current price
- T: Time to expiry in years
- n_batches: How many complete monte-carlo simulations to be run
- Start, end: The training range of the model. Note that the algorithm will begin predicting option prices from the 'end' date. So if the end date is 2025-01-01, it will predict the option price from there. So if T = 1/52, then the option's expiry date is one week from 2025-01-01

Stock prices are sourced from the yFinance library. Note that data may not be completely up to date. Use cautiously, especially in times of high economic volatility.
