create table Employees( 
EmpID number, 
EmpName varchar2(20), 
EmailID varchar2(20), 
mobileNo number, 
gender char(1), 
DateOFJoining date default sysdate);

alter table Employees drop column EmpID;

desc Employees;

alter table Employees set unused column gender;

desc Employees;
//truncate table Emlooyees; will release memory but if we use desc Employees; then it will show the table but all the data will be  deleted.
//if we use drop table Employees then all the data and table deleted. if we use desc Employees; then it will not show the table.
