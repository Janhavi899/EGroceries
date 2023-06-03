# EGroceries
 
Description	:	Website to order door step delivery of groceries in minimum time from nearby registered shops.
===============================================================================================================
Analysis:
=========
Shops 
shop details (shop name and more)
items that are being sold
address of the shop

Note: Payment is by default cash.
===============================================================================================================
Imp Tech Operations:
====================
1. A Spring boot micro services-
	Service 1: 
   Signup/signin of customers
   API to display near by shops based on location [City and Locality]
   List of items based on the shop to add them to cart
   Show cart items
   Show order summary
   Message to mail and contact number (Order Placed, Order in transit, Order delivered)
   Mail Bill to customer upon order received
   Tracking status
   Handle multiple address
		
	Service 2: 
   Registration/deregistration of shop (Details and address)
   Add and delete items that are meant to be sold
   Customer order summary
   Accept the order
   Decline the order with necessary reason
   Order delivered

2. Database schema:
   Customer
   Shop -> Shop_id (primary key), shop details , ...etc
     -> shop_items [A table having item details binded to shop_id ]
   shop_items (Details of all the items)
   Cart (cart details and summary)
   Orders
   My Order [Map of Customer<Key> with value as (List of that customer's orders)]

3. Tools:
   Backend: Spring Boot Suite, My SQL Workbench, postman, Kafka
   Frontend: Atom, npm, ngnix, (cors chrome extension)

 
Tech Stack:
===========
   Frontend	: 	React js
   Backend		: 	Java - Spring Boot (Mavean)
   Database	:	SQL DB
   MessageQueue:	Kafka

Future Scope:
=============
   Kafka
   Payment Integrations
   AWS integration
