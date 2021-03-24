# Build a category recommendation system 

#### The final step is to build a category recommendation system with market basket analysis. Recommendation systems are kinds of systems for filtering information which analyse user behaviour data from past times and try to predict the user's preference for items.Market basket analysis determines customer’s purchasing patterns by finding significant relationship among the items which they select in their shopping carts.

![image](https://user-images.githubusercontent.com/70103049/112318076-c3d58980-8d00-11eb-801d-f3c9c80814ad.png)

#### The support index is the occurrence possibility of the particular combination (X, Y). The confidence index measures the possibility of finding Y given X on condition. The lift index is used to calculate the symmetric association between the precedent and the result of the rules extracted. If lift (X, Y) = 1, it is not associated with itemsets X and Y, i.e., they are statistically independent. Lifting values below 1 indicate a negative correlation between itemsets X and Y while values above 1 display a positive correlation. 
 
#### 1. Calculate the support index. We define the minimum support index as 0.1 and then filter the categories whose support index is greater than the minimum.

![image](https://user-images.githubusercontent.com/70103049/112318894-a228d200-8d01-11eb-82bc-507c59d34cde.png)

![image](https://user-images.githubusercontent.com/70103049/112318918-a8b74980-8d01-11eb-88f1-b61c3f488baa.png)

![image](https://user-images.githubusercontent.com/70103049/112318949-afde5780-8d01-11eb-94e5-8de53ebbed4a.png)

#### 2. Filter out the orders which contain more than 2 categories
![image](https://user-images.githubusercontent.com/70103049/112319046-c7b5db80-8d01-11eb-86e7-149b06dd1734.png)
![image](https://user-images.githubusercontent.com/70103049/112319088-d3a19d80-8d01-11eb-899c-15c4f7114273.png)


#### 3. Re-calculate the occurrence frequency for each category and the support index.

![image](https://user-images.githubusercontent.com/70103049/112319164-e5834080-8d01-11eb-89c8-838469ebc5f4.png)

#### 4. Generate the combination of every two categories.
![image](https://user-images.githubusercontent.com/70103049/112319258-fd5ac480-8d01-11eb-9d44-30fad6e0072a.png)

#### 5. Calculate the combinations frequency and support index, and filter out the ones whose support index is greater than the minimum support index 0.2.
![image](https://user-images.githubusercontent.com/70103049/112319393-20857400-8d02-11eb-935a-a23b93a22790.png)
![image](https://user-images.githubusercontent.com/70103049/112319406-2418fb00-8d02-11eb-82bb-6ac0d50bf96e.png)
![image](https://user-images.githubusercontent.com/70103049/112319433-2b400900-8d02-11eb-8766-5d7dc6ffb313.png)

#### 6. Calculate the lift index for each combination and filter out the ones greater than 1.
![image](https://user-images.githubusercontent.com/70103049/112319551-4b6fc800-8d02-11eb-923f-92fb123e06f9.png)
![image](https://user-images.githubusercontent.com/70103049/112319574-50347c00-8d02-11eb-936a-2a67fde5b779.png)

#### 7. Calculate the confidence index for each combination and sort in descending order.

![image](https://user-images.githubusercontent.com/70103049/112319662-65110f80-8d02-11eb-9ee1-8b1f7400763d.png)

#### We can visualize the three index relations. The size of circle represents the support index. The combinations located on the top right corner with larger size means greater for recommendation.

![image](https://user-images.githubusercontent.com/70103049/112319754-7bb76680-8d02-11eb-8c91-9f18537b7d34.png)




