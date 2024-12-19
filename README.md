# Online Bookstore and Reading Competition Database System

This project is designed to manage the operations of an online bookstore and a reading competition. The system handles information related to books, orders, customers, competitions, participants, inventory, and employees.

## Entities and Attributes

### 1. **Book**
- **Attributes**:
  - `Book_ISBN` (Primary Key)
  - `Book_Year`
  - `Title`
  - `Price`

### 2. **Order**
- **Attributes**:
  - `Order_ID` (Primary Key)
  - `Customer_ID` (Foreign Key)
  - `Shipping_Type`
  - `Total_Fee`

### 3. **Customer**
- **Attributes**:
  - `Customer_ID` (Primary Key)
  - `Customer_Name`
  - `Customer_Phone`
  - `Customer_Address`

### 4. **Comment**
- **Attributes**:
  - `Order_ID` (Primary Key, Foreign Key from Order)
  - `Book_ISBN` (Foreign Key from Book)
  - `Text`
  - `Rating`

### 5. **Competition**
- **Attributes**:
  - `Competition_ID` (Primary Key)
  - `Competition_Type`
  - `Competition_Date`

### 6. **Employee**
- **Attributes**:
  - `Employee_ID` (Primary Key)
  - `Department`
  - `Salary`
  - `Competition_ID` (Foreign Key from Competition)

### 7. **Inventory**
- **Attributes**:
  - `Book_ISBN` (Primary Key, Foreign Key from Book)
  - `Inventory_Quantity`
  - `Employee_ID` (Foreign Key from Employee)

### 8. **Participant**
- **Attributes**:
  - `Participant_ID` (Primary Key)
  - `Participant_Name`
  - `Participant_Mobile`
  - `Participant_Address`
  - `Participant_Email`
  - `Participant_Type`
  - `Competition_ID` (Foreign Key from Competition)

## Objectives

1. Manage and organize information about the online bookstore and reading competitions.
2. Facilitate the buying and selling of books between customers and merchants.
3. Allow easy updates to the bookstore and competition information.
4. Manage procedures related to reading competitions.
5. Store and analyze information about books, orders, customers, and competition results.
6. Generate reports based on historical buying and selling trends to understand market trends.
7. Reduce operational costs and increase convenience for customers, participants, and staff.

## Scope

### System Scope
- The system manages the online bookstore, reading competitions, and related entities such as books, orders, inventory, participants, employees, and competition prizes.
- It tracks book availability, sales, and stock levels within the online bookstore.
- It records competition details, including participant scores and prize distribution.

### User Scope

1. **Customer**:
   - Buy books from the bookstore.
   - Add books to the shopping basket and complete the order.
   
2. **Participant**:
   - Participate in competitions.
   - Receive scores and prizes for winning the competition.
   - Ask for assistance from the staff.

3. **Author**:
   - Write books and make them available for sale in the bookstore.
   
4. **Staff**:
   - Manage competition prizes, update competition details, record scores, and assist participants.
   - Act as a point of contact between customers and the bookstore.

5. **Publisher**:
   - Publish books and supply them to the bookstore owners.

## Conclusion
This database system will streamline the operations of the online bookstore and reading competitions, providing a seamless user experience for customers, participants, and staff. By organizing key data and automating processes, it will reduce administrative workload and provide valuable insights for decision-making.

## Features

- **Customer Management**: Store and manage customer information.
- **Order Management**: Track book orders, shipping types, and total fees.
- **Inventory Management**: Track book stock, managed by employees.
- **Commenting System**: Customers can rate and review books.
- **Competition Management**: Employees can update competition information and record participant scores.
- **Report Generation**: Generate reports based on sales and competition data.

## How to Use

1. Clone the repository.
2. Set up the database with the provided schema.
3. Implement required functionalities to manage books, orders, customers, and competitions.
4. Add, update, and query data to manage the online bookstore and competitions.

Feel free to modify the sections based on your actual project structure and any additional requirements you may have.
