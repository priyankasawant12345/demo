in angular folder 
1) npm install
2) ng serve

in express folder
1) npm install
2) in cmd terminal node sever.js

login Credentials:
1) Username - demo, Password - demo
2) Username -Priyanka, Password -Priyanka
3) Username -abc, Password - abc 

In the dashboard page data display with above credentials . we can perform CRUD operation on the data.

Oracle Database as below:
there are two tables with following columns
1) users - id, username, password
2) orders -ordered,id,productid, productname, totalamount


CREATE TABLE USERS(
id number PRIMARY KEY,
username varchar2(100),
password varchar2(100)
);

insert into users (id,username,password) values (1,'demo','demo');
insert into users (id,username,password) values (2,'abc','abc');
insert into users (id,username,password) values (3,'Priyanka','Priyanka');

CREATE TABLE orders (
    orderid NUMBER PRIMARY KEY,
    id NUMBER,
    productids VARCHAR2(100),
    totalamount NUMBER,
    CONSTRAINT fk_user FOREIGN KEY (id) REFERENCES users(id)
);

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (1, 1, '101', 500, 'Laptop');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (2, 2, '102', 300, 'Keyboard');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (3, 3, '103', 150, 'Mouse');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (4, 1, '104', 500, 'Bluetooth');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (5, 2, '105', 300, 'Speaker');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (6, 3, '106', 150, 'Headphones');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (7, 1, '107', 800, 'Tablet');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (8, 2, '108', 1000, 'USB');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (9, 3, '109', 1500, 'Bluetooth Headphones');

INSERT INTO orders (orderid, id, productids, totalamount, productname)
VALUES (10, 3, '1010', 2000, 'Gaming Laptop');


