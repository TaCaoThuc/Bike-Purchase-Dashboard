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
<img src="image/Screenshot preview.png">
## Cleaning Data
### Remove duplicates
<img src="image/Screenshot remove duplicates 1.png">
<img src="image/Screenshot remove duplicates 2.png">

### Find and Replace 
The values in the Marital Status column and Gender column are abbreviated, which can cause ambiguity in visualizations. Therefore, we need to use Find and Replace feature to replace the abbreviations with the full forms. 

In the Marital Status column, change 'M' to 'Married' and 'S' to 'Single':
<img src="image/Screenshot find and replace 1.png"> 

Next, in the Gender column, change M to Male and F to Female:
<img src="image/Screenshot find and replace 2.png"> 
<img src="image/Screenshot find and replace 3.png">
### Change currency format
Change the data type of the Income column to Currency and remove decimal:

<img src="">
<img src="">
### Divide people into age groups
There are numerous ages in the dataset, which can make it difficult to visualize. To solve this, we need to divide people into three age groups: Adolescent (under 31 years old), Middle Age (31-55 years old), and Old (more than 55 years old). To do this we will use the NESTED If function.

Create a column next to Age named Age Brackets and insert the following formula in the first row:
<img src="">

Then apply for all cells of the column:
<img src="">
## Creating Pivot tables and Pivot charts
Create a new sheet, insert Pivot table using cleaned data.

Create a pivot table to summarize bike purchase by gender and average income. Then create a bar chart to visualize it: 
<img src="">
<img src="">

Create another pivot table to summarize bike purchase by commute distance:
<img src="">
<img src="">

Go back to the dataset, change 10+ Miles to “More than 10 miles” so that rows’ values are in ascending order. Next, create a line graph to visualize it:
<img src="">
## Creating Dashboard
Copy and paste 3 charts into a new sheet then insert Slicers to allow readers filter people by Marital Status, Region, Education and Number of cars owned:

<img src="">
<img src="">

Connect 4 slicers to all 3 Pivot charts:
<img src="">

Design the dashboard:
<img src="">

## 
Some general insights that can be seen from the dashboard:
-	Individuals with higher income levels are more likely to purchase a bike.
- People in the Middle Age group are more likely to purchase a bike than those in other age groups.
- The likelihood of bike purchase decreases as the distance of people's commutes increases
More insights can be discovered using filters, according to the purposes of the dashboard viewers.


















