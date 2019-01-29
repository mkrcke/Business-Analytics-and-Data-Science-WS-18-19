# Business-Analytics-and-Data-Science-WS-18-19
Code Submission Date: 12.02.2019

Paper Submission Date: 18.03.2019

Input:
BADS_WS1819_known
BADS_WS1819_unknown

1. Data Prep
- all values to.lowercase to prevent distinction of same values. 
- order_item_id is a unique identifier of order item. doesn't matter REMOVE
- order_date and delivery_date should be coerced into a date diff variable
- item_id is a factor. lots of small values - maybe discretize into frequency of purchase.
- item_size factor. probably not relevant on it's own REMOVE
- item_color probably not relevant on it's own REMOVE
- brand_id is a factor. some different in test / training, test set should be scaled down. see item_id note
- item_price numeric, but in test set there are higher values. handle 0 values
- user_id is a factor. see item_id note
- user_title is a factor but high class imbalance, follows same distribution and appears to be decent signal
- user_dob is date of birth. consider discretizing and removing bad values (impute?)
- user_state is a factor. follows same distribution and appears to be decent signal
- user_reg_date is a date. consider changing to "length of account" and "time between open and order"
- basic colors (e.g. black, white, navy) are correlating with lower return probability, bc uncertainty regarding color is reduced
- basic sizes (m) are correlating with lower return probability, bc uncertainty regarding color is reduced
- "trends" --> products with a high purchase rate
- 

2. Transforming Variables
3. Building a model
4. Model Assessment

Additional Modeling Challenge: Use a genetic algorithm to minimize costs directly using a linear classifier. 
