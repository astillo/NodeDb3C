# Database Queries

### Display the ProductName and CategoryName for all products in the database. Shows 76 records.
select P.ProductName, C.CategoryName 
from products as P 
join Categories as C on C.CategoryID = C.CategoryID
### Display the OrderID and ShipperName for all orders placed before January 9, 1997. Shows 161 records.
select o.OrderID, s.ShipperName
from Orders as o 
join Shippers as s on s.ShipperName = s.ShipperName
where o.OrderDate >= '1997-01-09'
### Display all ProductNames and Quantities placed on order 10251. Sort by ProductName. Shows 3 records.

### Display the OrderID, CustomerName and the employee's LastName for every order. All columns should be labeled clearly. Displays 196 records.

### (Stretch)  Displays CategoryName and a new column called Count that shows how many products are in each category. Shows 9 records.

### (Stretch) Display OrderID and a  column called ItemCount that shows the total number of products placed on the order. Shows 196 records. 