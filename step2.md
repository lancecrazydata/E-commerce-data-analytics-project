# Step 2: Data Cleaning

#### The next step would be data cleaning. The completeness of the datasets needs to be checked first. The time span need to checked in order to match the research boundary. Does the dataset structure look normal? 

![image](https://user-images.githubusercontent.com/70103049/112313197-b36ee000-8cfb-11eb-9a2a-55c8f113fc7a.png)

 ![image](https://user-images.githubusercontent.com/70103049/112313205-b7026700-8cfb-11eb-8ffd-8a34c0b6f214.png)

#### The sales trend from September 2018 to Octorber 2018 dropped suddenly, maybe due to data missing and errors. Therefore, this part of data should be ignored.

#### The missing value (NA) should be checked, too. We can find the missing percentage of “product_id” is only 0.67%, which could be deleted from the relevant samples.

![image](https://user-images.githubusercontent.com/70103049/112313498-05176a80-8cfc-11eb-9536-b30b41c0dbf5.png)


#### Some click-farm transactions should also be excluded for future analysis since it might cause some outliers. However, after “drop_duplicate()”, the maximum number of transactions for a single user is 16, and most of multiple transactions for a single user is below 10, which indicates normal. If we take 12 as the maximum tolerance of multiple transactions for a single user, we can remove the orders which “trans_units” are larger than 12.

![image](https://user-images.githubusercontent.com/70103049/112313658-3728cc80-8cfc-11eb-8f0a-649aef2bd435.png)


#### The next cleaning step is to check if all of the figures are non-negative. Luckily, the number from the data source is all non-negative.

![image](https://user-images.githubusercontent.com/70103049/112313780-5aec1280-8cfc-11eb-98b0-6bd0ef665057.png)

#### The final step of data cleaning is to check the logic of the figures. 

#### The total price of products + freight_value - discount = payment_value

![image](https://user-images.githubusercontent.com/70103049/112313994-9be42700-8cfc-11eb-9531-de091f073324.png)
![image](https://user-images.githubusercontent.com/70103049/112314050-ab637000-8cfc-11eb-924c-efdd1320200a.png)
 
