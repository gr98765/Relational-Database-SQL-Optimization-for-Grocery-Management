Relational Model from ER Diagram 

CUSTOMER (cust\_ID, c\_first\_name, c\_last\_name, c\_email, c\_address) 

* Primary Key: cust\_ID 

CUST\_PHONE (cust\_ID, c\_phone) 

* Primary Key: cust\_ID 
* Foreign Key (cust\_ID) references CUSTOMER 

TRANSACTION (transaction\_ID, store\_ID,t\_date, cust\_ID) 

* Primary Key: transaction\_ID 
* Foreign Key (cust\_ID) references CUSTOMER 
* Foreign Key (store\_ID) references STORE 

TRANSACTION\_RECORD (transaction\_ID, quantity, total\_price) 

* Primary Key: (transaction\_ID) 
* Foreign Key (transaction\_ID) references TRANSACTION 

STORE (store\_ID, store\_name, location, poduct\_ID,manager\_ID) 

* Primary Key: store\_ID 
* Foreign Key (manager\_ID) references MANAGER 
* Foreign Key(product\_ID) references PRODUCT 

MANAGER (manager\_ID, m\_first\_name, m\_last\_name, m\_email) 

Primary Key: manager\_ID 

PRODUCT (product\_ID, product\_name, cost, p\_quantity, manufacture\_date, brand\_ID,store\_ID, category\_ID) 

* Primary Key: product\_ID 
* Foreign Key (brand\_ID) references BRAND 
* Foreign Key (category\_ID) references CATEGORY 
* Foreign Key (store\_ID) references STORE 

HAS\_STOCK (product\_ID, store\_ID) 

* Primary Key: product\_ID 
* Primary Key: store\_ID 
* Foreign Key (product\_ID) references PRODUCT 
* Foreign Key (store\_ID) references STORE 

PRICE\_RECORD (price\_record\_ID, product\_ID, effective\_date, retail\_price, promotional\_price) 

* Primary Key: (product\_ID, price\_record\_ID) 
* Foreign Key (product\_ID) references PRODUCT 

CATEGORY (category\_ID, category\_name) 

* Primary Key: category\_ID 

BRAND (brand\_ID, brand\_name, manufacturer\_name) 

* Primary Key: brand\_ID 

TIME\_PERIOD (time\_period\_ID,period\_name,start\_date,end\_date) 

* Primary Key: time\_period\_ID 

SUPPLIER (supplier\_ID, s\_name, s\_email) 

* Primary Key: supplier\_ID 

SUPPLIER\_PHONE (supplier\_ID, s\_phone) 

* Primary Key: supplier\_ID 
* Foreign Key (supplier\_ID) references SUPPLIER  

SUPPLY\_AGREEMENT (time\_period\_ID,brand\_ID,store\_ID,supplier\_ID,product\_ID) 

* Primary Key: time\_period\_ID 
* Primary Key: brand\_ID 
* Primary Key: store\_ID 
* Primary Key: supplier\_ID 
* Primary Key: product\_ID 
* Foreign Key (supplier\_ID) references SUPPLIER  
* Foreign Key (product\_ID) references PRODUCT 
* Foreign Key (brand\_ID) references BRAND 
* Foreign Key (store\_ID) references STORE 
* Foreign Key (time\_period\_ID) references TIME\_PERIOD 



Assumptions 

* One price record could be for only 1 product.  
* One product can have multiple price records. 
* One store must have at least one transaction. 
* One transaction can be made to one store. 
* One manager manages only one store. 
* Products belong to one brand and one category, but the brand and category have many products. 
* Store could have 0 or many product stocks.
