# sqltask
### create a database Loan Applications Database
```
create database Loan Applications Database
```
### create a table name Loans
```sql
create table Loans(
ID tinyint,
FirstName Varchar(40),
LastName Varchar(40),
Email Varchar(40),
LoanAmount number,
Purpose Varchar(20),
Status Varchar(20));
```
### insert records into table
```sql
1. insert into Loans(ID, FirstName, LastName, Email, LoanAmount, Purpose, Status) 
values( 1,'John', 'Doe','john.doe@example.com',10000,'Home Improvement','Approved');
2. insert into Loans(ID, FirstName, LastName, Email, LoanAmount, Purpose, Status) 
values( 2,'Jane', 'Smith','jane.smith@example.com',5000,'Debt Consolidation','Approved');
3. insert into Loans(ID, FirstName, LastName, Email, LoanAmount, Purpose, Status) 
values( 3,'Bob', 'Johnson','bob.johnson@example.com',15000,'Business','Pending');
4. insert into Loans(ID, FirstName, LastName, Email, LoanAmount, Purpose, Status) 
values( 4,'Emily', 'Brown','emily.brown@example.com',8000,'Vacation','Approved');
5. insert into Loans(ID, FirstName, LastName, Email, LoanAmount, Purpose, Status) 
values( 5,'Michael', 'Davis','michael.davis@example.com',20000,'Education','Denied');
6. insert into Loans(ID, FirstName, LastName, Email, LoanAmount, Purpose, Status) 
values( 6,'Sarah', 'Wilson','sarah.wilson@example.com',10000,'Home Improvement','Approved');
```
### Select all loan applications from the table
```sql
select * from Loans;
```
### select all loan applications with a status of "Approved"
```sql
select * from Loans
where status='Approved';
```
### select all loan applications with a loan amount greater than 10000.
```sql
select * from Loans
where LoanAmount > 10000
```
### Update the status of all loan applications with a purpose of "debt consolidation" to "approved"
update Loans set status='Approved' where Purpose='Debt Consolidation';
### Update the loan amount of a specific loan application by its ID.
update Loans set LoanAmount=19000 where ID=1;
### Delete all loan applications with a status of "Denied".
Delete from Loans where status='Denied';
### select the first name, last name and loan amount of all loan applications.
```sql
select FirstName,LastName,LoanAmount form Loans;



