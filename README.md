# Bike-Purchase-Dashboard
## Introduction
The aim of this project is to analyze and visualize a dataset containing information about 1000 individuals residing in Europe, Pacific, and North America. This dataset includes their demographic details and their bike purchasing status, with the objective of deriving insights into factors influencing their decision to purchase a bike. The initial steps involved cleaning the data by eliminating duplicates, utilizing Find and Replace techniques, and addressing formatting inconsistencies and using Nested If function. Following this, pivot tables and pivot charts were generated to summarize and visually represent the data. Lastly, a comprehensive dashboard was constructed using the pivot charts and slicers so that viewers can interact and gain more insights about the data.
The dataset contains following columns:
- ID: IDs of people in the dataset
- Marital Status: "Single" (S) or "Married" (M).
- Gender: "Male" (M) or "Female" (F).
- Income: Individual earnings in USD
- Children: Number of children.
- Education: Educational level.
- Occupation: Type of work.
- Home Owner: Home ownership ("Yes" or "No").
- Cars: Number of owned cars.
- Commute Distance: Distance traveled to commute.
- Region: Geographical location.
- Age: Individual age.
- Purchased Bike: Bike purchase ("Yes" or "No").
  
A preview of the dataset:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/930de8ad-8d13-47b8-93bf-3fa3db1df383)
## Cleaning Data
### Remove duplicates
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/308650bb-d711-4c1f-99d6-0721d6f04afa)
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/af502991-f70b-4c58-a247-48aa07903cbe)
### Find and Replace 
The values in the Marital Status column and Gender column are abbreviated, which can cause ambiguity in visualizations. Therefore, we need to use Find and Replace feature to replace the abbreviations with the full forms. 

In the Marital Status column, change 'M' to 'Married' and 'S' to 'Single':
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/41361ab0-0172-4f0c-bbc4-b196812ed3e5) 

Next, in the Gender column, change M to Male and F to Female:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/c731edc3-db42-40bb-a503-2dd34f4f68ef) 
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/654a6c44-888d-4544-89f1-683f57030f6d)
### Change currency format
Change the data type of the Income column to Currency and remove decimal:

![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/cbb619bb-a55c-460c-955b-cb430232c079)
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/6b2685b7-8274-4bba-8d84-7a1db5e63614)
### Divide people into age groups
There are numerous ages in the dataset, which can make it difficult to visualize. To solve this, we need to divide people into three age groups: Adolescent (under 31 years old), Middle Age (31-55 years old), and Old (more than 55 years old). To do this we will use the NESTED If function.

Create a column next to Age named Age Brackets and insert the following formula in the first row:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/0b9b27a0-2e82-4ead-bf3a-1b98e725f2e6)

Then apply for all cells of the column:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/fbbfc611-61f5-476c-968a-df8e8c1aa6d2)
## Creating Pivot tables and Pivot charts
Create a new sheet, insert Pivot table using cleaned data.

Create a pivot table to summarize bike purchase by gender and average income. Then create a bar chart to visualize it: 
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/8889baab-7b14-45c9-9a91-c6ad02d78876)
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/31231749-5391-4a97-8d99-b96fed0fec9e)

Create another pivot table to summarize bike purchase by commute distance:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/9949f87b-d08c-4ac9-ab75-1e85b3f120e1)
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/81705046-b1d1-449c-9eaa-dbe08339fc7a)

Go back to the dataset, change 10+ Miles to “More than 10 miles” so that rows’ values are in ascending order. Next, create a line graph to visualize it:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/29e92522-8fb8-423d-b911-e0572b4de08b)
## Creating Dashboard
Copy and paste 3 charts into a new sheet then insert Slicers to allow readers filter people by Marital Status, Region, Education and Number of cars owned:

![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/774d0e42-2e3f-4411-b7fb-fb0567724b24)
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/52a737f3-b2ad-4bf1-b19b-be1d65942a54)

Connect 4 slicers to all 3 Pivot charts:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/10986e89-b917-4ca5-a196-a8eb723a1df0)

Design the dashboard:
![image](https://github.com/TaCaoThuc/Bike-Purchase-Dashboard/assets/142728022/7ef2baec-1aeb-4680-ad82-0f0e5f774c17)

## 
Some general insights that can be seen from the dashboard:
-	Individuals with higher income levels are more likely to purchase a bike.
- People in the Middle Age group are more likely to purchase a bike than those in other age groups.
- The likelihood of bike purchase decreases as the distance of people's commutes increases
More insights can be discovered using filters, according to the purposes of the dashboard viewers.


















