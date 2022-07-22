# Project Plan

Pod Members: **Adriana Morales, Cynthia Delira, Michelle Fox-Romero, Monica Kirabo**

## Problem Statement and Description

Insert the latest summary of your problem statement and app description.

Problem statement: Many people find difficulty in looking for specific clothing items and must travel from shop to shop, either online or in person, just to see what kinds of things are in store. An upward trend in fast fashion purchases has also increased environmental and energy costs due to long shipping times and wasteful packaging. Our application seeks to allow people looking for clothing in one centralized place and give local clothing shops a platform to reduce time and energy costs and make shopping for clothing more convenient.

App Description: Application loads a list of stores depending on location of user and displaying the stores at closest range. Application allows user to scroll through nearby stores and allows user to click on a store of interest to see the store's list of products. Application also contains search bar that allows user to search for specific products and the application will display a list of products that match the search. Application will also contain a feature that allows local stores to display their store information alongside products and their store will be displayed to shoppers nearby and their products will be displayed if user searches for a product that matches the given description.

## User Roles and Personas

Include the most up-to-date user roles and personas.


Shopper: someone seeking to purchase clothing

Emma is a local boutique owner and is trying to increase sales, but does not a have platform to display her products to a wider range of people. She can enroll on our site as a vendor to begin displaying her merchandise online in a place frequented by local shoppers.
Emily just received extra inventory for several of her products and is having trouble selling through store front and is looking to promote her business.

Vendor: someone trying to sell their clothes locally

Eva recently tore her favorite pair of work pants and is in need of a new pair but is caught up in work and therefore can not find the time to go shopping in look for new pants.
Ellie loves online shopping but recently read an article about all the cardboard and plastic waste that is harmful to the planet due to online shopping. However, Ellie finds it more convenient to shop online and wants to continue in a more environmentally and friendly way.
Ella frequently purchases different clothing items in various stores and finds it inconvenient the high shopping cost for each store.

## User Stories

List the current user stories you will implement.

- As a shopper, I want to be able to have a centralized list of stores near me, so that I can better identify clothing stores that suit my style.
- As a shopper, I want to know the kind of merchandise available in the stores near me, so that I can save my time when shopping.
- As a shopper, I want to avoid gathering too much cardboard and plastic waste as possible, to be more sustainable.
- As a shopper, I want to know about the clothing stores near me, in order to support local businesses and vendors.
- As a vendor, I want to have a place for people to see what I sell, to generate more revenue.
- As a vendor, I want my customers to shop in a more environmentally and friendly way.
- As a vendor, I want to have a tracking page for all the online orders.
- As a shopper, I want to be able to not pay several shipping costs for different stores.
- As a vendor, I want my customers to easy and convenient way to purchase my products.
- As a shopper, I want to be able to search for a specific product in a convenient way.

## Pages/Screens

List all the pages and screens in the app. Include wireframes for at least 3 of them.

Link to Wireframe: https://www.figma.com/file/OhMsVzc4yNkFRXoyoKxgMw/Name?node-id=0%3A1

## Data Model

Describe your app's data model using diagrams or tables
| Store Card | Type | Description |
| --- | --- | --- |
| store_id | integer | primary key for store |
| store_name | text | store name |
| location | text | address of store |
| image | url | store picture/logo |
| description | text | information of store |

| User | Type | Description |
| --- | --- | --- |
| user_id | integer | primary key for store |
| first_name | text | first name |
| last_name | text | last name |
| email | text | email/username for user |
| password | text | hashed password |
| number | integer | phone number of user |

| Product Card | Type | Description |
| --- | --- | --- |
| product_id | integer | primary key for store |
| store_id | integer | store key |
| name | text | name of product |
| description | text | description of product |
| price | integer | cost of product |
| image | url | picture of product |
| category | text | specific category for product |
| color | text | color of product |
| size | text | size of product |
| quantity | integer | amount of product |

| Shopping Cart | Type | Description |
| --- | --- | --- |
| user_id | integer | key |
| product_id | integer | key |
| store_id | integer | key |

| Checkout | Type | Description |
| --- | --- | --- |
| user_id | integer | key |
| store_id | integer | key |
| location | integer | key |

| Wishlist | Type | Description |
| --- | --- | --- |
| user_id | integer | key |
| product_id | integer | key |
| store_id | integer | key |

| Orders | Type | Description |
| --- | --- | --- |
| user_id | integer | key |
| product_id | integer | key |
| store_id | integer | key |

## Endpoints

List the API endpoints you will need to implement.
Base URL: ___.com/

Utility endpoints:
- /login
- /register

Landing Page:
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/" fetches landing page |

User: 
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/user" Fetch id of specific shopper | 
| Create | POST | "/user/:user_id" Create new user account for shopper |

Store: 
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/store/:store_id" Fetch id from store |

Product:
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/product/:product_id" Fetch id from product from all stores |
| Create | POST | "/cart/:product_id" Fetch product id from the cart |
| Create | POST | "/wishlist/:product_id" Fetch product from the wishlist |

Shopping Cart:
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/cart" Fetch list of products in cart |
| Create | POST | "/orders/:order_id" Create new order with list of products in cart |

Orders:
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/orders" Fetch order list |

Wishlist
| CRUD | HTTP Verb | Description |
| --- | --- | --- |
| Read | GET | "/wishlist" Fetch product list in wishlist |

***Don't forget to set up your Issues, Milestones, and Project Board!***
