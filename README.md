[![wercker status](https://app.wercker.com/status/1c2980fb853831004b2a4919859f3bda/s/master "wercker status")](https://app.wercker.com/project/byKey/1c2980fb853831004b2a4919859f3bda)

source: http://www2.stat.duke.edu/~cr173/Sta523_Fa16/hw/hw2.html

## Data

For this assignment you will be working with a synthetic data set of sales records for lego construction sets. We will assume that the original data was stored in a JSON format but a colleague has managed to import it into R as a list of lists data structure. The code below will load a copy of the object, called sales, into your R environment.

load("lego_sales.RData")
The original JSON file is also available, as lego_sales.json in your hw2 repo, if you would prefer to examine a text based representation of the data.

The data is structured such that each entry in the top list represents a different purchaser. These list entries contain basic information about the purchaser (name, age, phone number, etc.) as well as their purchase history. Everyone in the data set has purchased at least one lego set but most have purchased more than one. The purchase histories are stored in the purchases element which is also a list of lists. Each entry within the purchases list reflects a different lego set which the customer purchased. Note that the customer may have purchased more than one copy of any particular set, this number is stored as Quantity within the purchase record.



## Task 1 - Tidying the data
Our first task is covert the sales object into a tidy data frame. Each row represents a separate purchase of a lego set by an individual and the columns should correspond to the keys in the JSON data. Duplicate columns will be avoided as much as possible and no data slost / ignored in the conversion.



## Task 2 - Processing the data
This task will involve answering the following questions about that data that will involve manipulating and summarizing the data frame we created in Task 1:

What was the most common first name of purchasers? Last name?

What are the five most popular lego sets based on these data?

Which five customers have spent the most money so far and how much have they spent?

Which lego theme has made the most money for lego?

Do men or women buy more lego sets (per person) on average?

What are the five most popular hobbies of lego purchasers?

How many total pieces have been purchased from lego by these customers?

What state has spent the most money on legos? Hint - customer area codes may prove useful for this.
