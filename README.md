# Superstore Dataset Exploration
## by Goodrich Okoro


## Dataset

>> Dataset containing Sales & Profit of a Superstore. This dataset can be found on [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final?select=Sample+-+Superstore.csv)

>There are 9,994 entries of product ordered with 20 fields that give  details about the product such as ship date, ship mode, region, product name, sales, quantity, profit, e.t.c.,There a five (5) categorical fields, ship mode being one of it is a ordered categorical type. Only four fields are numeric in nature, sales, quantity,discount, and profit.

>**Metadata**

    Row ID => Unique ID for each row.
    Order ID => Unique Order ID for each Customer.
    Order Date => Order Date of the product.
    Ship Date => Shipping Date of the Product.
    Ship Mode=> Shipping Mode specified by the Customer.
    Customer ID => Unique ID to identify each Customer.
    Customer Name => Name of the Customer.
    Segment => The segment where the Customer belongs.
    Country => Country of residence of the Customer.
    City => City of residence of the Customer.
    State => State of residence of the Customer.
    Postal Code => Postal Code of every Customer.
    Region => Region where the Customer belongs.
    Product ID => Unique ID of the Product.
    Category => Category of the product ordered.
    Sub-Category => Sub-Category of the product ordered.
    Product Name => Name of the Product
    Sales => Sales of the Product.
    Quantity => Quantity of the Product.
    Discount => Discount provided.
    Profit => Profit/Loss incurred.
    
> I renamed all columns in the data to lowercase and used underscore in place of space or dash, this was done for easy accessing of the columns when coding. I changed the data type of order date and ship date to datetime. I made ship mode, category, region, segments and sub-categories categorical data type.

## Summary of Findings

>**Office Supplies Category**
The Office Supplies category is the most ordered product with over 6,000 count, mostly bought in the west. Sadly, this high count did not contribute much to the sales generated. A bar chart was plotted and it depicts that Office Supplies generate the least average sales (below $150) compared to others that have over $300. 

>**Technology Category**
Technology category is the least ordered product(count below 2,000) and south region buyers in the south region purchase few of this product. Though being the least ordered product this category generated the highest sales (average of $500), and its profit is the highest too (above $70) compared to other categories that their average profit is not up to half its own.

>**Furniture Category**
Total product purchased from this category falls between 2,000 and 2,500. Amongst the three categories, Furniture is the second category with high sales (average between $300 and $400). Surprisingly, it generated the lowest profit (below $20)

>Products ordered to the South are the lowest compared to other regions. South made the highest sales but did not make the highest profit.
>
>The region with the highest purchase is the West. West did not make the highest sale but it made the highest profit as a region
>
>The Central region purchases more Office supplies products. This region generates the lowest profit (average below $20) and it was later discovered that most of the state with loss falls in this region.
>
>We know that Technology generated the most profit but the most contributor to this was the East region. East generated an average profit of approximately $89 from the Technology category. 

>In the sub-category, Phones from technology category generated the highest sales (above $33K) followed by Chairs (approximately $33K) from furniture category. Meanwhile, Fasteners in the office supplies category generate the lowest sales(below $3.5K).

>Higher discount seems to be associated with products generating loss. A scatter plot was plotted and it depicts that the higher the loss, the higher the discount.

>When looking at the Segment of the data, Consumers make the most purchase of products and Home Office the least with Corporate in-between. Product from Technology category generates the highest sales amongst segments and Home Office in the South region happens to be the segment with this high sales. Corporate segment in the west region seems to generate neither profit or loss from Office Supplies category

>When considering the data of the 10 states with loss (negative profit) only, a heatmap depicts that Office Supplies category generates the least average sales across all states. Another heat map shows that the majority of the category had loss across each state which is no surprise since we are looking at states with loss. But the loss of Ohio stood out because it was the highest, a loss of approximately -$124

## Key Insights for Presentation

>I will start with the distribution of sales and profit, then proceed to the most ordered product. I will go on to check average sales and profit in each category and region after which we will see which customer segment is producing profit amongst the category. Then I will look at states that are generating loss.

>While arranging the above for presentation. I will set titles to plots without any, then reset the ticklabels if necessary and add dollars symbols to the heatmap for good annotation. I will make sure all colors are used accurately, both for qualitative and categorical variables.