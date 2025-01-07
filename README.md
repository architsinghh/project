# Amazon-Like Retail System

## Overview
A simplified online retail system that enables product searches, cart management, and purchases.

### Features
- **Search Functionality** with AND/OR operations
- **Shopping Cart Management**
- **Product Categories**: Books, Clothing, Movies
- **User Management** with credit tracking
- **Database Storage** and retrieval

## System Architecture

### Product Categories
| Category | Attributes |
|----------|------------|
| Books    | Name, Price, Quantity, ISBN, Author |
| Clothing | Name, Price, Quantity, Size, Brand |
| Movies   | Name, Price, Quantity, Genre, Rating |

### Commands
- AND term1 term2   :  Products matching all terms
- OR term1 term2    :  Products matching any term
- ADD username hit  :  Add item to cart
- VIEWCART username :  Show cart contents
- BUYCART username  :  Process purchase
- QUIT filename     :  Save and exit


## Technical Requirements

### Core Components
- **Product Class Hierarchy**
- **Custom DataStore Implementation**
- **Keyword Indexing System**
- **Shopping Cart Management**
- **Database Parsing and Saving**

### Performance Specifications
- O(n*log(n)) search operations
- Memory leak-free implementation
- Case-insensitive search
- FIFO cart ordering

# Database Format

## Products Section
<products>
book
Data Abstraction & Problem Solving with C++
79.99
20
978-013292372-9
Carrano and Henry

book
Great Men and Women of Troy
19.50
5
978-000000000-1
Tommy Trojan

clothing
Men's Fitted Shirt
39.99
25
Medium
J. Crew

movie
Hidden Figures DVD
17.99
1
Drama
PG
</products>

## Users Section
<users>
aturing 100.00 0
johnvn 50.00 0
adal 120.00 1
</users>
