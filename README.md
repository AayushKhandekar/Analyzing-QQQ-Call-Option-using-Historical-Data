# Analyzing-QQQ-Call-Option-using-Historical-Data

### Project Overview
- Understanding basics of Options.
- Understanding In-the-money, Out-the-money, At-the-money.
- Calculating Intrinsic Value, Profit/Loss
- Calculating Profit/Loss if Option was purchased on start date and sold at expiry.


### Data, Assumptions and Considerations
- QQQ 1 year data from `start_date = 2023-05-20` to `expiry_date = 2024-06-20` 
- strike_price = 420
- premium = 10
- option_type = call
- Assumption: Option was purchased on start_date

### Results

We figure out if the underlying asset is In-the-money, Out-the-money or At-the-money.

Then we calculate the Intrinsic Value of the asset. Intrinsic value is the amount by which an option is In-the-money. 

After that, we calculate the Profit/Loss and the Net Profit/Loss which is the difference of the Profit/Loss and the premium paid.

All the above values are calculated and presented in the image of the dataframe below.

![Options-Data](/Images/Options-Data.png)

The below plot visualizes the intrinsic in-the-money value for QQQ between the start date and the expiry.

![Options-In-the-Money-Plot](/Images/Options-In-the-Money-1.png)

Comparison between the intrinsic value and the price of the underlying asset. An intrinsic value of zero indicates that the strike_price is greater compared to the current price of the asset and hence, the option is not in-the-money yet.

![Options-Data](/Images/Options-Intrinsic-Value-vs-Stock-Price.png)

The lines in the below plot show the effect of the premium charged. 

![Options-Data](/Images/Options-Profit:Loss.png)

If the call option was purchased on 2023-05-20 and sold at expiry, we expect a profit of 65.20999145507812 per share.

