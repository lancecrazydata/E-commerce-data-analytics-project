# Build a customer segmentation model

#### The next step is to build a customer segmentation model. A good customer segmentation model can help target the right people with the right marketing strategy.

![image](https://user-images.githubusercontent.com/70103049/112316639-67259f00-8cff-11eb-9b99-f595604a0221.png)

![image](https://user-images.githubusercontent.com/70103049/112316656-6ab92600-8cff-11eb-9e97-891277a97352.png)

#### Only recency and monetary has discernibility as most of users only consume once. We can use recency and monetary to categorize customers into 4 types of membership: platinum, gold, silver, lost. We can take different marketing strategies for different types of members.

![image](https://user-images.githubusercontent.com/70103049/112316756-8290aa00-8cff-11eb-8a77-ef8ac1943ecc.png)


#### According to those 4 types of members, we can calculate lifetime value for each type.

##### Lifetime value =  Customer Value per year * Customer Average Lifespan(years)
##### Customer Value per year = Average Order Value * Purchase Frequency per year
##### Customer Average Lifespan per year = (Last Purchase time – first Purchase time)/365
##### Average Order Value = Total Order Value 365 days / Number of Orders 365 days 
##### Purchase Frequency per year = Number of Orders in 365 days / Unique Customers in 365 days 


![image](https://user-images.githubusercontent.com/70103049/112317231-f16e0300-8cff-11eb-8850-7ddd7a78736f.png)

#### We can see that customers in Gold category have the highest lifetime value.



