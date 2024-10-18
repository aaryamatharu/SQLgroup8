# Team 8 Mist 4610 Group Project 1
# Team Name:
4610 Fa24 Group8
# Team Members:
1. Aarya Matharu [@aaryamatharu](https://www.github.com/aaryamatharu)
2. Anica Singh [@anicasingh](https://www.github.com/anicasingh)
3. Murray Freeman [@murrayfreeman](https://www.github.com/murrayfreeman)
4. Nick Dortzbach [@dortzenbacher](https://www.github.com/dortzenbacher)
5. Jonah Kilpi [@Jonah-Kilpi](https://www.github.com/Jonah-Kilpi)
# Problem Description:
Our project involves modeling and developing a relational database to represent the operations of Procter & Gamble (P&G), a leading global consumer goods company. The core entity in our model is the Product Line, representing the various lines P&G manufactures and distributes across different markets. P&G collaborates with various suppliers, retailers, and customers that are crucial to P&G's business model. Our aim is to accurately model these relationships, create sample data, and populate the entities accordingly. In addition, we will perform queries on this data to extract valuable business insights, such as product sales performance, supply chain efficiency, and the impact of marketing efforts. These insights will enable us to make data-driven decisions that enhance operational effectiveness and contribute to the overall growth and profitability of the business.
# Data Model:
Our project focuses on developing a data model based on the operations of Procter & Gamble. In our data model, the core entity revolves around Product Lines, representing the diverse lines of products that Procter & Gamble (P&G) manufactures. Everything from Tide Pods to Gain Flings. Each product line is categorized by attributes such as the product line's name, category, and revenue. Each product line is linked to a specific Brand, showing a many-to-one relationship since multiple product lines may fall under one brand, such as Tide, Gillette, or Pampers. The Brand entity consists of attributes related to name, category (home, laundry etc.), revenue, and description. 

ProductLine is also connected to the Warehouse entity, which represents storage facilities where products are kept. The warehouses are detailed with attributes like location, size, city, and contact information, ensuring that we can track where products are stocked. Additionally, ProductLine has a relationship with Supplier, representing the companies that provide the products for these product lines. Each supplier includes details like name, address, and phone number.

The ProductLineSaleChannel entity serves as an associative entity, linking ProductLine with Retailers, and representing the sales channel through which product lines are sold. Attributes here include the number of stores a retailer operates, the start date of their partnership. This provides us with vital information about our retailer partnerships. The Retailer entity reflects the various retailers that purchase from P&G product lines. Big stores such as Target and Walmart that house P&G products on their shelves. The attributes we deemed crucial to label here include retailer name, number of stores, and overall revenue.

The Product entity ties back to the ProductLine as a one-to-many relationship since a product line can have multiple products but a product can only relate to one product line. It holds information related to the specific instance of a product such as its  name, price, weight, and status (in stock/out of stock). 

Customers purchase directly from P&G using online order methods. CustomerOrder captures key order data, including the quantity ordered, order price, order date, and shipping details. It has a many-to-one relationship with products because customers have to order products separately from each product line but can have multiple orders. Customers are represented in the Customer entity, with attributes such as customer name, email, and phone number stored. Customer feedback on orders is collected in the CustomerFeedback entity, which ties feedback directly to specific orders and the customer includes feedback details like description, type (positive or negative), and date. This information allows us to update our product lines and continue growing our sales.

This structure allows a comprehensive view of how P&G’s various product lines interact with brands, suppliers, warehouses, and retailers, while also tracking customer interactions and feedback, providing insights into the lifecycle of each product line.

<img width="876" alt="PNG image" src="https://github.com/user-attachments/assets/38014aaa-0944-46cf-a63c-bbce7fe38773">



# Data Dictionary:
# Queries

![Screenshot 2024-10-18 085118](https://github.com/user-attachments/assets/6ec4126e-be48-45fa-86fe-31091ce0ab34) 

<img width="601" alt="Screenshot 2024-10-18 at 12 48 05 PM" src="https://github.com/user-attachments/assets/4a6183cc-6012-412e-b983-b36aa3c846ba">


<img width="592" alt="Screenshot 2024-10-18 at 12 48 24 PM" src="https://github.com/user-attachments/assets/6a47b283-8faa-4e6d-b51c-4fe0ec7b036d">

<img width="607" alt="Screenshot 2024-10-18 at 12 49 21 PM" src="https://github.com/user-attachments/assets/cc05f989-d85e-41df-b6a7-2b6357c472ab">

<img width="597" alt="Screenshot 2024-10-18 at 12 49 40 PM" src="https://github.com/user-attachments/assets/7c645fd1-c4a3-4b0a-8954-caf9b975269a">

<img width="593" alt="Screenshot 2024-10-18 at 12 50 00 PM" src="https://github.com/user-attachments/assets/b3cc2869-8539-4955-9e64-68e11be86a91">

<img width="606" alt="Screenshot 2024-10-18 at 12 50 16 PM" src="https://github.com/user-attachments/assets/cc2de2ff-103f-4eba-b090-52ab99efe8f0">

<img width="589" alt="Screenshot 2024-10-18 at 12 50 38 PM" src="https://github.com/user-attachments/assets/399d3f28-b9b0-42f3-b273-c3d636a99742">

<img width="604" alt="Screenshot 2024-10-18 at 12 51 07 PM" src="https://github.com/user-attachments/assets/4f9153dd-cc64-43b6-9eef-575e39eda70b">

<img width="561" alt="Screenshot 2024-10-18 at 12 51 29 PM" src="https://github.com/user-attachments/assets/7134d70a-99c2-4dea-a5d1-8d86599512fc">

<img width="580" alt="Screenshot 2024-10-18 at 12 52 01 PM" src="https://github.com/user-attachments/assets/3bc6259e-c39d-4b60-99d9-4c1ab3911be8">


# Database information:
Name of the database : ns_4610Fa24Group8

Additional information: All queries listed above are marked in the database using stored procedures, which can be called using CALL TP_Qx(); for each query number. 
