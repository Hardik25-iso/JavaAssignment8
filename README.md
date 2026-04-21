# JavaAssignment8

# Product Management System (Java – Collections & Singleton Design Pattern)

## Overview

This project is a **Java-based Product Management System** that demonstrates the use of the **Java Collections Framework** along with the **Singleton Design Pattern**.

The application allows users to manage products by performing operations such as adding, removing, displaying, searching, and sorting products. It uses efficient data structures like `ArrayList` and `HashMap` to ensure optimized performance.

---

## Features

* Add new products
* Remove products by ID
* Display all products in tabular format
* Search products by name
* Sort products by price
* Ensure unique product IDs
* Menu-driven interface
* Implementation of Singleton Design Pattern

---

## Project Structure

### 1. Product Class

Represents a product entity.

#### Data Members

* `productId` – unique identifier
* `name` – product name
* `price` – product price
* `quantity` – available quantity

#### Methods

* `toString()` – returns formatted product details for display

---

### 2. ProductManager Class (Singleton)

Manages all product-related operations.

#### Key Features

* Implements Singleton pattern to ensure only one instance exists
* Uses:

  * `ArrayList` to store products
  * `HashMap` for fast lookup using product ID

#### Methods

* `getInstance()` – returns the single instance
* `addProduct(Product p)` – adds a product
* `removeProduct(int id)` – removes a product
* `displayProducts()` – displays all products
* `searchProduct(String keyword)` – searches by name
* `sortByPrice()` – sorts products by price

---

### 3. CollectionsDesignPatternApp Class (Main Class)

Handles user interaction and program execution.

Responsibilities:

* Provides menu-driven interface
* Takes user input
* Calls appropriate methods from `ProductManager`
* Demonstrates Singleton behavior

---

## Design Pattern Used

### Singleton Pattern

* Ensures only one instance of `ProductManager` exists
* Prevents inconsistent data handling
* Accessed via:

```
ProductManager.getInstance()
```

---

## Data Structures Used

* **ArrayList**

  * Stores products dynamically
  * Maintains insertion order

* **HashMap**

  * Maps product ID to product object
  * Enables fast lookup and validation

---

## Functionalities

1. Add Product
2. Remove Product
3. Display All Products
4. Search Product by Name
5. Sort Products by Price
6. Exit Application

---

## How to Run the Program

### Prerequisites

* Java Development Kit (JDK) installed
* Terminal or command prompt

### Steps

1. Compile the program:

```
javac CollectionsDesignPatternApp.java
```

2. Run the program:

```
java CollectionsDesignPatternApp
```

---

## Sample Output

```
Same instance? true

1.Add  2.Remove  3.Display  4.Search  5.SortByPrice  0.Exit
Choice: 3

+------+----------------------+----------+-------+
| ID   | Name                 |  Price   | Qty   |
+------+----------------------+----------+-------+
| 1    | Laptop               | 65000.00 | 10    |
| 2    | Mouse                |   800.00 | 50    |
...
```

---

## Concepts Used

* Java Collections Framework (`ArrayList`, `HashMap`)
* Object-Oriented Programming
* Singleton Design Pattern
* Method abstraction
* Sorting using Comparator
* Exception Handling
* Menu-driven programs

---





Tell me the number.
