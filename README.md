Part 1
All USDT pairs in Binance - attached as CSV
All categories in crypto - attached as CSV
Fetch all coins by categoryID from https://www.coingecko.com/en/api/documentation
delete all coins received in Step 3 which are not present in Step 1.
Map all coins in Step 1 to their categories. Many to many relationships which means, multiple coins can have multiple categories
Every category is the bucket which has N number of coins
Part 2
Fetch all coins' last 6 months' data on a 24H timeframe from Binance API - store it in DB
Calculate daily %change of all coins - (current close-previous close)/previous close
Group coins by category 
Category 1 - Coin 1, coin 2, coin 3, coin 4
Category 2 - Coin 5, coin 6, coin 7, coin 1
Category 3 - Coin 1, coin 4
Get the average of % change on a category basis for the last 6 months
Make a line chart plotting all categories' last 6 months' data
Part 3
we are monitoring daily % change on that category level and getting RS of the bucket
We are also monitoring the RS of coins on global and bucket level
