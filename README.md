### Exploratory Data Anaysis
The dataset contains sale transactions from the past year. I analyzed and provided initial insights.

The dataset can be grouped into 3 based on the columns data:

- Order data : These tells us information about the order and shipment, columns inclded are order_id, ship_mode etc.
- Customer data : These contains the customer details and their corresponding address for shipment.
- Product data : Here we have information on the product, their category, quantity and also price.

The dataset contains the following columns:
| Column       | Description                                                         |
|---------------|----------------------------------------------------------------------|
| order_id      | A unique identifier for each order.                                  |
| product       | The name of the product purchased.                                   |
| quantity      | The number of units of the product sold in the order.                |
| price         | The price of a single unit of the product.                           |
| order_date    | The date the order was placed (format: YYYY-MM-DD).                  |
| customer_id   | A unique identifier for the customer.                                |


#### Descriptive Statistics
<img width="870" height="362" alt="image" src="https://github.com/user-attachments/assets/00bce076-44f4-4596-bc63-81476c8dbe2c" />
 From the numerical columns we can see the following :
 
 - Sales: The price for the products ranges from min of 0.444 to the max of 13,999.96 . These tells us that we have both relative cheap and expensive products bought. 75% of the orders are products with price around 205. These tells us that we have few bulk or expensive orders.
 - Quantity: We have a mean of 3.766908, these tells us that the average quantity per order is approximately 4 units. The minimum order is 1 unit and 75% of orders are 5 units. These suggests that most customers buy small or moderate quantities. While the max order is 14 units.
 - Discount : Some products don't have discount (min = 0). While the average discount is around 15.65%. The upper quartile or 75% of orders have 20% discount. Some discounts can go up to 80%.
 - Profit : The average profit is 28.21, the min and max profits are -3839.9904 and 6719.9808. These suggest relatively large lossess and large profits. The large losses could be due to inaccurate pricing or even huge discounts.
 - Total Sale : The average total sale per order is 1082.37 which is way greater than the median at 184.42 and also greater than the 75% of the total sale. The max is 56782.648. These suggests that small number of expensive orders move the revenue up.

- Also there is an average of 4 days between the order date and shipment date.


#### Insights and Recommendation

 - Top 5 products by revenue : 40% are under the category Technology, the other 40% under Office Supplies and the remaining 20% under Furniture.
- Top 5 products by quantity sold : 40% under Technology, the other 40% under Furniture and the remaining 20% under Office supplies. Therefore we can see that for both revenue and quantity sold (top 5), the products are from 3 categories (Technology, Furniture, and Office supplies).
- From the descriptive statistics, we saw that we have some huge losses as well as large profits. I recommend reducing the discount percentage for some products to ensure consistent pricing. We should also review the profit margins for some products.
- Also from the descriptive statistics, we saw that majority of orders are in small or moderate quantites. I recommend using incentives like cuopons or bundles to encourage relatively large quantity order.
