# InvestigatoryProject

Source used for SQL installation
https://www.youtube.com/watch?v=MhaH7o3lf4E

Used pip to install sql, sql connector and curses libraries

Create a database named Hubnet and tables Bank & Transaction

create table bank(name varchar(30), UserName varchar(30),password tinytext , Date_of_birth date, address varchar(40) ,Mobile_Number varchar(30) ,Aadhar_no varchar(30), Balance int, PRIMARY KEY(UserName));

create table Transaction(credited int , debited int , username1 varchar(20), Date date, foreign key(username1) references bank(Username));
