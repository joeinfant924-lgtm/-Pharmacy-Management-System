# -Pharmacy-Management-System
-- Medicine Table
CREATE TABLE Medicine (
    Medicine_ID INT,
    Medicine_Name VARCHAR(50),
    Price INT,
    Quantity INT,
    Expiry_Date DATE
);

INSERT INTO Medicine VALUES
(101,'Paracetamol',20,100,'2026-05-10'),
(102,'Amoxicillin',45,50,'2026-07-15'),
(103,'Vitamin C',30,80,'2026-09-20');

-- Customer Table
CREATE TABLE Customer (
    Customer_ID INT,
    Customer_Name VARCHAR(50),
    Phone VARCHAR(15),
    Address VARCHAR(50)
);

INSERT INTO Customer VALUES
(1,'Ravi Kumar','9876543210','Bangalore'),
(2,'Anil Kumar','9123456780','Chennai'),
(3,'Priya Sharma','9988776655','Hyderabad');

-- Supplier Table
CREATE TABLE Supplier (
    Supplier_ID INT,
    Supplier_Name VARCHAR(50),
    Phone VARCHAR(15),
    Address VARCHAR(50)
);

INSERT INTO Supplier VALUES
(201,'ABC Pharma','9876501234','Mumbai'),
(202,'MediLife Suppliers','9765432109','Delhi');

-- Billing Table
CREATE TABLE Billing (
    Bill_ID INT,
    Customer_ID INT,
    Medicine_ID INT,
    Quantity INT,
    Total_Price INT,
    Date DATE
);

INSERT INTO Billing VALUES
(1,1,101,2,40,'2026-03-12'),
(2,2,103,3,90,'2026-03-12');

-- OUTPUT
SELECT * FROM Medicine;
SELECT * FROM Customer;
SELECT * FROM Supplier;
SELECT * FROM Billing;