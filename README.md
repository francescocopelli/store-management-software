[![GitHub license](https://img.shields.io/github/license/francescocopelli/store-management-software?style=for-the-badge)](https://github.com/francescocopelli/store-management-software/blob/main/LICENSE)

# Store Management Software
Created by Francesco Copelli and Stefan Yoshovski on July 2021 during the course "Graphic Interfaces and Event Programming" at University of Calabria (Rende, Italy)

# Table of Contents
<details>
  <summary>Show</summary>
  
* [Snapshots and Demo](#snapshots)
* [Introduction](#introduction)
* [Features](#features)
* [Technology Used](#technology-used)
* [Demo Credentials](#demo-credentials)
</details>

## Snapshots
<details>

Login: ![Login](https://github.com/francescocopelli/store-management-software/blob/main/Snapshots/login_light.jpg)
Register: ![Register](https://github.com/francescocopelli/store-management-software/blob/main/Snapshots/register_light.jpg)
- More Snapshots: https://github.com/francescocopelli/store-management-software/tree/main/Snapshots

</details>

## Introduction
The program is based on a Client-Server architecture that accesses a remote database. The application was designed to have two roles, the Customer and the Shop Manager, each of which has access to different functions. During the registration phase the user will automatically be registered as "Customer".

## Features
-	Sending E-mails: When updating an order status, the customer will receive an e-mail and the customer can send an email to the admin through the dashboard cards.
-	Password Generation: Each user can request a new password through the Forgot Password Page, which wll be sent via email to the user.
-	Implemented Dark Mode and possibility to choose the mode of the theme color between LIGHT, DARK, AUTO. The preference will be stored for the next time you sign in.

 ### Customer
 -	Dashboard: Welcome card with shortcuts to the Settings Page, support card for sending e-mail to staff and useful statistics such as outgoing money in the current month, orders and many more..
-	Products: A view of all available products with the possibility to add them to the Shopping Cart
-	Shopping Cart: Shows all products in the user's cart. The products in the cart are available for 30 minutes, after that the cart session will expire due to restore unwanted product so the quantities in the inventory are increased. The program check every minute if the products in the cart are still reserved for the current user otherwise it will remove them from the cart.
-	Checkout: By entering data such as address, phone number the order will be placed (the order does not require a real payment).
-	Orders: The history of all orders placed, the status of the order and the last note sent to the customer 
-	Settings: Change password and change personal information.
 
 ### Shop Manager
-	Dashboard: Welcome card with statistics such as online users, registered users, total orders, orders to be shipped, total products and many more..
-	Inventory of products: Create, Read, Update, Delete of products
-	Product Categories: Create, Read, Update, Delete ofCategories. 
-	Orders: Read, Update, Delete of Orders. Possibility to edit the Status of an order that will affect statistics and dashboard cards; if the order status is changed, an e-mail will be sent to the customer.
-	Statistics: Pie chart of the most sold products and bar chart related to earnings of a specified period of the year
-	Users : Create, Read, Update, Delete of Users. 
-	Settings: Change password and personal information. It's possible to configure some store settings such as the Store Name and to configure the mail server.

## Technology Used
- Java (jdk 15.0.2)
- JavaFX and SceneBuilder (8.5.0)
- jfoenix, animateFX, controlsfx, fontawesomefx (libraries for GUI components)
- CSS
- PHP (used for a script that has been written to reserve customers' carts for 30 minutes)
- Database Connection Pool (for better performance)
- External Mail Server
- Sentry (for Logging System for monitoring errors)

## Demo Credentials
- Admin (email: admin@gmail.com - password: prova123)
- Customer (email: elon@gmail.com - password: prova123)
