# Fraud_analysis_by_analysing_data
You are a data analyst and your client has a large ecommerce company in India (let’s call it X).
X gets a thousand orders via their website on a daily basis and they have to deliver them as fast
as they can. For delivering the goods ordered by the customers, X has tied up with multiple
courier companies in India as delivery partners who charge them some amount per delivery.
The charges are dependent upon two factors:
● Weight of the product and the Price of the product.
● Distance between the warehouse (pickup location) and customer’s delivery address
(destination location)
On an average, the delivery charges are Rs. 100 per shipment. So if X ships 1,00,000 orders
per month, they have to pay approximately Rs. 1 crore to the courier companies on a monthly
basis as charges.
As the amount that X has to pay to the courier companies is very high, they want to verify if the
charges levied by their Delivery partners per Order are correct.
Input Data
Left Hand Side (LHS) Data (X’s internal data spread across three reports)
● Website order report- which will list Order IDs ,various products (SKUs) part of each
order and the Payment Type of the Order ( COD or Prepaid). Order ID is common
identifier between X’s order report and courier company invoice
● Warehouse pincode to All India pincode mapping -(this should be used to figure out
delivery zone (a/b/c/d/e) and during analysis compare against one reported by courier
company in their CSV invoice per Order ID
● SKU master with gross weight of each product. This should be used to calculate total
weight of each order and during analysis compare against one reported by courier
company in their CSV invoice per Order ID. The courier company calculates weight in
slabs that is applicable for that delivery zone, so first you have to figure out the total
weight of the shipment and then figure out applicable weight (based on zone’s weight
slab).
