DRAFT
dito muna code at changes

# Inventory Management System Instructions

## Overview
Create an inventory management system for a store that tracks products, their quantities, prices, and suppliers. This system will allow users to add, update, remove, and display product information, as well as track sales and generate reports. The system should utilize arrays, structures, pointers, linked lists, and file handling to manage data.

## Features to Implement

### Functions
- **Product Management:**
  - Functions for adding, updating, deleting, and searching products.
- **Sales Tracking:**
  - Functions to calculate total sales, generate reports, and handle user interactions.
- **Data Persistence:**
  - Functions to save and load data from files.
- **Product Information:**
  - Functions for viewing specific product information.

### Arrays
- Use arrays to store product information temporarily before transitioning to linked lists or other dynamic structures.
- Store product names, prices, and quantities in arrays for initial implementation or a simpler view.

### Character and String Manipulation
- Use strings (or character arrays) to store product names, supplier names, and categories.
- Allow for searches or filtering based on product names, and manipulate strings by trimming or formatting input.

### Structures
- Define a `Product` structure that holds:
  - Product ID
  - Name
  - Price
  - Quantity in stock
  - Supplier information (which could be another structure).
- Define other structures as needed, such as `Sale` or `Supplier`, depending on the system's complexity.

### Pointers
- Use pointers for dynamically allocating memory for the linked list of products.
- Use pointers in functions to pass data by reference to avoid unnecessary copies, especially for large structures like product records.
- Use pointers to link product records in the linked list.

### Linked List
- Implement a linked list to store products. Each node would contain a `Product` structure and a pointer to the next product.
- Provide operations like:
  - Adding a new product
  - Removing a product
  - Updating product details
- Traverse the linked list to display product information or generate reports.

### File Handling
- Use file handling to load the inventory from a file (e.g., `inventory.txt`) on startup.
- Store updated product details (like quantities, prices, and sales) back to a file whenever changes are made.
- Implement file reading and writing using streams to store product data in a readable and editable format (e.g., CSV or tab-separated).

## Possible Workflow

### Main Menu System (for User Interaction)
Display a menu allowing users to perform operations like:
1. Add a new product.
2. Update product information (e.g., change price or quantity).
3. Delete a product.
4. Search for a product by name or ID.
5. Display all products.
6. Track sales and update inventory.
7. Generate sales reports (e.g., total sales for the day).
8. Save inventory to a file and load inventory from a file.

### Product Data Flow
1. On startup, read the inventory data from a file into a linked list of products.
2. The user can then perform actions to modify the inventory (add new products, delete, or update details).
3. After any change, the system will save the updated inventory back to the file.

## Bonus (Advanced Features)
- Track sales and automatically update inventory when products are sold.
- Implement a sales report feature to calculate total sales or the remaining inventory for each product.
- Allow multiple suppliers, and link products to their suppliers using another structure (e.g., a `Supplier` structure with information about suppliers).

## Detailed Breakdown of Topics Covered
- **Functions:** Handle different actions such as adding, deleting, and updating products; calculating total sales; displaying reports.
- **Arrays:** Store product information temporarily in arrays before transitioning to a dynamic linked list.
- **Character/String Manipulation:** Handle product names and other text fields, such as searching for products by name.
- **Structures:** Use structures to represent products, sales, suppliers, and other key entities in the system.
- **Pointers:** Use pointers to dynamically allocate memory for product records and linked list nodes.
- **Linked List:** Store products in a linked list and provide operations to add, remove, or modify product data.
- **File Handling:** Read and write product data from/to a file to ensure data persistence across program sessions.
