Employees

- Columns: EmployeeID, FirstName, LastName, Age, PhoneNumber, Address, Salary
  
- Description: Stores details of company employees
  
- Relationship: One-to-Many (with Offices)

Customers

- Columns: CustomerID, FirstName, LastName, LastTimeBuying, Address, PhoneNumber
  
- Description: Stores customer information
  
- Relationship: One-to-Many (with Orders, Payments)

Products

- Columns: ProductID, Price, ProductLine, QuantityInStock, BuyPrice, MSRP

- Description: Stores product pricing and inventory data
  
- Relationships: Many-to-One (Product Lines), Many-to-Many (Orders via Order Details)

Stores

- Columns: StoreID, Location, Size, NumberOfEmployees
  
- Description: Physical retail store locations
  
- Relationship: One-to-Many

Manufacturing Locations

- Columns: ManufacturingLocationID, Location, ProductManufactured

- Description: Tracks where products are manufactured
  
- Relationship: Many-to-Many (via associative table)

Product Details

- Columns: ProductID, ProductName, TextDescription
  
- Description: Descriptive information for products

Orders

- Columns: OrderID, OrderDate, CustomerNumber, QuantityOrdered, OrderStatus

- Description: Captures customer purchase activity
  
- Relationships:
  - Many-to-One (Customers)
  - Many-to-Many (Products via Order Details)

Order Details (Associative Table)

- Columns: OrderID, DateOfPurchase, DateOfDelivery
  
- Description: Links orders and products
  
- Relationship: Many-to-One with Orders and Products

Product Lines

- Columns: ProductLineCode, ProductLineName
  
- Description: Categorizes products
  
- Relationship: One-to-Many (with Products)

Offices

- Columns: OfficeNumber, City, State, Address
  
- Description: Corporate and administrative locations
  
- Relationship: One-to-Many (with Employees)

Payments

- Columns: CustomerID, PaymentDate, Amount
  
- Description: Tracks customer payment activity
  
- Relationship: Many-to-One (with Customers)
