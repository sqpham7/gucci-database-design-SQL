# gucci-database-design
## Project Overview
Presents a comprehensive relational database design for Gucci, modeling the core business operations of a global luxury fashion brand. The database integrates key functional areas including employees, customers, products, stores, manufacturing locations, orders, payments, and product lines to support both online and in-store retail activity.
## Database Scope & Objectives
The database is designed to create a logical and connected data structure across Gucci’s operations. By integrating employee records, inventory, customer purchases, and store data, the system allows managers to:

• Track inventory levels and pricing accuracy

• Locate employees across offices and retail stores

• Analyze customer purchasing behavior

• Maintain consistency between online and in-store transactions

##
After forward engineering the databases into MySQL, 5 associative tables were created to connect the tables with a many-to-many relationship. This will allow us  to make joint queries between these tables and connect the data between them. 
## Business Questions

1. Gucci wants to give extra special Christmas bonuses to their employees over 40 years old. They decided to give each of these employees a 10% raise. The company would only really use this query when handing out raises, most likely once a year.
<img width="428" height="286" alt="Screenshot 2026-02-11 at 10 35 26 AM" src="https://github.com/user-attachments/assets/827b0d1e-0be2-4c9d-aa76-b3f67416cb1a" />

2. Gucci wants to know the average price of each of their products. This is a good query to have to make sure their prices remain affordable. 
<img width="225" height="297" alt="image" src="https://github.com/user-attachments/assets/9be428cf-4e17-49b4-ad52-e0328f53dec8" />

3. Gucci wants to know which customers order a high amount of products, specifically which customers order more than 5 of one product in one order. This query could help the marketing team in sending out coupons and deals for loyal customers who order a high amount of product and make sure they take efforts to secure these customers as long time buyers.
   <img width="348" height="256" alt="image" src="https://github.com/user-attachments/assets/a16b6684-041b-47f4-bce7-88155c0d69d9" />


4. Gucci wants to know which of its employees work out of the Florida offices and stores? They have a conference coming up in Miami and want to know which employees are closest to send and which stores to pull product out of.
<img width="481" height="266" alt="image" src="https://github.com/user-attachments/assets/d792741f-740f-41f8-b24d-7a582c2ef90b" />

5. Gucci wants to know which product is the most expensive? They want to try and increase sales for this product to increase revenue.
<img width="366" height="249" alt="image" src="https://github.com/user-attachments/assets/1fe3179f-039b-4d27-b5b1-809737866ad9" />



