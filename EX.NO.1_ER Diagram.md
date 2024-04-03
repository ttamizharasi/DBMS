![image](https://github.com/ttamizharasi/DBMS/assets/119657317/e61f4783-b6b6-400a-8b3a-aa488a1e83b9)# EXP NO 1: ER DIAGRAM CREATION, RELATIONAL MODEL AND SCHEMA GENERATION  
### DATE
## AIM:
<div align="justify">
   To create a ER Diagram for Bank management system or College management system using ERD Plus tool and generate the relational model with schema. 
</div>

## Algorithm
1. Create a login with https://erdplus.com.
2. Create a new ER Diagram with name
3. Create a strong entity, relation and attributes.
4. Create a weak entity, relation and attributes.
5. Specify attributes unique, multivalued and composite attributes.

### ER Diagram 
![ER diagram](https://github.com/ttamizharasi/DBMS/assets/119657317/819177b1-d7ac-4e2f-93bb-a95c1b91134c)

### Relational model
![Screenshot 2024-04-03 103224](https://github.com/ttamizharasi/DBMS/assets/119657317/2716896a-976f-44f1-8c31-526607106584)

### SQL DDL Schema
```
CREATE TABLE BANK
(
  Code INT NOT NULL,
  Name INT NOT NULL,
  Addr INT NOT NULL,
  PRIMARY KEY (Code)
);

CREATE TABLE BANK_BRANCH
(
  Branch_no INT NOT NULL,
  Addr INT NOT NULL,
  PRIMARY KEY (Branch_no)
);

CREATE TABLE LOAN
(
  Loan_no INT NOT NULL,
  Amount INT NOT NULL,
  Type INT NOT NULL,
  PRIMARY KEY (Loan_no)
);

CREATE TABLE CUSTOMER
(
  Phone INT NOT NULL,
  Ssn INT NOT NULL,
  Name INT NOT NULL,
  Addr INT NOT NULL,
  PRIMARY KEY (Ssn)
);

CREATE TABLE ACCOUNT
(
  Acct_no INT NOT NULL,
  Balance INT NOT NULL,
  Type INT NOT NULL,
  PRIMARY KEY (Acct_no)
);
```
## RESULT 
<div align="justify">
Thus the ER diagram was drawn and relational diagram, SQL DDL staements are generated using ERD plus tool.
</div>
