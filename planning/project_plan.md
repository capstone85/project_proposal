# Project Plan

Pod Members: **Adriana Morales, Cynthia Delira, Michelle Fox-Romero, Monica Kirabo**

## Problem Statement and Description

Insert the latest summary of your problem statement and app description.

Problem statement: Many people find difficulty in looking for specific clothing items and must travel from shop to shop, either online or in person, just to see what kinds of things are in store. An upward trend in fast fashion purchases has also increased environmental and energy costs due to long shipping times and wasteful packaging. Our application seeks to allow people looking for clothing in one centralized place and give local clothing shops a platform to reduce time and energy costs and make shopping for clothing more convenient.

App Description: Application loads a list of stores depending on location of user and displaying the stores at closest range. Application allows user to scroll through nearby stores and allows user to click on a store of interest to see the store's list of products. Application also contains search bar that allows user to search for specific products and the application will display a list of products that match the search. Application will also contain a feature that allows local stores to display their store information alongside products and their store will be displayed to shoppers nearby and their products will be displayed if user searches for a product that matches the given description.

## User Roles and Personas

Include the most up-to-date user roles and personas.

## User Stories

List the current user stories you will implement.

## Pages/Screens

List all the pages and screens in the app. Include wireframes for at least 3 of them.


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

## Endpoints

List the API endpoints you will need to implement.

***Don't forget to set up your Issues, Milestones, and Project Board!***
