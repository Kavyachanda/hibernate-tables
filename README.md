# hibernate-tables
I have created product,supplier and category tables in database.

create table category
(
 id varchar(20) primary key,
 name varchar(20) not null,
 description varchar(50)
 )
 
 create table supplier
(
 id varchar(20) primary key,
 name varchar(20) not null,
 address varchar(50)
 )
 
 create table product
(
 id varchar(20) primary key,
 name varchar(20) not null,
 price double,
 category_id varchar(20) references category(id),
 supplier_id varchar(20) references supplier(id)
 )
