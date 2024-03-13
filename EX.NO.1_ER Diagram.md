# EXP NO 1: ER DIAGRAM CREATION, RELATIONAL MODEL AND SCHEMA GENERATION  
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

![erd diagram](https://github.com/arunkumardev-07/DBMS/assets/135949761/104657c0-e27e-4654-9258-dc602ea920c3)


### Relational model
![Screenshot 2024-03-13 110007](https://github.com/arunkumardev-07/DBMS/assets/135949761/ef44aab5-1817-4265-ba42-26a2c1011bbe)





### SQL DDL Schema 
```
CREATE TABLE Employee
(
  Ssn INT NOT NULL,
  Bdate INT NOT NULL,
  Minit INT NOT NULL,
  Lname INT NOT NULL,
  Fname INT NOT NULL,
  Salary INT NOT NULL,
  Sex INT NOT NULL,
  PRIMARY KEY (Ssn)
);

CREATE TABLE Department
(
  Name INT NOT NULL,
  Number INT NOT NULL,
  PRIMARY KEY (Name),
  UNIQUE (Number)
);

CREATE TABLE Project
(
  Location INT NOT NULL,
  Number INT NOT NULL,
  Name INT NOT NULL,
  PRIMARY KEY (Number),
  UNIQUE (Name)
);

CREATE TABLE Dependent
(
  Name INT NOT NULL,
  Sex INT NOT NULL,
  Relationship INT NOT NULL,
  Birth_date INT NOT NULL,
  PRIMARY KEY (Name)
);

CREATE TABLE Department_Location
(
  Location INT NOT NULL,
  Name INT NOT NULL,
  PRIMARY KEY (Location, Name),
  FOREIGN KEY (Name) REFERENCES Department(Name)
);
```

## RESULT 
<div align="justify">
Thus the ER diagram was drawn and relational diagram, SQL DDL staements are generated using ERD plus tool.
</div>
