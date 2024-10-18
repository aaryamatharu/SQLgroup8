# Team 8 Mist 4610 Group Project 1
# Team Name:
4610Fa24Group8
# Team Members:
1. Aarya Matharu @aaryamatharu
2. Anica Singh @anicasingh
3. Murray Freeman
4. Nick Dortzbach @dortzenbacher
5. Jonah Kilpi @Jonah-Kilpi
# Problem Description:
Our project involves modeling and developing a relational database to represent the operations of Procter & Gamble (P&G), a leading global consumer goods company. The core entity in our model is the Product Line, representing the various lines P&G manufactures and distributes across different markets. P&G collaborates with various suppliers, retailers, and customers that are crucial to their business model. Our aim is to accurately model these relationships, create sample data, and populate the entities accordingly. In addition, we will perform queries on this data to extract valuable business insights, such as product sales performance, supply chain efficiency, and the impact of marketing efforts. These insights will enable us to make data-driven decisions that enhance operational effectiveness and contribute to the overall growth and profitability of the business.
# Data Model:
Our project focuses on developing a data model based on the operations of Procter & Gamble. In our data model, the core entity revolves around the ProductLine, representing the diverse lines of products that Procter & Gamble (P&G) manufactures. Each ProductLine consists of various products and is categorized by attributes such as the product line's name, category, and revenue. Each ProductLine is linked to a specific Brand, showing a many-to-one relationship since multiple product lines may fall under one brand, such as Tide, Gillette, or Pampers. The Brand entity consists of attributes related to name, category (home, laundry etc.), revenue, and description. 

ProductLine is also connected to the Warehouse entity, which represents storage facilities where products are kept. The warehouses are detailed with attributes like location, size, city, and contact information, ensuring that we can track where products are stocked. Additionally, ProductLine has a relationship with Supplier, representing the companies that provide the products for these product lines. Each supplier includes details like name, address, and phone number.

The ProductLineSaleChannel entity serves as an associative entity, linking ProductLine with Retailers, representing the sales channel through which product lines are sold. Attributes here include the number of stores a retailer operates, the start date of their partnership. This provides us with vital information about our retailer partnerships. The Retailer entity reflects the various retailers that purchase from P&G product lines. The attributes we deemed crucial to label here include retailer name, number of stores, and overall revenue.

The Product entity ties back to the ProductLine as a one-to-many relationship since a product line can have multiple products but a product can only relate to one product line. It holds information like the product’s name, price, weight, and status (in stock/out of stock). This allows us to track every individual item within a given product line, and their respective orders by customers are recorded in the CustomerOrder entity.

CustomerOrder captures key order data, including the quantity ordered, order price, order date, and shipping details. It has a many-to-one relationship with products because customers have to order products separately from each product line but can have multiple orders. Customers are represented in the Customer entity, with attributes such as customer name, email, and phone number stored. Customer feedback on orders is collected in the CustomerFeedback entity, which ties feedback directly to specific orders and includes feedback details like description, type (positive or negative), and date.

This structure allows a comprehensive view of how P&G’s various product lines interact with brands, suppliers, warehouses, and retailers, while also tracking customer interactions and feedback, providing insights into the lifecycle of each product line.

<img width="688" alt="PNG image" src="https://github.com/user-attachments/assets/ef84cbae-3691-445d-be6c-7fb8e76b7427">


# Data Dictionary:
# Queries
# Database information:
Name of the database : ns_4610Fa24Group8
