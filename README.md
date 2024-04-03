 Database Fundamentals :-

 What is Database ?
 What is DBMS ?
 Types of DBMS ?
 What is RDBMS ?
 What is ORDBMS ?
 DB development life cycle
 ER model
 Normalization


 ORACLE 19C

 Languages :- 

 SQL
 PL/SQL

 SQL :-

 SQL commands
 DDL commands
 DML commands
 DQL commands
 writing queries using various clauses like where,order by
 writing queries using group by
 writing queries using joins
 writing queries using subqueries
 Database Transactions
 views
 indexes
 sequences

 PL/SQL :- 

 writing simple pl/sql programs
 writing programs using cursors
 writing programs using stored procedures
 writing programs using functions
 writing programs using triggers 

 Database :- a Database is a organized collection of interrelated
 data.for example a univ db stores data related to students,
 courses,faculty etc.

 
  VARIABLES           FILES              DATABASES 

  not permanent      permanent          permanent  
  not secured        not secured        secured

=> Databases are 2 types 

 1 OLTP DB (online transaction processing)
 2 OLAP DB (online analytical processing) / DWH

=> organizations uses OLTP db for storing day-to-day transactions
  and OLAP db for analysis. OLTP is used for running business and OLAP is used for
  analyzing business.

=> day-to-day operations on db includes 

  1 C (create)
  2 R (read)
  3 U (update)
  4 D (delete)

 => users cannot directly operate databases and databases are
 operated through a software called DBMS.


 DBMS :- (Database Management System)

 => DBMS is a software used to create,read,update,delete data
   in database.

 => DBMS is an interface between user and database.
 
        C
  USER--R---------DBMS-----------DB
        U
        D
 
 Evolution of DBMS :- 

 
  1960           fms  (file mgmt system)

  1970		 hdbms (hierarchical dbms)
		 ndbms (network dbms)

  1980		 rdbms (relational dbms)

  1990		 ordbms (object relational dbms)
		 oodbms (object oriented dbms)

 File Management System :- 

          data storage +  data processing

          files           COBOL

 DisAdvantages :- 

 1 difficult to access(R) and manipulate(C,U,D) data
 2 more redundency (duplication of data)
 3 less security
 4 doesn't support data integrity (data quality)
 5 doesn't support data sharing
 6 doesn't supports transactions 

 Types of DBMS :- 

 hdbms
 ndbms
 rdbms
 ordbms
 oodbms

 RDBMS :- (relational database management system)

 => rdbms concepts introduced by E.F.CODD
 => e.f.codd introduced 12 rules called codd rules
 => a db software supports all 12 rules is called perfect rdbms

 information rule :- 

 => according to information rule data must be organized in tables
    i.e. rows and columns

    DATABASE =  COLLECTION OF TABLES
    TABLE    =  COLLECTION OF ROWS & COLS
    ROW      =  COLLECTION OF FIELD VALUES
    FIELD    =  COLLECTION OF VALUES ASSIGNED TO ONE COLUMN

=> every table must contain a primary key to uniquely identify
 records.

 Ex :- accno,empid,aadharno,panno
 
 => one table is related to another table by using foreign key.

        foreign key
        key of foreign
        pk  of some other table

   CUSTOMERS
   CID(PK)	CNAME	CADDR
   10		A	HYD
   11		B	MUM
   12		C	DEL

   ORDERS
   ORDID   ORD_DT   DEL_DT    CID(FK)
   1000    01-APR   20-APR    10
   1001    05-APR   25-APR    11
   1002    10-APR   30-APR    12

 RDBMS features :- 

 1 organizing data in the form of tables i.e. rows and cols
 2 every table contains to uniquely identify records
 3 one table related to another table using foreign key
 4 easy to access and manipulate data
 5 more security
 6 less redundency
 7 supports data integrity (data quality)
 8 supports data sharing
 9 supports transactions (ACID properties)

    A  => atomocity
    C  => consistency
    I  => isolation
    D  => durability

 RDBMS softwares :- 

 oracle         from Oracle corp
 sql server     from Microsoft
 mysql          open source
 postgresql     open source

 ORDBMS :- (object relational database management system)

 => it is the combination of RDBMS & OOPS
  
     ORDBMS = RDBMS + OOPS (reusability)

 => RDBMS doesn't support reusability but ORDBMS supports
 reusability.

 => ORDBMS supports reusability by using ADT(abstract datatype)

   RDBMS :- 

     emp
     empid  ename  sal   hno  street  city  state

     cust
     cid   cname  hno  street  city  state

  ORDBMS :-  

    ADT :-  ADDR(hno,street,city,state)

    EMP
    EMPID  ENAME  ADDR

    CUST
    CID   CNAME   ADDR

 ORACLE upto 7 VER RDBMS
 ORACLE from 8 VER ORDBMS 

  What is ORACLE ?

  => ORACLE is basically a RDBMS software and also supports
 features of ORDBMS and used for db development and
 administration.

 DB DEVELOPMENT LIFE CYCLE :- 

 analysis
 design
 development
 testing
 implementation
 maintenance

 =>  DB is designed by designer/architect by using 

  1  ER model (Entity Relationship Model)
  2  Normalization

 => DB is developed by Developers & DBAs(Database Administrators)
    by using any RDBMS softwares like ORACLE.

         Developer                       DBA

  1  creating tables              installation of oracle
  2  creating views               creating database
  3  creating synonyms            creating userids
  4  creating sequences           db backup & restore
  5  creating indexes             db export & import   
  6  creating materialized views  performance tuning
  7  creating procedures          db upgradation & migration
  8  creating functions           
  9  creating triggers
  10 writing queries

 => db is tested by QA (Quality Assurance) team by using 
 some tools called testing tools.

 => implementation means moving db from Development server to
 Production server.

		   ORACLE 19C

  What is ORACLE 19C ?

 => oracle is basically a rdbms software and also supports the
 features of ordbms and used for db development and 
 administration.
 
 Versions of ORACLE :- 

 1,2,3,4,5,6,7,8,8i,9i,10g,11g,12c,18c,19c

    i => internet
    g => grid
    c => cloud

 => from  8i onwards oracle can be used for
  internet applications.

 => grid means collection of server, from 10g onwards oracle
 database can be accessed through multiple server. Adv of
 grid is it improves availability.

 => from 12c onwards oracle db is can be delivered in two ways

  1 on premises
  2 on cloud

 => in "on premises" db is deployed in the server managed by 
 client.

=> in "on cloud" db is deployed in the server managed by 
 cloud service provider for ex :- amazon.

=> the following components are installed after installing
  oracle.

 1 SERVER
 2 CLIENT

 SERVER :- 

 => server is a system where oracle software is installed and
 running. server manages two components 

  1 DB
  2 INSTANCE

 => DB is created in hard disk and acts  as permanent storage
 => INSTANCE is created in ram and acts as temporary storage.

 CLIENT :- 

 => using client system users can 

 1 connects to server
 2 submit requests to server
 3 recieves response from server

 client tools :- 

 sqlplus (CUI)
 sql developer (GUI)
 toad (GUI)

			  SQL

  =>  structured query language.
  =>  language used to communicate with oracle.
  =>  user communicates with oracle by sending commands called queries.
  =>  a query is command/instruction given to oracle to perform
      some operation on database.
  =>  SQL is introduced by IBM and initial name was "SEQUEL" 
      and later it is renamed to SQL.
  =>  SQL is common to all databases.

       ORACLE     SQL SERVER     MYSQL     POSTGRESQL
          SQL        SQL           SQL         SQL
  
   => based on operations on database SQL is categorized into
 following sublanguages.

     DDL (data definition lang)
     DML (data manipulation lang)
     DQL (data query lang)
     TCL (transaction control lang)
     DCL (data control lang)

   EMPID	ENAME	SAL   => DATA DEFINITION / STRUCTURE / METADATA
   100		ABC	5000  => DATA 
 
  sqlplus :- 

  => using this tool we can connect to oracle and we can execute
 sql commands.  
   
  user---sqlplus------sql---------oracle----------db
         tool         lang        software       storage

 schema :- a user in oracle db is called

 SERVER
    DATABASE
          USERS
             TABLES
                 DATA 

 SERVER
    ORCL
       SYS              (DBA)
       SYSTEM/manager   (DBA)
       SCOTT/TIGER      (Normal user)
       HR/HR            (Normal user)

 => to connect to oracle open sqlplus and enter username & password

   username :- system
   password :- manager

   or

   username  :-  system/manager

 creating user/account/schema in oracle :- 

 => only DBA can create new users.

 step 1 :- conn as DBA 

   USERNAME :- / AS SYSDBA

 step 2 :- create user

 syntax :-

  CREATE USER <NAME> IDENTIFIED BY <PWD>
  DEFAULT TABLESPACE USERS
  QUOTA UNLIMITED ON USERS ;

 example :-

    SQL>CREATE USER BATCH2PM IDENTIFIED BY NACRE
         DEFAULT TABLESPACE USERS
         QUOTA UNLIMITED ON USERS ;

 step 3 :- granting permissions to user

    SQL>GRANT CONNECT,RESOURCE TO BATCH2PM;

             CONNECT => to connect to database
             RESOURCE => to create tables 

 Testing :- 

 =>  open sqlplus 

   username :- BATCH2PM/NACRE

 changing password :- 
 
 => both user & dba can change password

  by user :- (BATCH2PM/NACRE)

 SQL>PASSWORD
    changing password for batch2pm
    old password :- NACRE
    new password :- NACRE123
    retype new password :- NACRE123
    password changed

  SQL>

  by DBA :- ( / as sysdba)

  SQL>ALTER USER BATCH2PM IDENTIFIED BY NARESH ;
 
 Datatypes in oracle :- 

 => a datatype specifies type of the data allowed in a column 
    and amount of memory allocated for column.
  
                         DATATYPES

     CHAR            NUMERIC         DATE             BINARY

ASCII      UNICODE   Number(P)       DATE             BFILE
char       nchar     Number(p,s)     TIMESTAMP        BLOB 
varchar2   nvarchar2
long       nclob
CLOB

char :- 

 => allows character data upto 2000 chars.
 => recommended for fixed lengh char columns.

   ex :-   NAME    CHAR(10)
           sachin----
                  wasted
           ravi------ 
                  wasted
 
  => in CHAR datatype extra bytes are wasted.so don't use char
 datatype for variable length columns, use char datatype for
 fixed length columns.

    ex :-    STATE_CODE   CHAR(2)

             TS
             AP
             MH
             UP

             COUNTRY_CODE  CHAR(3)

             IND
             USA
             JPN

  VARCHAR2 :- 

  => allows character data upto 4000 chars
  => recommended for variable length columns

  ex :-  NAME      VARCHAR2(10)

         SACHIN----- 
                released

=> in varchar2 extra bytes are released.

=> both char/varchar2 allows ASCII characters (256 chars) that
  includes a-z,A-Z,0-9,special chars.

         ex :- PANNO  CHAR(10)

 LONG :- allows character data upto 2GB.

 CLOB  :- allows character data upto 4GB.

  NCHAR/NVARCHAR2 :-  (N => National)

  => both allows unicode characters(65536 chars) thant includes
   all ASCII chars and also chars belongs to different languages.

  NCLOB :- allows unicode characters upto 4GB.

 Number(p) :-

 => allows numeric data upto 38 digits.
 => allows integers i.e. numbers without decimal part.

           ex :-  EMPNO   NUMBER(4)
                  10
                  100
                  1000
                  10000 => not accepted

 Number(p,s) :- 

 => allows numbers with decimal part.

   p => precision => total no of digits allowed
   s => scale     => no of digits allowed after decimal

    ex :-   SAL    NUMBER(7,2)
            
            5000
            5000.50
           50000.50
          500000.50 => INVALID
           5000.501 => VALID => 5000.50
       5000.50678356 => VALID => 5000.51

   DATE :- 

   => date allows date & time
   => but time is optional , if not entered then oracle stores 12:00 AM
   => default date format in oracle is DD-MON-YY / YYYY
   
      EX :-  DOB   DATE

            22-APR-20  => 22-APR-2020
            10-OCT-97  => 10-OCT-2097
            10-OCT-1997 => 10-OCT-1997

  TIMESTAMP :- 

  => allows date,time and also milliseconds.

        EX :-  T    TIMESTAMP
               22-APR-20 14:40:20.123
               --------  -------  ---
                 DATE    TIME     MS

 BINARY :- 

 => allows binary data that includes audio,video,images 

 1 BFILE (binary file)
 2 BLOB  (binary large object)

 => bfile is called external lob because lob is stored outside
  db but db stores path.

 => blob is called internal lob because lob stored inside db.

 creating table in oracle database :- 

 CREATE TABLE <TABNAME>
 (
   COLNAME  DATATYPE(SIZE),
   COLNAME DATATYPE(SIZE),
   ------------
  );

 Rules :- 

 1  tabname should start with alphabet.

 2  tabname should not contain spaces and special chars
    but allows $,#,_.

 3  tabname can be upto 128 chars.

 4  table can have max 1000 columns.

 5  no of rows unlimited.

 Example :- 
 
  CREATE TABLE EMP
    (
       EMPID NUMBER(4),
       ENAME VARCHAR2(10),
       JOB   VARCHAR2(10),
       SAL   NUMBER(7,2),
       HIREDATE DATE);

 => above command created table structure/definition/metadata
  that includes columns,datatype and size.

 DESC :- (DESCRIBE) 

 => command to see the table structure
 
   SQL>DESC  EMP ;

       EMPNO   	NUMBER(4)
       ENAME   	VARCHAR2(10)
       JOB     	VARCHAR2(10)
       SAL     	NUMBER(7)
       HIREDATE DATE

 Inserting data into table :- 

 => "INSERT" command is used to insert data into table.

 inserting single row :- 

  INSERT INTO <TABNAME> VALUES(V1,V2,V3,---);

 => char and date values should be in ' '

 example :- 

1  INSERT INTO EMP VALUES(100,'sachin','clerk',3000,'22-APR-20'); 

2  INSERT INTO EMP VALUES(101,'vijay','manager',8000,sysdate);

 inserting multiple rows :- 

 => insert command executed multiple times with different values
 by using variables prefixed with "&".

  syn :-  INSERT INTO <TABNAME> VALUES(&F1,&F2,&F3------);

  ex  :-  

  SQL>INSERT INTO EMP VALUES(&EMPID,&ENAME,&JOB,&SAL,&HIREDATE);
     enter value for empid :- 102
     enter value for ename :- 'satish'

     enter value for hiredate :- sysdate

  SQL> /  (executes previous command)

  => above insert commands inserted data into instance(RAM).
   to save this data execute COMMIT.

	  SQL>COMMIT; 

 inserting nulls :- 

 => null means  blank or empty
 => it is not equal to 0 or space
 => nulls can be inserted in two ways

  1 explicitly (by user)
  2 implicitly (by oracle)

 explicitly :- 

  SQL>INSERT INTO EMP VALUES(105,'suresh','',NULL,SYSDATE);

 implicitly :- 

  SQL>INSERT INTO EMP(EMPID,ENAME,HIREDATE)
               VALUES(106,'ravi',sysdate);

  remaining two columns job,sal filled with null

 Displaying Data :- 

 => "SELECT" command is used to display data from table

       SELECT <columns>/* FROM <tabname> 

          sql =  english
         queries =  sentences
         clauses =   words

         FROM clause => specify tablename
         SELECT clause => specify column names
                    *  => all columns
        
       display all the data from emp table ?

       SELECT * FROM emp ;
  
      display employee names and salaries ?

      SELECT ename,sal FROM emp ;

  Operators in oracle :- 

  Arithmetic Operators =>  +  - *  /   
  Relational Operators =>  > >=  <  <=  =  <>
  Logical Operators    =>  AND OR NOT
  Special Operators    =>  between,in,like,is,any,all,exists
  Set Operators        =>  union,union all,intersect,minus
  
  WHERE clause :- 

  => used to get specific row/rows from table based on a condition

    SELECT columns
    FROM  tabname
    WHERE condition

 condition :- 

           COLNAME OP VALUE

 => OP must be any relational operator
 => if cond = true row is selected
 => if cond = false row is not selected

  display employee details whose id = 103 ? 

  SQL>SELECT * FROM emp WHERE empid=103 ;

  display employee details whose name=satish ?

  SQL>SELECT * FROM emp WHERE ename='satish' ;

 display employee details earning more than 5000 ?

  SQL>SELECT * FROM emp WHERE sal>5000;

 display employee details joined after 2019 ?

 SQL>SELECT * FROM emp WHERE hiredate > 2019 ; => ERROR

 SQL>SELECT * FROM emp WHERE hiredate > '31-DEC-2019' ;

 employees joined before 2019 ? 

 SQL>SELECT * FROM emp WHERE hiredate < '01-JAN-2019' ;

 compound condition :-

 => multiple conditions combined with AND/OR operators is called
    compound conditioin.

    WHERE  cond1  and  cond2   result
            T           T       T
            T           F       F
            F           T       F
            F           F       F

    WHERE cond1  or   cond2    result
           T            T       T
           T            F       T
           F            T       T
           F            F       F

    employees working as clerk,manager ?

    SQL>SELECT * FROM emp WHERE job='clerk' or job='manager' ;

    employees whose id=100,103,105 ?

    SQL>SELECT * FROM emp 
          WHERE empid=100 OR empid=103 OR empid=105 ;

    employees working as clerk and earning more than 3000 ?

    SQL>SELECT * FROM emp 
              WHERE job='clerk' and  sal>3000;

   employees earning more than 5000 and less than 10000 ?

   SQL>SELECT * FROM emp
             WHERE sal>5000 and sal<10000;

   employees working as clerk,manager,analyst ?

   select * from emp 
           where job='clerk' or job='manager' or job='analyst' 

           where job='clerk','manager','analyst' => invalid

  IN operator :- 

 => use IN operator when "=" comparision with multiple values

   WHERE COLNAME IN (V1,V2,V3,----) (COL=V1 OR COL=V2 OR COL=V--)
   WHERE COLNAME NOT IN (V1,V2,V3,--)

  employees working as clerk,manager ?

  SQL>SELECT * FROM emp 
              WHERE job IN ('clerk','manager');

 employees whose id=100,103,105 ? 

 SQL>SELECT * FROM emp
              WHERE empid IN (100,103,105);

 BETWEEN operator :- 

 => use BETWEEN operator when comparision with range.
 
     WHERE COL BETWEEN V1 AND V2 (WHERE COL>=V1 AND COL<=V2)
     WHERE COL NOT BETWEEN V1 AND V2

   employees earning between 5000 and 10000 ?

  SQL>SELECT * FROM emp
           WHERE sal BETWEEN 5000 and 10000 ;

          (where sal>=5000 and sal<=10000) 

  employees joined in 2020 year ?

  SQL>SELECT * FROM emp
        WHERE hiredate BETWEEN '01-JAN-20' AND '31-DEC-20' ; 

 FAQ :-

 SQL>SELECT * FROM emp
         WHERE sal BETWEEN 10000 AND 5000;

 a error
 b no rows
 c returns rows
 d none

          WHERE sal>=10000 and sal<=5000;

 ans :- b 

 display employee list working as clerk,manager and earning
 between 2000 and 5000 and joined in 1981 year and not 
 working for dept 10,20 ?

 SELECT *
 FROM emp
 WHERE job IN ('CLERK','MANAGER')
       AND
       sal BETWEEN 2000 AND 5000
       AND
       hiredate BETWEEN '01-JAN-1981' AND '31-DEC-1981'
       AND
       deptno NOT IN (10,20);

 LIKE operator :- 

 => use LIKE operator when comparision based on patterns

     WHERE COLNAME LIKE 'pattern'
     WHERE COLNAME NOT LIKE 'pattern'

 => pattern consists of alphabets,digits,special chars and
    wildcard chars.

 wildcard chars :- 

  %  => zero or many chars
  _  => exactly 1 char

 employees name starts with 's' ?

 SELECT * FROM emp WHERE ename LIKE 'S%' ;

 employees name ends with 's' ?

 SELECT * FROM emp WHERE ename LIKE '%S'

 employees name contains 's' ?

 SELECT * FROM emp WHERE ename LIKE '%S%' ;

 where 'A' is the 3rd char in their name ?

 SELECT * FROM emp WHERE ename LIKE '__A%' ;

 where 'E' is the 2nd char from last ?

 SELECT * FROM emp WHERE ename LIKE '%E_' ;

 employees earning 5 digit salary ?

  SELECT * FROM emp WHERE sal LIKE '_____' ;

 employees joined in JAN month ?

 DD-MON-YY

 SELECT * FROM emp WHERE hiredate LIKE '%JAN%' ;

 employees joined in 1983 year ?

 SELECT * FROM emp WHERE hiredate LIKE '%83' ;
 
 IS operator :- 

 => use IS operator when comparision based on NULL / NOT NULL

    WHERE COLNAME IS NULL
    WHERE COLNAME IS NOT NULL

  Employees who are not earning comm ?

  SQL>SELECT * FROM emp WHERE comm IS NULL ;    

 Employees who are earning comm ? 

  SQL>SELECT * FROM emp WHERE comm IS NOT NULL ;

 WHERE COL BETWEEN V1 AND V2
 WHERE COL IN (V1,V2,V3,--)
 WHERE COL LIKE 'PATTERN'
 WHERE COL IS NULL
 WHERE COL IS NOT NULL

 display names and annual salaries ?

 SELECT ename,sal*12 FROM emp ;

 ALIAS :- 

 => alias means another name or alternative name
 => used to change column heading in select stmt output.

       COLNAME/EXPR [AS] ALIAS

    display names and annual salaries ?

    SELECT ename,sal*12 as annsal FROM emp ;

    SELECT ename,sal*12 as "annual salary" FROM emp ;

 => if alias contains space then enclose in in " "

   display names and experience ?

   SELECT ename,(sysdate-hiredate)/365 as experience 
   FROM emp ;

  employee details having more than 39 years of experience ?

  SELECT * 
  FROM emp
  WHERE (sysdate-hiredate)/365 > 39 ; 

  display ENAME,SAL,HRA,DA,TAX,TOTSAL ?

      HRA = 20% ON SAL
      DA  = 30% ON SAL            
      TAX = 10% ON SAL
      TOTSAL = SAL + HRA + DA - TAX 

   SELECT ename,sal,
          sal*0.2 as hra,
          sal*0.3 as da,
          sal*0.1 as tax,
          sal+(sal*0.2)+(sal*0.3)-(sal*0.1) as totsal
  FROM emp ; 

  ORDER BY clause :- 

  => ORDER BY clause is used to sort data based on one or more
   columns either in ascending or in descending order.

   SELECT columns
   FROM tabname
   [WHERE cond]
   ORDER BY <col> [ASC/DESC]

  => default order is ASC , for descending order use DESC.

  => arrange employee list name wise asc order ?

    SELECT * FROM emp ORDER BY ename ASC;

 => arrange employee list sal wise desc order ?

    SELECT * FROM emp ORDER BY sal DESC ;
      
  NOTE :- in order by clause we can use column name or column
  number.

     SELECT * FROM emp ORDER BY 6 DESC ;  

 => above query sorts data based on 6th column i.e. sal.

    SELECT empno,ename,sal,deptno
    FROM emp
    ORDER BY 6 DESC ;  => error

  note :- order by number is not based on table , it is based
          on select list.

    SELECT empno,ename,sal,deptno
    FROM emp
    ORDER BY 3 DESC ; 

  arrange employee list dept wise asc and with in dept sal wise
  desc order ?

    SELECT empno,ename,sal,deptno
    FROM emp
    ORDER BY 4 ASC,3 DESC ; 

    1 A 5000 20        5 E 5000 10
    2 B 3000 10        2 B 3000 10
    3 C 4000 30  =>    4 D 6000 20
    4 D 6000 20        1 A 5000 20 
    5 E 5000 10        3 C 4000 30

   How to see the list of tables ?

   SELECT * FROM TAB ; 

   list of users ?

   SELECT USERNAME FROM ALL_USERS ;
    
  DML commands :- 

  insert  
  update
  delete

 => these commands acts on table data.
 => all DML commands acts on instance , to save these operations
    execute commit and to cancel these operations execute rollback.

 update command :- 

 => command used to modify the data in a table.
 => using update command we can modify all rows and all cols.
 => using update command we can modify specific rows & specific cols.

  UPDATE <tabname>
  SET <colname> = <value> , <colname> = <value> --------
  [WHERE condition]

 => update all employees comm to 500 ? 

   SQL>UPDATE emp SET comm = 500 ;

 => update employees comm to 500 whose comm = null ?

   SQL>UPDATE emp SET comm=500 WHERE comm IS NULL ;

 => update comm to null whose comm <> null ?

   SQL>UPDATE emp 
       SET comm = NULL 
       WHERE comm IS NOT NULL ;

       NULL assignment  use   = 
       NULL comparision use   IS

  => update employee job to manager and sal to 3000 whose 
      empno=7369 ? 

  SQL>UPDATE emp 
      SET job='MANAGER',sal=3000
      WHERE empno=7369 ;

 => incr sal by 20% and comm by 10% those working as salesman
  and joined in 1981 year ? 

   SQL>UPDATE emp
       SET sal=sal+(sal*0.2),comm=comm+(comm*0.1)
       WHERE job='SALESMAN' and hiredate like '%81' ;

  DELETE command :- 

  => command used to delete row/rows from table
  => using delete command we can delete all rows or specific rows

    DELETE FROM <tabname> [WHERE condition]

  => delete all rows from emp table ?

    SQL>DELETE FROM emp ;

 => delete employees having more than 39 years of experience ?

   SQL>DELETE FROM emp 
          WHERE (sysdate-hiredate)/365 > 39 ; 

 DDL commands :-

 create
 alter
 drop
 truncate
 rename
 flashback
 purge

 => all DDL commands acts on table structure
 => DDL commands are auto committed.

    DDL command = DDL command + commit

 example 1 :-

  create table a(a number(2));
  insert into a values(10);
  insert into a values(20);
  insert into a values(30);
  insert into a values(40);
  rollback;  

  => create table is saved and insert commands are cancelled

  select * from a ;

  no rows selected

 example 2 :- 

   create table a(a number(2));
   insert into a values(10);
   insert into a values(20);
   create table b(b number(2));
   insert into a values(30);
   insert into a values(40);
   rollback;  

  => insert 10,20 are saved insert 30,40 are cancelled

  select * from a ;

  10
  20 
   
 ALTER command :- 

 => command used to modify table structure
 => using ALTER command we can

  1 add columns
  2 drop columns
  3 rename column
  4 modify a column 
         incr/decr field size
         changing datatype

 adding column :- 
 
 ALTER TABLE <TABNAME>
       ADD(COLNAME DATATYPE(SIZE),----);

 add column gender to emp table ?        
 
 SQL>ALTER TABLE emp
          ADD(gender CHAR(1)); 

=>  by default this new column is filled with NULLs. To insert
 data into this new column use UPDATE command.

  SQL>UPDATE emp
      SET gender='M'
      WHERE empno=7369 ;

 =>  update all employee genders with diffent values ?

  SQL>UPDATE emp
      SET gender='&GENDER'
      WHERE empno=&empno;

 Droping column :- 

 ALTER TABLE <tabname>
     DROP (COL1,COL2,--------);

 =>drop gender from emp table ?

  SQL>ALTER TABLE emp
             DROP(gender);
 
 renaming a column :- 

  ALTER TABLE <TABNAME>
          RENAME COLUMN <OLDNAME> TO <NEWNAME> ;

 => change the column name COMM to BONUS ?

  SQL>ALTER TABLE emp 
          RENAME COLUMN COMM TO BONUS ;

   SELECT ENAME,SAL,COMM AS BONUS FROM EMP ;

   diff b/w rename & alias ? 

          rename           alias 

      1 permanent         not permanent

      2 changes column    changes column heading in
        name in table     select stmt output

 Modifying a column :- 

  1 incr/decr field size
  2 changing datatype

  ALTER TABLE <TABNAME>
        MODIFY (COLNAME DATATYPE(SIZE));

  incr size of ename to 20 ? 

  SQL>ALTER TABLE EMP
         MODIFY(ENAME VARCHAR2(20));

  SQL>ALTER TABLE EMP
         MODIFY(ENAME VARCHAR2(5));  => ERROR

  => char field size can be decreased upto the max length.

  => numeric field must be empty to decrese size

  SQL>ALTER TABLE EMP
          MODIFY(SAL NUMBER(6,2)); => ERROR

  => column must be empty to change datatype.

  SQL>ALTER TABLE EMP
          MODIFY(EMPNO VARCHAR2(10)); => ERROR
  
  DROP command :- 

  => drops the table from database.
  => drops table structure along with data.

      DROP TABLE <tabname> ;

   ex :- SQL>DROP TABLE EMP ;

 => before 10g if table is dropped then it is permanent deleted
    from database and cannot be restored.

 => from 10g onwards when table is dropped then it is moved to
    recyclebin.To see the recyclebin execute the following
    command

   SQL>SHOW RECYCLEBIN

  FLASHBACK command :- 

  => introduced in 10g ver.
  => command used to restore the table from recyclebin.
  => useful to recover the table if it is dropped accidentally

     FLASHBACK TABLE <TABNAME> TO BEFORE DROP;

    SQL>FLASHBACK TABLE EMP TO BEFORE DROP;   

  PURGE command :- 

  => introduced in 10g
  => used to delete the object from recyclebin.
  => after deleting object from recyclebin flashback will not 
          work.

    PURGE TABLE <TABNAME> 

    Ex :- SQL>PURGE TABLE EMP ;

          SQL>DROP TABLE EMP PURGE ;

    => above commands drops table and also deletes the table from
        recyclebin.

  RENAME :- used to change tablename

    RENAME <OLDNAME> TO <NEWNAME> 

    SQL>RENAME EMP TO EMPLOYEES ;

 TRUNCATE :- 

 => deletes all the data from table but keeps structure.
 => will empty the table.
 => releases memory allocated for table.

       TRUNCATE TABLE <tabname> 

  ex :-  SQL>TRUNCATE TABLE EMP ;

  DROP VS TRUNCATE VS DELETE :- 

  1  drop vs truncate/delete 

      DROP                   TRUNCATE/DELETE
 
   drops structure with data  deletes only the data but keeps structure

 2  truncate vs delete :- 

     TRUNCATE               DELETE
 
 1   DDL command            DML command

 2  deletes all rows but     can delete specific row/rows
    can't delete specific
    row/rows

 3  where cond can't be      where cond can be used with 
    used with truncate       delete

 4  cannot be rolledback      can be rolledback

 5  deletes all rows at       deletes row-by-row
    a time

 6  faster                   slower

 7  releases memory          will not release memory

		         chapter 2   
 
		   Integrity Constraints	

 => Integrity Constraints are rules to maintain data integrity
    i.e. data quality.

 => used to prevent users from entering invalid data.

 => used to enforce rules like min sal must be 3000.

                   integrity constraints

  Entity Integrity     Domain Integrity    Refrential Integrity

  unique               not null            foreign key
  primary key          check
                       default

 => above constraints can be declared in two ways 

  1  column level
  2  table level

 column level :- 

 => if constraints are declared immediately after declaring
  column is called column level.

  CREATE TABLE <TABNAME>
   (
    COLNAME DATATYPE(SIZE) CONSTRAINT,
    -------------);

 NOT NULL :- 

 => not null constraint doesn't accept nulls
 => if column declared with NOT NULL then it is called mandatory column

  CREATE TABLE EMP11
   (
      EMPNO NUMBER(4),
      ENAME VARCHAR2(10) NOT NULL);

  INSERT INTO EMP11 VALUES(100,'A');
  INSERT INTO EMP11 VALUES(101,'');  => ERROR

 UNIQUE :- 

 => unique constraint doesn't accept duplicates
 
  CREATE TABLE EMP12
   (
     EMPNO NUMBER(4),
     EMAILID VARCHAR2(20) UNIQUE
   );

  INSERT INTO EMP12 VALUES(100,'abc@gmail.com');
  INSERT INTO EMP12 VALUES(101,'abc@gmail.com'); => ERROR
  INSERT INTO EMP12 VALUES(102,'');
  INSERT INTO EMP12 VALUES(103,'');

 PRIMARY KEY :- 

 => primary key doesn't accept duplicates and nulls
 => primary key is the combination of unique & not null

       PRIMARY KEY = UNIQUE + NOT NULL

   CREATE TABLE EMP13
    (
       EMPNO NUMBER(4) PRIMARY KEY,
       ENAME VARCHAR2(10)
    );

  INSERT INTO EMP13 VALUES(100,'A');
  INSERT INTO EMP13 VALUES(100,'B'); => ERROR
  INSERT INTO EMP13 VALUES(NULL,'C'); => ERROR

  => PRIMARY KEY is used to uniquely identify the records
    in a table.

  => a table allows only one primary key , if we want two 
   primary keys then declare one column with primary key
   and another column unique & not null.

   CREATE TABLE CUST
     (
       ACCNO  NUMBER(4) PRIMARY KEY,
       NAME   VARCHAR2(10) NOT NULL,
       AADHARNO  NUMBER(12) UNIQUE NOT NULL);

   diff b/w primary key & unique not null ?

    primary key                  unique not null

  a table can have only         a table can have multiple
  one primary key                 unique & not null

  CHECK constraint :- 

  => use check constraint when rule based on condition.

       syn :-  CHECK(condition)
 
 ex :- 1   sal must be min 3000

       CREATE TABLE EMP14
        (
         EMPNO NUMBER(4),
         ENAME VARCHAR2(10),
         SAL  NUMBER(7) CHECK(SAL>=3000)
        );

    INSERT INTO EMP14 VALUES(100,'A',5000);
    INSERT INTO EMP14 VALUES(101,'B',1000); => ERROR
    INSERT INTO EMP14 VALUES(102,'C',NULL); => accepted

   => check constraint allows nulls.

    2  gender must be 'M','F' ?

       GENDER CHAR(1) CHECK(GENDER IN ('M','F'))

    3  amt must be multiple of 100 ? 

        AMT NUMBER(5) CHECK(MOD(AMT,100)=0)

    4  pwd must be min 8 chars ?

        pwd  VARCHAR2(10) CHECK(length(pwd)>=8)
   
  FOREIGN KEY :- 

  => foreign key is used to establish relationship between two 
   tables.

  => to establish relationship between two tables , take primary 
  key of one table and add it to another table as foreign key

   DEPT
   DEPTNO  DNAME  LOC 
   10      HR     MUM
   20      IT     HYD
   30      SALES  BLR

   EMP
   EMPNO   ENAME   SAL    DEPTNO  REFERENCES DEPT(DEPTNO)  
   1       A       5000    10
   2       B       3000    20
   3       C       4000    90 => ERROR
   4       D       2000    10 
   5       E       1000    NULL 

 => values entered in fk column should match with values 
   entered in primary key.

 => fk allows duplicates and nulls

 => after declaring fk a relationship is established between
  two table called parent/child relationship.

 => primary key table is parent and fk table is child.

  CREATE TABLE DEPT55
   (
     DEPTNO NUMBER(2) PRIMARY KEY,
     DNAME VARCHAR2(10) UNIQUE NOT NULL,
     LOC VARCHAR2(10));

   INSERT INTO DEPT55 VALUES(10,'HR','MUM');
   INSERT INTO DEPT55 VALUES(20,'IT','HYD');

  CREATE TABLE EMP55
   (
    EMPNO NUMBER(4) PRIMARY KEY,
    ENAME VARCHAR2(10) NOT NULL,
    SAL   NUMBER(7,2) CHECK(SAL>=3000),
    DEPTNO NUMBER(2) REFERENCES DEPT55(DEPTNO)
   );

 INSERT INTO EMP55 VALUES(1,'A',5000,10);
 INSERT INTO EMP55 VALUES(2,'B',3000,90); => ERROR
 INSERT INTO EMP55 VALUES(3,'C',3000,10);
 INSERT INTO EMP55 VALUES(4,'D',4000,NULL);

 DEFAULT :- 

 => a column can be declared with default value as follows

    ex :- HIREDATE DATE DEFAULT SYSDATE

 => while inserting if we skip hiredate then oracle inserts
  default value.

  CREATE TABLE EMP17
   (
    EMPNO NUMBER(4),
    HIREDATE DATE DEFAULT SYSDATE);

  INSERT INTO EMP17(EMPNO) VALUES(100);
  INSERT INTO EMP17 VALUES(101,'01-JAN-20');
  INSERT INTO EMP17 VALUES(102,'');

  SELECT * FROM EMP17 ;

  EMPNO   HIREDATE
  100     30-APR-20
  101     01-JAN-20
  102     

 TABLE LEVEL :- 

 => if constraints are declared after declaring all columns
 then it is called table level.

 => use table level to declare constraints for multiple or
 combination of columns.

  CREATE TABLE <TABNAME>
   (
     COLNAME DATATYPE(SIZE),
     COLNAME DATATYPE(SIZE),
            CONSTRAINT(collist)
   );

 Declaring check constraint table level :- 

 MANAGERS
 MGRNO   MNAME   START_DATE  END_DATE
 100     A       30-APR-20   01-JAN-20      => INVALID

 RULE :-  END_DATE > START_DATE 

 => above rule based on multiple columns so declare the 
  constraint at table level.

 CREATE TABLE MANAGERS
  (
   MGRNO NUMBER(4),
   MNAME VARCHAR2(10),
   START_DATE DATE ,
   END_DATE DATE ,
          CHECK(END_DATE > START_DATE)
  );
          
 INSERT INTO MANAGERS VALUES(100,'A',SYSDATE,'01-JAN-20'); => ERROR
 INSERT INTO MANAGERS VALUES(101,'B','01-JAN-20',SYSDATE);
 
 composite primary key :- 

 => if primary key declared for combination of columns then it
 is called composite primary key.

 => if combination declared primary key then combination should
  not be duplicate.

  STUDENT               COURSE
  SID   SNAME           CID   CNAME
  1     A               10    ORACLE
  2     B               11    JAVA

  REGISTRATIONS
  SID  CID   DOR   FEE
  1    10    ??    ??
  1    11    ??    ??
  2    10    ??    ??

 => in the above example SID,CID combination uniquely identifies
  records in the table.so declare this combination as primary  
  key at table level.

  CREATE TABLE REGISTRATIONS
   (
     SID NUMBER(2),
     CID NUMBER(2),
     DOR DATE,
     FEE NUMBER(5),
            PRIMARY KEY(SID,CID)
   ) 

  INSERT INTO REGISTRATIONS VALUES(1,10,SYSDATE,1000); 
  INSERT INTO REGISTRATIONS VALUES(1,11,SYSDATE,1000);
  INSERT INTO REGISTRATIONS VALUES(2,10,SYSDATE,1000);
  INSERT INTO REGISTRATIONS VALUES(1,10,SYSDATE,1000); => ERROR
 
  composite foreign key :- 

  => if combination of columns declared foreign key then it is
 called composite foreign key.

 => a composite foreign key refers composite primary key

 
  REGISTRATIONS
  SID  CID   DOR   FEE
  1    10    ??    ??
  1    11    ??    ??
  2    10    ??    ??
 
  CERTIFICATES
  CERTNO  DOI  SID   CID
  1000    ??   1     10
  1001	  ??   1     11  
  1002	  ??   2     11

 => in the above example SID,CID combination should match with    
    registrations table SID,CID combination.so declare this
    combination as fk that refers registrations table pk.

  CREATE TABLE CERTIFICATES
    (
      CERTNO NUMBER(4),
      DOI DATE,
      SID NUMBER(2),
      CID NUMBER(2),
          FOREIGN KEY(SID,CID) REFERENCES REGISTRATIONS(SID,CID)
   );

  which of the following constraint cannot be declared at 
 table level ?

  a unique
  b primary key
  c not null
  d check
  e foreign key

  ans :-  c  

  Adding constraints to existing table :- 

=>  "ALTER" command is used to add constraints to existing table.
   
  CREATE TABLE EMP66
   (
     EMPNO NUMBER(4),
     ENAME VARCHAR2(10),
     SAL  NUMBER(7,2),
     DNO NUMBER(2));

   SQL>ALTER TABLE EMP66 ADD PRIMARY KEY(EMPNO);
   SQL>ALTER TABLE EMP66 ADD CHECK(SAL>=3000);
   SQL>ALTER TABLE EMP66 
        ADD FOREIGN KEY(DNO) REFERENCES DEPT55(DEPTNO);
   SQL>ALTER TABLE EMP66 MODIFY(ENAME NOT NULL);

  Droping constraints :- 

   ALTER TABLE <TABNAME>
         DROP CONSTRAINT <NAME> ;
   
  USER_CONSTRAINTS :- 

 => system table that stores information about constraints declared
  in a table.
 
  SELECT CONSTRAINT_NAME,CONSTRAINT_TYPE,
          SEARCH_CONDITION
  FROM USER_CONSTRAINTS
  WHERE TABLE_NAME='EMP66' ;
 
 SQL>ALTER TABLE EMP66
      DROP CONSTRAINT SYS_C0011690 ;
    
 SQL>ALTER TABLE EMP66
           DROP PRIMARY KEY ;

 SQL>ALTER TABLE DEPT55
          DROP PRIMARY KEY ; => ERROR

 => PRIMARY KEY cannot be dropped if referenced by some fk.

 SQL>ALTER TABLE DEPT55
         DROP PRIMARY KEY CASCADE ;  

  => drops pk and also drops dependent foreign key.

 
 importance of constraints
 types of constraints
 declaring constraints
   column level
   table level
 adding constraints to existing table
 droping constraints
 getting constraints information

			joins

  => join is an operation performed to get data from two or 
  more tables. To get data from two tables we need to join those
 two tables.

 => in DB tables are normalized i.e. related data stored in
   multiple tables.if we want to combine this data stored 
   in multiple tables then we need to join those tables.

  Types of joins :- 

  1 Equi Join / Inner join
  2 Outer join
       left outer
       right outer
       full outer
  3 Non Equi Join
  4 Self join
  5 Cross join / Cartisean join

 Equi Join / Inner join :- 

 => to perform equi join between the two tables there must be
 a common field and name of the common field need not to be
 same and pk-fk relationship is not compulsory.

  SELECT columns
  FROM tabnames
  WHERE join condition ;

 join condition :- 

 => based on the given join condition oracle joins the records
 of two tables.
 
   TABLE1.COMMONFIELD = TABLE2.COMMONFIELD

  EMP					DEPT
  EMPNO  ENAME  SAL  DEPTNO		DEPTNO DNAME 	LOC
  1	 A	5    10			10     ACCT  	HYD
  2	 B	4    20			20     RESEARCH	
  3	 C	3    30			30     SALES
  4	 D	4    10			40     OPERATIONS
  5	 E	3    NULL

 display  ENAME,SAL,DNAME  ?

 SELECT ENAME,SAL,DNAME
 FROM EMP,DEPT
 WHERE EMP.DEPTNO = DEPT.DEPTNO ; 

  A   5   ACCT
  B   4   RESEARCH
  C   3   SALES
  D   4   ACCT

 display ENAME,SAL,DEPTNO,DNAME ?

 SELECT ENAME,SAL,DEPTNO,DNAME
 FROM EMP,DEPT
 WHERE EMP.DEPTNO = DEPT.DEPTNO ;  => ERROR

 => in join queries declare table alias and prefix column 
  names with table alias for two reasons

 1 to avoid ambiguity
 2 for faster execution

 SELECT E.ENAME,E.SAL,D.DEPTNO,D.DNAME,D.LOC AS CITY
 FROM EMP E,DEPT D
 WHERE E.DEPTNO = D.DEPTNO ;

 display ENAME,DNAME,LOC working at NEW YORK loc ?

 SELECT E.ENAME,E.SAL,D.DEPTNO,D.DNAME,D.LOC AS CITY
 FROM EMP E,DEPT D
 WHERE E.DEPTNO = D.DEPTNO 
       AND
       D.LOC='NEW YORK' ;

 => we can write join queries in 2 styles 

  1 Native style (oracle style)
  2 ANSI style

 ANSI style :- (American National Standard Institute)

 => introduced in oracle 9i.
 => Adv of ANSI style is portability.
 => ANSI style gurantees portability but Native style doesn't
    gurantees portability.
 => in ANSI style tablenames are seperated by keywords and
    use ON clause for join conditions instead of WHERE clause.

   
  SELECT E.ENAME,E.SAL,D.DNAME
  FROM EMP E INNER JOIN DEPT D
    ON E.DEPTNO = D.DEPTNO 

 Outer join :- 

 => Equi join returns only matching records but can't return
 unmatched records , to get unmatched records also perform
  outer join.

 => outer join is 3 types 

   l left outer join
   2 right outer join
   3 full outer join

  EMP					DEPT
  EMPNO  ENAME  SAL  DEPTNO		DEPTNO DNAME 	LOC
  1	 A	5    10			10     ACCT  	HYD
  2	 B	4    20			20     RESEARCH	
  3	 C	3    30			30     SALES
  4	 D	4    10			40     OPERATIONS => unmatched
  5	 E	3    NULL => unmatched 

  left outer join :- 

 => returns all rows(matched + unmatched) from left side table 
    and matching rows from right side table.

    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E ,DEPT D
    WHERE E.DEPTNO = D.DEPTNO(+) ;

 => above query returns all rows from emp and matching rows from
  dept table.

    A   4000  ACCT
    B   3000  RESEARCH
    C   2000  SALES
    D   5000  ACCT
    E   3000  NULL  => unmatched record from left side table.

 right outer join :- 

 => returns all rows (matched + unmatched) from right side table
 and matching rows from left side table.

    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E ,DEPT D
    WHERE E.DEPTNO(+) = D.DEPTNO ;

    A   4000  ACCT
    B   3000  RESEARCH
    C   2000  SALES
    D   5000  ACCT
              OPERATIONS => unmatched from dept

   full outer :- 

   => returns all rows from both tables 

    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E ,DEPT D
    WHERE E.DEPTNO(+) = D.DEPTNO(+) ; => error

 => (+) cannot be on both sides.
 => Native style doesn't support full outer join only ANSI 
    style supports full outer join.
 => in Native style to perform full outer join combine the
   outputs of left outer & right outer by using UNION operator.
 
  A=1,2,3,4
  B=1,2,5,6

  AUB = 1,2,3,4,5,6

    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E ,DEPT D
    WHERE E.DEPTNO  = D.DEPTNO(+) 
    UNION
    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E ,DEPT D
    WHERE E.DEPTNO(+) = D.DEPTNO  
 
   
    A   4000  ACCT
    B   3000  RESEARCH
    C   2000  SALES
    D   5000  ACCT
    E   3000  NULL     => unmatched from emp
              OPERATIONS => unmatched from dept

  ANSI style :- 

  left outer join :- 

    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E LEFT OUTER JOIN DEPT D
      ON E.DEPTNO  = D.DEPTNO ; 
 
  right outer join :- 

    SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E RIGHT OUTER JOIN DEPT D
      ON E.DEPTNO  = D.DEPTNO ; 

  full outer join :- 

      SELECT E.ENAME,E.SAL,D.DNAME
    FROM EMP E FULL OUTER JOIN DEPT D
      ON E.DEPTNO  = D.DEPTNO ; 
 
 Non Equi Join :- 

 => Non Equi Join is performed between two tables not sharing
 a common field.

  EMP                              SALGRADE
  EMPNO	 ENAME  SAL                GRADE   LOSAL   HISAL
  1       A     3500               1       700     1000               
  2       B     2000               2       1001    2000
  3       C     5000               3       2001    3000
  4       D     1500               4       3001    4000
  5       E     3000               5       4001    9999

  display ENAME,SAL,GRADE  ? 

  SELECT ENAME,SAL,GRADE
  FROM EMP E,SALGRADE S
  WHERE E.SAL BETWEEN S.LOSAL AND S.HISAL ; 

  A   3500  4
  B   2000  2
  C   5000  5
  D   1500  2
  E   3000  3

 Display grade 3 employee list ?

  SELECT ENAME,SAL,GRADE
  FROM EMP E,SALGRADE S
  WHERE E.SAL BETWEEN S.LOSAL AND S.HISAL /* join condition */
        AND
        S.GRADE = 3   /* filter cond */ 

 joining more than 2 tables :- 

 => no of join conditions is based on no of tables to be joined.
  to join N tables N-1 join conditions required.

 display ENAME,DNAME,GRADE  ?

 SELECT E.ENAME,D.DNAME,S.GRADE
 FROM EMP E,DEPT D,SALGRADE S
 WHERE E.DEPTNO = D.DEPTNO
       AND
       E.SAL BETWEEN S.LOSAL AND S.HISAL ;

 ANSI style :- 

 SELECT columns
 FROM tab1 join tab2
   ON cond
           join tab3
   ON cond

 SELECT E.ENAME,D.DNAME,S.GRADE
 FROM EMP E INNER JOIN DEPT D
   ON E.DEPTNO = D.DEPTNO
            JOIN SALGRADE S
   ON E.SAL BETWEEN S.LOSAL AND S.HISAL ;

 Self Join :- 

 => joining table to itself is called self join or recursive join.

 => in self join a record in one table joined with another record
    of same table.

  EMP 
  EMPNO  ENAME  MGR
  1      A      NULL
  2      B      1 
  3      C      1
  4      D      2
  5      E      3

 => above table contains EMPNO and MGR numbers but to display
   manager name we need to perform self join.

 => to perform self join the same table must be declared two times
  with different alias.

         
             FROM EMP X,EMP Y


   EMP X                          EMP Y
  EMPNO  ENAME  MGR               EMPNO  ENAME  MGR
  1      A      NULL               1     A      NULL
  2      B      1                  2     B      1
  3      C      1                  3     C      1
  4      D      2                  4     D      2
  5      E      3                  5     E      3

  display employee name & manager name ? 

  SELECT X.ENAME,Y.ENAME AS MANAGER
  FROM EMP X,EMP Y
  WHERE X.MGR = Y.EMPNO 

  B   A 
  C   A
  D   B
  E   C

 display employee list reporting to blake ? 

  SELECT X.ENAME,Y.ENAME AS MANAGER
  FROM EMP X,EMP Y
  WHERE X.MGR = Y.EMPNO
        AND
        Y.ENAME='BLAKE' ;

 display blake's manager name ? 

  SELECT X.ENAME,Y.ENAME AS MANAGER
  FROM EMP X,EMP Y
  WHERE X.MGR = Y.EMPNO
        AND
        X.ENAME='BLAKE' ;

 Display employees earning more than their managers ? 

   SELECT X.ENAME,X.SAL,
          Y.ENAME AS MANAGER,Y.SAL AS MGRSAL
   FROM EMP X,EMP Y
   WHERE X.MGR = Y.EMPNO
         AND
         X.SAL > Y.SAL ;

 Display employees joined before their manager ? 
 
   SELECT X.ENAME,X.HIREDATE,
          Y.ENAME AS MANAGER,Y.HIREDATE AS MGRHIRE
   FROM EMP X,EMP Y
   WHERE X.MGR = Y.EMPNO
         AND
         X.HIREDATE < Y.HIREDATE ;
 
 ANSI STYLE :- 

  Display employees joined before their manager ? 
 

   SELECT X.ENAME,X.HIREDATE,
          Y.ENAME AS MANAGER,Y.HIREDATE AS MGRHIRE
   FROM EMP X JOIN EMP Y
     ON  X.MGR = Y.EMPNO
         AND
         X.HIREDATE < Y.HIREDATE ;

  display  ENAME  DNAME   GRADE  MNAME  ?

  SELECT E.ENAME,D.DNAME,S.GRADE,M.ENAME
  FROM EMP E INNER JOIN DEPT D
    ON E.DEPTNO=D.DEPTNO
             JOIN SALGRADE S
    ON E.SAL BETWEEN S.LOSAL AND S.HISAL
             JOIN EMP M
    ON E.MGR = M.EMPNO 

   
  exercise :- 

  TEAMS
  ID   COUNTRY
  1     IND
  2     AUS
  3     SA

  OUTPUT :- 

  IND VS AUS
  IND VS SA
  AUS VS SA 

 write a query to produce the above output ? 

 cross join / cartisean join :- 

 => cross join returns cross product or cartisean product of 
 two tables 

  A=1,2
  B=3,4
  AXB = (1,3) (1,4) (2,3) (2,4)  

 => if cartisean join performed between two tables then each
 record of 1st table joined with each and every record of
 second table.

 => oracle performs cross join if submit the join query without join
 condition.

 SELECT E.ENAME,D.DNAME
 FROM EMP E,DEPT D ;
   
 importance of join
 types of joins
 equi join
 outer join
 non equi
 self join
 cartisean / cross join
 ANSI style

 SET OPERATORS :- 

 UNION
 UNION ALL
 INTERSECT
 MINUS

 A=1,2,3,4
 B=1,2,5,6

 A U B   = 1,2,3,4,5,6
 A UA B  = 1,2,3,4,1,2,5,6
 A INT B = 1,2
 A-B     = 3,4
 B-A     = 5,6

 SELECT STATEMENT 1
 UNION / UNION ALL / INTERSECT / MINUS
 SELECT STATEMENT 2 ;

 => in ORACLE set operations are performed between records
 return by two select statements.

 SELECT job FROM emp WHERE deptno=20 ;

 CLERK
 MANAGER 
 ANALYST
 CLERK
 ANALYST 

 SELECT job FROM emp WHERE deptno=30 ;

 SALESMAN
 SALESMAN
 SALESMAN
 MANAGER
 SALESMAN
 CLERK

 UNION :- 

 => combines rows return by two select stmts
 => eliminates duplicates
 => sorts result

 SELECT job FROM emp WHERE deptno=20
 UNION
 SELECT job FROM emp WHERE deptno=30 ; 

 ANALYST
 CLERK
 MANAGER  
 SALESMAN

 UNION ALL :- 

 => combines output of two queries
 => duplicates are not eliminated
 => result is not sorted 
  
FAQ  diff b/w UNION & UNION ALL ?

       UNION                  UNION ALL

 1  eliminates duplicates    duplicates are not eliminated
 2  result is sorted         result is not sorted 
 3  slower                   faster

 SELECT job FROM emp WHERE deptno=20
 UNION ALL
 SELECT job FROM emp WHERE deptno=30 ; 

 CLERK
 MANAGER
 ANALYST
 CLERK
 ANALYST
 SALESMAN
 SALESMAN
 SALESMAN
 MANAGER
 SALESMAN
 CLERK

 FAQ :- diff b/w union & join ? 

     T1        T2
     F1        C1
     1         4
     2         5
     3         6

  T1 U T1 =  1
             2
             3
             4
             5
             6

 T1 JOIN T2  =    1     4
                  2     5
                  3     6


           UNION                 JOIN 

  1  merges data horizontally    merges data vertically 
  2  combines rows               combines columns
  3  performed between two       performed between two 
     similar structures           dissimilar structure

 example :- 

  EMP_US
  ENO  ENAME  SAL  DNO
                                      DEPT
  EMP_IND                             DNO  DNAME  LOC
  ENO  ENAME  SAL   DNO

  1 total employees list ? 

   SELECT * FROM EMP_US
   UNION
   SELECT * FROM EMP_IND ; 

 2 list of employees working at US loc with dept details ? 

   SELECT E.*,D.*
   FROM EMP_US E,DEPT D
   WHERE E.DNO=D.DNO

 3 total employees with dept details ? 

   SELECT E.*,D.*
   FROM EMP_US E,DEPT D
   WHERE E.DNO=D.DNO
   UNION
   SELECT E.*,D.*
   FROM EMP_IND E,DEPT D
   WHERE E.DNO=D.DNO ;

  INTERSECT :- 

  => returns common values from the output of two select stmts.

    SELECT job FROM emp WHERE deptno = 20 
    INTERSECT
    SELECT job FROM emp WHERE deptno = 30 ;

    CLERK
    MANAGER

 MINUS :- 

 => returns values present in 1st query output and not present
  in 2nd query output.

  
    SELECT job FROM emp WHERE deptno = 20 
    MINUS
    SELECT job FROM emp WHERE deptno = 30 ;
 
    ANALYST 
 

    SELECT job FROM emp WHERE deptno = 30 
    MINUS
    SELECT job FROM emp WHERE deptno = 20 ;

    SALESMAN

 CASE statement :- 

 => case statement is similar to switch case
 => used to implement IF-THEN-ELSE
 => introduced in oracle 9i
 => case statements are 2 types 

    1 simple case
    2 searched case 

 1 simple case :- 

 => use simple case when condition based on "=" operator.
 
   CASE EXPR
   WHEN VALUE1 THEN RETURN EXPR1
   WHEN VALUE2 THEN RETURN EXPR2
   -----------------
   ELSE RETURN EXPR
   END

 Example 1 :- 

  display ENAME,JOB  ? 
  
       if job=CLERK display WORKER
              MANAGER       BOSS
              PRESIDENT     BIG BOSS
              OTHERS        EMPLOYEE
  SELECT ENAME,
        CASE JOB
        WHEN 'CLERK' THEN 'WORKER'
        WHEN 'MANAGER' THEN 'BOSS'
        WHEN 'PRESIDENT' THEN 'BIG BOSS'
        ELSE 'EMPLOYEE'
        END AS JOB
 FROM EMP ;

 Example 2 :- 

 increment employee salaries as follows ? 
 
 if deptno=10 incr sal by 10%
           20             15%
           30             20%
          others          5% 

  UPDATE EMP 
  SET SAL = CASE DEPTNO
            WHEN 10 THEN SAL+(SAL*0.1)
            WHEN 20 THEN SAL+(SAL*0.15)
            WHEN 30 THEN SAL+(SAL*0.2)
            ELSE SAL+(SAL*0.05)
            END
 
 Example 3 :- 
 
  display  ENAME,SAL,DEPTNO ?

              if deptno=10 display TEN
                        20         TWENTY
                        30         THIRTY
                       OTHERS      OTHERS 

searched case :- 

=> use searched case when conditions not based on "=" operator.

 CASE 
 WHEN COND1 THEN RETURN EXPR1
 WHEN COND2 THEN RETURN EXPR2
 ---------------
 [ELSE RETURN EXPR]
 END

 display ENAME,SAL,SALRANGE ? 

            if sal>3000 display HISAL
               sal<3000 display LOSAL
               sal=3000 display AVGSAL

  SELECT ename,sal,
         case 
         when sal>3000 then 'Hisal'
         when sal<3000 then 'Losal'
         else 'Avgsal'
         end as salrange
  FROM emp ; 

 Example 2 :- 

  STUDENT
  SNO  SNAME  S1   S2  S3 
  1    A      80   90  70
  2    B      30   60  50

  display SNAME,TOTAL,AVG,RESULT ?

 
  SELECT SNAME,
         S1+S2+S3  AS TOTAL,
         (S1+S2+S3)/3 AS AVG,
         CASE 
         WHEN S1>=35 AND S2>=35 AND S3>=35 THEN 'PASS' 
         ELSE 'FAIL'
         END AS RESULT
  FROM STUDENT 

 GROUP functions :- 

 1 MAX()
 2 MIN()
 3 SUM()
 4 AVG()
 5 COUNT(*)

 MAX() :- returns maximum value.

    MAX(arg) 

 SQL>SELECT MAX(SAL) FROM EMP ;  => 5000
 
 SQL>SELECT MAX(HIREDATE) FROM EMP ; => 12-JAN-83

 MIN() :- returns minimum value

    MIN(arg)

 SQL>SELECT MIN(SAL) FROM EMP ;

 SUM() :- returns total 

    SUM(arg)

 SQL>SELECT SUM(SAL) FROM EMP ;   => 33225

 display total sal paid to managers ? 

 SQL>SELECT SUM(SAL) FROM EMP WHERE JOB='MANAGER' ; => 8275

 AVG() :- returns average 

 AVG(arg) 

 SQL>SELECT AVG(SAL) FROM EMP ; => 2215

 COUNT(*) :- returns no of rows in a table

 SQL>SELECT COUNT(*) FROM EMP ; => 15

 count no of employees joined in 1981 year ? 

 SQL>SELECT COUNT(*) FROM EMP
             WHERE HIREDATE LIKE '%81' ;

   WHERE HIREDATE BETWEEN '01-JAN-1981' AND '31-DEC-1981'
   WHERE HIREDATE LIKE '%81'

 TO_CHAR() :- 

 => function used to extract part of the date.

       TO_CHAR(date,format)

    examples :- 

    TO_CHAR(SYSDATE,'YYYY')  =>  2020
    TO_CHAR(SYSDATE,'MM')    =>  04
    TO_CHAR(SYSDATE,'MON')   =>  APR
    TO_CHAR(SYSDATE,'MONTH') =>  APRIL
    TO_CHAR(SYSDATE,'DD')    =>  08
    TO_CHAR(SYSDATE,'DAY')   =>  FRIDAY
    TO_CHAR(SYSDATE,'DY')    =>  FRI  
    TO_CHAR(SYSDATE,'D')     =>  6  
    TO_CHAR(SYSDATE,'HH')    =>  2
    TO_CHAR(SYSDASTE,'HH24') =>  14
    TO_CHAR(SYSDATE,'MI')    =>  minutes
    TO_CHAR(SYSDATE,'SS')    =>  seconds
    TO_CHAR(SYSDATE,'AM')    =>  AM/PM

 => by default sysdate will display only date

  SQL>SELECT SYSDATE FROM DUAL ; => 08-MAY-20

=> to display date & time then execute the following query
    
    SELECT TO_CHAR(SYSDATE,'MM/DD/YYYY HH:MI:SS AM')
    FROM DUAL ; 

    05/08/20 3:31:21 PM

  how many employees joined on sunday ? 

  SQL>SELECT COUNT(*) FROM EMP 
            WHERE TO_CHAR(HIREDATE,'DY') = 'SUN' ;

 GROUP BY clause :-  

 => GROUP BY clause is used to group rows based on one or
  more columns to calculate min,max,sum,avg,count for each 
  group.

 
 1  A  5000   20                       10   9000
 2  B  3000   10                       20   9000
 3  C  4000   30    ------GROUP BY---> 30   4000
 4  D  4000   20
 5  E  6000   10

 => group by clause converts detailed data to 
 summarized data which is useful for analysis.

 SELECT columns
 FROM tabname
 [WHERE condition]
 GROUP BY <col>
 [HAVING <condition]
 [ORDER BY <col>]

 Execution :- 

 FROM
 WHERE
 GROUP BY
 HAVING
 SELECT
 ORDER BY 

 display dept wise total salaries ? 

 SELECT  deptno,sum(sal)
 FROM emp 
 GROUP BY deptno 
 ORDER BY deptno asc ;

  10  7450
  20  11075
  30  9400
  40  1300

  display job wise no of employees ?

  SELECT job,count(*)
  FROM emp 
  GROUP BY job 
  ORDER BY job asc ;

  display year wise no of employees joined ? 

  SELECT TO_CHAR(hiredate,'YYYY') AS YEAR,count(*)
  FROM emp
  GROUP BY TO_CHAR(hiredate,'YYYY')  
  ORDER BY 1 ASC ; 

  display month wise no of employees joined ?

  display day of the week wise no of employees joined ? 

     
  display dept wise total sal where deptno=10,20 ? 

 SELECT  deptno,sum(sal)
 FROM emp
 WHERE deptno IN (10,20) 
 GROUP BY deptno 
 ORDER BY deptno asc ;


 FROM emp :- 

 1  A 5000 10
 2  B 6000 20
 3  C 4000 30
 4  D 4000 10
 5  E 5000 20

 WHERE deptno IN (10,20) :- 

   1  A 5000 10
   2  B 6000 20
   4  D 4000 10
   5  E 5000 20

 GROUP BY deptno :- 

  10
    1  A 5000  
    4  D 4000 
 
  20
     2  B  6000
     5  E  5000

 SELECT deptno,sum(sal) :- 

   10   9000
   20   11000

  display dept wise total sal where deptno=10,20 and
  sum(sal) > 10000 ? 

  SELECT  deptno,sum(sal)
  FROM emp
  WHERE deptno IN (10,20) and sum(sal) > 10000
  GROUP BY deptno 
  ORDER BY deptno asc ;  => ERROR

  => oracle cannot calculate sum(sal) of dept before group by
     it calculates only after group by.so apply the cond
     sum(sal) > 10000 after group by using HAVING clause.

  SELECT  deptno,sum(sal)
  FROM emp
  WHERE deptno IN (10,20) 
  GROUP BY deptno 
  HAVING sum(sal) > 10000
  ORDER BY deptno asc ;

 => display no of employees for each job where job=clerk,manager
  and no of employees > 3 ? 

  SELECT job,count(*)
  FROM emp
  WHERE job in ('CLERK','MANAGER')
  GROUP BY job 
  HAVING count(*) > 3   ;
  
 WHERE VS HAVING :- 

      WHERE                   HAVING

1  selects specific rows      selects specific groups

2  conditions applied         conditions applied after group by
   before group by

3  use where clause if        use having clause if cond
   cond doesn't contain       contains group function
   group function

 
  subqueries / nested queries :- 

  =>  a query in another query is called subquery or nested query
  => one query is called inner/child/sub query
  => other query is called outer/parent/main query
  => first oracle executes inner query and it executes outer query
     and result of inner query is input to outer query
  => use subquery when where condition is based on unknown value
  
   SELECT columns
   FROM tabname
   WHERE col OP (SELECT statement) 

   employees earning more than blake ?

   SELECT * FROM emp
      WHERE sal > (SELECT sal FROM emp WHERE ename='BLAKE');
  
   employees who are senior to KING ? 

   SELECT * FROM EMP
    WHERE HIREDATE < (SELECT HIREDATE FROM EMP
                         WHERE ENAME='KING') ;

 employee name earning max salary ?

 SELECT ename
 FROM emp
 WHERE sal = MAX(SAL) ;  => error

 => group functions are not allowed in where clause. they are
 allowed in SELECT,HAVING clauses.

   SELECT ename
   FROM emp
   WHERE sal = (SELECT max(sal) FROM emp) ;

 => display name of the employee having max experience ?

    SELECT ename 
    FROM emp
    WHERE hiredate = (SELECT min(hiredate) FROM emp)

 => employee names earning min,max salaries ?

    method 1 :- 

    SELECT ename,sal 
    FROM emp
    WHERE sal = (SELECT min(sal) FROM emp) 
          OR
          sal = (SELECT max(sal) FROM emp) ;

   method 2 :- 
 
    SELECT ename,sal 
    FROM emp
    WHERE sal = (SELECT min(sal) FROM emp) 
    UNION
    SELECT ename,sal 
    FROM emp
    WHERE sal = (SELECT max(sal) FROM emp) 


 => outer query can be SELECT/INSERT/UPDATE/DELETE but
    inner query must be always SELECT.

 subqueries in update command :- 

   UPDATE tabname
   SET colname = value,---
   [WHERE cond]

 => update employee sal to max(sal) of 30th dept whose
    empno=7499 ? 

   UPDATE emp
   SET sal = (SELECT max(sal) FROM emp WHERE deptno=30) 
   WHERE empno=7499 ;

 => swap employee salaries whose empno=7369,7499 ? 

    UPDATE EMP
    SET SAL = CASE EMPNO
              WHEN 7369 THEN (SELECT SAL FROM EMP 
                                    WHERE EMPNO=7499)
              WHEN 7499 THEN (SELECT SAL FROM EMP
                                    WHERE EMPNO=7369)
              END
  WHERE EMPNO IN (7369,7499) ; 
              
 INLINE views :- 

 => subqueries in FROM clause are called inline views.

     SELECT * FROM (subquery) <alias>

 => subquery output acts like a table for outer query

 => by default oracle executes the clauses in the following
  order

 FROM
 WHERE
 GROUP BY
 HAVING
 SELECT
 ORDER BY 

=> use INLINE views to control this order of execution.

 Example 1 :- 

   display employee names and annusal salaries earning more
   than 30000 annual sal ?

   SELECT ename,sal*12 as annsal
   FROM emp 
   WHERE annsal > 30000 ;  => ERROR

  => column aliases cannot be used in WHERE clause because
  WHERE clause is executed before SELECT. use INLINE views
  To overcome this problem.

   SELECT *
   FROM (SELECT ename,sal*12 as annsal 
         FROM emp) E
   WHERE annsal > 30000;

  Example 2 :- 

   DENSE_RANK() :- function used to calculate ranks 

           DENSE_RANK() OVER (EXPR)

  => EXPR includes 

  1 column name
  2 sort order

 => display ranks of the employees based on their salary ?
    highest paid employee should get 1st rank ?

    SELECT ename,sal,
      dense_rank() over (order by sal desc) as rnk
    FROM emp 

  => above query displays ranks of all the employees

      ENAME   SAL    RNK
      KING    5000    1
      FORD    3000    2
      SCOTT   3000    2
      JONES   2975    3

      JAMES   950     12

 => display top 5 employees ? 

     SELECT ename,sal,
      dense_rank() over (order by sal desc) as rnk
     FROM emp 
     WHERE rnk <= 5 ;  => ERROR

     
     SELECT *
     FROM (SELECT ename,sal,
                 dense_rank() over (order by sal desc) as rnk
           FROM emp )
     WHERE rnk <= 5 ; 

 =>  to display top 5 max salaries ?

     SELECT DISTINCT sal
     FROM (SELECT ename,sal,
                 dense_rank() over (order by sal desc) as rnk
           FROM emp) E
     WHERE rnk <= 5 ; 

 => to display 5th max sal ?

     SELECT DISTINCT sal
     FROM (SELECT ename,sal,
                 dense_rank() over (order by sal desc) as rnk
           FROM emp )
     WHERE rnk = 5 ; 

   Example 3 :- 

   ROWNUM :- 

   => returns record numbers for the records return by select 
         stmt
   => ROWNUM is called psuedo column
   => ROWNUM is not a column but acts like a column

     
     SELECT rownum,empno,ename,sal FROM emp 

        9   king
 
    SELECT rownum,empno,ename,sal FROM emp WHERE sal>=2000

        5   king

    SELECT rownum,empno,ename,sal FROM emp WHERE sal>=3000

        3   king

   => if query changes rownum also changes because rownum is
     not based on table, it is based on query output

   => rownum is useful when fetching records from table is 
  based on record numbers.

   display first 5 rows from emp table

   SELECT rownum as rno,empno,ename,sal 
   FROM emp 
   WHERE rownum <= 5 ;

   dislay 5th row ?

   SELECT rownum as rno,empno,ename,sal 
   FROM emp 
   WHERE rownum = 5 ;

   => in where condition with rownum =  >  >= operators will not
    work only  <  <= operators works. To overcome this problem
    use INLINE views.

    SELECT *
    FROM (SELECT rownum as rno,empno,ename,sal
          FROM emp) E
    WHERE rno=5 
    WHERE rno IN (5,7,11)  
    WHERE rno BETWEEN 5 AND 10
    WHERE MOD(rno,2)=0

 
  writing queries :- 

  using basic clauses like where,order by
  using group by 
  using joins
  using set operators
  using subqueries

 Database Transactions :- (TCL commands)

 => a Transaction is a unit of work that contains one or more
   dmls and must be saved as a whole or must be cancelled as 
   a whole.

   withdrawl :- 

   update  

   depsoit :- 

   update

   money transfer :- 

   acct1------------------->acct2

   update(-)                update(+)  

   successful               failed       not a valid txn
   failed                   successful   not a valid txn

   successful               successful    valid
   failed                   failed        valid

 => if txn contains multiple dmls then if all dmls are successful
  then it must be saved. if one of the operations fails then
  entire txn must be cancelled

 => every txn should gurantee a property called atomocity
    i.e. all or none.

 => the following commands provided by oracle to control the
 transactions called TCL commands.
 
  1 commit  => to save txn
  2 rollback => to cancel txn
  3 savepoint => to cancel part of the txn

 => every txn has a begin point and an end point

 => a txn begins whenever user submits dml command to oracle
 
 => a txn ends when user submits any of the following commands

    1 commit/rollback
    2 DDL/DCL commands the txn ends with commit

 
 UPDATE1 => txn begins T1
 INSERT1 
 UPDATE2
 INSERT2
 COMMIT   => txn ends 

 => if txn ends with COMMIT then it is called successful txn
  and operations are saved.

 UPDATE1 => txn begins T1
 INSERT1
 UPDATE2
 INSERT2
 ROLLBACK  => txn ends 

 => if txn ends with ROLLBACK then it is called aborted txn 
    and operations are cancelled.

 scenario :- 

1

 create table a(a int);
 insert into a values(10);
 insert into a values(20);
 insert into a values(30);
 insert into a values(40);
 rollback ;

 which operations are saved and which are cancelled ?

 ans :- 

   create table is saved and inserts are cancelled

    DDL command =  DDL command + commit

2 

  create table a(a number);
  insert into a values(10);
  insert into a values(20);
  create table b(b number);
  insert into a values(30);
  insert into a values(40);
  rollback ;

  which are saved and which are cancelled ?

  ans :-  insert 10,20 are saved
          insert 30,40 are cancelled

 savepoint :- 

 => we can declare savepoint and we can rollback upto the savepoint
 => using savepoint we can cancel part of the txn   
 
  create table a(a number);
  insert into a values(10);
  insert into a values(20);
  savepoint sp1;
  insert into a values(30);
  insert into a values(40);
  savepoint sp2;
  insert into a values(50);
  insert into a values(60);
  rollback to sp1; 

 
  select * from a ;

  10
  20

 Database security :-  (DCL commands)

 => the following facilities provides security in oracle

   1 users & pwd => provides security at db level
   2 privileges  => provides security at table level
   3 views       => 

   DATABASE (users & pwd)
       TABLES (privileges)
           ROWS & COLS (views)

  creating user in oracle :- 

  system/manager :- 

  SQL>create user scott identified by tiger
      default tablespace users
      quota unlimited on users ;

  SQL>grant connect,resource to scott ;

  privileges :- 

  => privileges means permissions on tables 
  => permissions are granted to user by using grant command
  
  
   GRANT <privileges> ON <tabname> TO <usernames> 

  BATCH2PM :- 

  SQL>GRANT ALL ON EMP TO SCOTT; 

  SCOTT :- 

  SQL>SELECT * FROM BATCH2PM.EMP ;

  SQL>UPDATE BATCH2PM.EMP SET SAL=2000 WHERE EMPNO=7369;

  => changes made by SCOTT are visible to BATCH2PM after 
  executing COMMIT.

  SQL>COMMIT;

 Granting specific privileges :- 

 BATCH11AM :- 

 SQL>GRANT SELECT,INSERT,UPDATE ON DEPT TO SCOTT ;

 SCOTT :- 

 SQL>DELETE FROM BATCH2PM.DEPT WHERE DEPTNO=10;

 Granting privileges to multiple users :- 

 BATCH11AM :- 

  SQL>GRANT ALL ON EMP TO SCOTT,HR,SH ;
  SQL>GRANT ALL ON EMP TO PUBLIC;

 REVOKE command :- 

 => command used to take back permissions from user

  REVOKE <privileges> ON <tabname> FROM <username> 

 BATCH11AM :- 

 SQL> REVOKE ALL ON EMP FROM SCOTT ; 
 
 
 VIEWS :- 

 => a view is a virtual table that doesn't store data and doesn't
 occupy memory. It always derives data from base table.

 => views are created 

 1 to provide security
 2 to reduce complexity

 => view provides another level of security by granting specific
  rows and columns to users.

 => views are 2 types 

  1 simple views
  2 complex views 

 simple views :- 

 => if view created on single table then it is called simple view

  CREATE VIEW <NAME>
  AS
  SELECT STATEMENT ;

  Granting permission to create view :- (system/manager)

  SQL> GRANT CREATE VIEW TO BATCH2PM;

 
 Example :- (batch2pm/NARESH)

 SQL>CREATE VIEW V1
     AS
     SELECT EMPNO,ENAME,JOB,DEPTNO FROM EMP ;

 =>  when above command executed oracle creates view "V1" and
  stores query but not query output (data).

  SQL>SELECT * FROM V1 ;

 => when we execute query on "V1" , the query associated with 
   "V1" is executed.

   SQL>SELECT * FROM (SELECT empno,ename,job,deptno FROM emp);

  Granting permissions on view to user :-

 BATCH2PM :- 

  SQL>GRANT ALL ON V1 TO SCOTT ; 

 => after granting permissions  scott can perform operations on
   emp table through view.

 SCOTT :- 

  SQL>INSERT INTO BATCH2PM.V1 VALUES(777,'PQR','clerk',20);

  => above command inserts record into emp table and remaining
   fields filled with nulls.

  => changes made by SCOTT visible to batch2pm after executing
     commit.

  SQL>UPDATE BATCH2PM.V1 SET JOB='MANAGER' WHERE EMPNO=777;

  SQL>UPDATE BATCH2PM.V1 SET SAL=4000 WHERE EMPNO=777;  => ERROR

  complex view :- 

  => a view said to be complex view 

  1 if it based on multiple tables
  2 if query performs group by,distinct,aggregate operations

 Example :- 

 1

  SQL>CREATE VIEW CV1
      AS
      SELECT E.EMPNO,E.ENAME,E.SAL,
             D.DEPTNO,D.DNAME,D.LOC 
      FROM EMP E INNER JOIN DEPT D
        ON E.DEPTNO = D.DEPTNO ;

  => after creating view whenever we want data from EMP & DEPT
 tables instead of executing join query execute the simple
 query as follows

   SQL>SELECT * FROM CV1 ;

 2 

   SQL>CREATE VIEW CV2
       AS
       SELECT DEPTNO,MIN(SAL) AS MINSAL,
                     MAX(SAL) AS MAXSAL,
                     SUM(SAL) AS SUMSAL,
                     COUNT(*) AS CNT
      FROM EMP
      GROUP BY DEPTNO ;

  => after creating view whenever we dept wise summary then
     execute the following query

    SQL>SELECT * FROM CV2; 

  Diff b/w  simple and complex views ?

         simple                complex 

 1    based on sigle table     based on multiple tables 

 2    query performs simple    query performs complex operations
      operations like where    like joins,group by etc.
 
 3    always updatable         not always updatable
      (allows dml)              

 synonyms :- 

 => a synonym means another name or alternative name for a table
 or view.

 => synonyms are created 

  1 if tablename is lengthy
  2 to access tables without owner name

 granting permission to create synonym :- 
 
  system/manager :- 

  SQL>GRANT CREATE SYNONYM TO BATCH2PM ;

 creating synonym :-

  syntax :-  CREATE SYNONYM <NAME> FOR <TABNAME> 

    SQL>CREATE SYNONYM E FOR EMP ;

 =>  after creating instead of using tablename use synonym name
     in SELECT/INSERT/UPDATE/DELETE  queries.

    SQL>SELECT * FROM E ;
   
    SQL>UPDATE E SET SAL=2000 WHERE EMPNO=7369;

 accessing tables without owner name :- 

 BATCH2PM :- 

 SQL>GRANT ALL ON EMP TO SCOTT;

 SCOTT :- 

 SQL>SELECT * FROM BATCH2PM.EMP ;

 SQL>CREATE SYNONYM E FOR BATCH2PM.EMP; 
 
 SQL>SELECT * FROM E;

 Question :- 

 sql>create synonym  e for emp; 
 sql>select * from emp e ;
 sql>rename emp to e ; => changes original tablename emp to e 

    diff b/w synonym & alias  ?

      synonym                     alias 

  1  permanent                    not permanent

  2 stored in db                  not stored in db 

  3 scope of the synonym         scope of the alias is upto the
    is upto the schema            query

 SEQUENCE :- 

 => sequences are created to generate sequence numbers.
 => sequences are used to auto increment column values.

  CREATE SEQUENCE <NAME> 
  [START WITH <VALUE>]
  [INCREMENT BY <VALUE>]
  [MAXVALUE <VALUE>]
  [MINVALUE <VALUE>]
  [CYCLE/NOCYCLE]
  [CACHE <size>]


 Example :- 

  SQL>CREATE SEQUENCE S1
      START WITH 1
      INCREMENT BY 1
      MAXVALUE  5 ;

 => every sequence has two columns 

  1 currval  => returns current value
  2 nextval  => returns next value

  seqname.currval
  seqname.nextval => generates nextvalue and returns that value

  using sequence :-

  SQL>CREATE TABLE STUDENT
       (
         SNO NUMBER(2),
         SNAME VARCHAR2(10)
       );

  SQL>INSERT INTO STUDENT VALUES(S1.NEXTVAL,'&SNAME');
      enter value for sname :- A

  SQL>/  (repeat  the above insert command 5 times)

  SQL>SELECT * FROM STUDENT;

     SNO  SNAME
      1    A
      2    B
      3    C
      4    D
      5    E

 generate sequence nos for existing rows :- 

 SQL>CREATE SEQUENCE S2
     START WITH 100
     INCREMENT BY 1
     MAXVALUE 1000;

  => generate sequence nos for empno column using s2 ?
  
   SQL>UPDATE EMP SET EMPNO = S2.NEXTVAL ; 

  CYCLE/NOCYCLE :- 

 => default is NOCYCLE.

 => if sequence created with NOCYCLE then it starts from 
 START WITH and generates upto MAXVALUE , after reaching
 MAXVALUE then it stops.

  start with-----------------------maxvalue

=> if sequence created with CYCLE then it starts from
   START WITH and generates upto MAXVALUE. after reaching
   MAXVALUE  then it is reset to MINVALUE.

     SQL>CREATE SEQUENCE S3
         START WITH 1
         INCREMENT BY 1
         MAXVALUE 5
         MINVALUE 1
         CYCLE
         CACHE 4; 

  SQL>INSERT INTO STUDENT VALUES(S3.NEXTVAL,'&SNAME');

  SQL>/ (repeate above insert command for 10 times)

  SQL>SELECT * FROM STUDENT ;

        SNO  SNAME
        1    A 
        2    B
        3    C
        4    D
        5    E
        1    F
        2    G
 
INDEX :- 

=>  index is also a db object created to improve the performance
    of data accessing. Index makes data accessing faster.

=> index in db is similar to index in textbook. In textbook
  using index a particular topic can be located fastly.
  In db using index a particular record can be located fastly.

=> indexes are created on columns and that column is called
   index key.

 Types of Indexes : -

1 BTREE indexes
   1 simple index 
   2 composite index
   3 unique index
2 BITMAP indexes 

1 simple btree index :- 

 => if we create index on single column then it is called
  simple index.

    CREATE INDEX <NAME> ON <TABNAME>(COLNAME) ;

    SQL>CREATE INDEX I1 ON EMP(SAL);

  => when we submit query to oracle then it uses following
  methods to locate records 

  1 table scan
  2 index scan

 => in "table scan" oracle scans entire table i.e. scans all the
    records of the table to locate required record

 => in "index scan" on avg oracle scans only half of the table
    to locate required record.so index scan is much faster 
    than table scan.

=> to see the execution plan execute the following command 

  SQL>SET AUTOTRACE ON EXPLAIN ;

 1 select * from emp where sal=3000; (index scan)
 2 select * from emp where sal>=3000; (index scan)
 3 select * from emp where sal<=3000; (index scan)
 4 select * from emp where sal<>3000; (table scan)

 2 composite index :- 

 => if index created on multiple columns then it is called
  composite index.

  SQL>CREATE INDEX I2 ON EMP(DEPTNO,JOB);

 => oracle uses above index when where condition based on 
  leading column of the index i.e. deptno.

  select * from emp where deptno=20; (index scan)
  select * from emp where deptno=20 and job='clerk'; (index)
  select * from emp where job='clerk'; (table scan)

3 unique index :- 

 => unique index doesn't allow duplicate values into the
 column on which index is created.

  SQL>CREATE UNIQUE INDEX I3 ON EMP(ENAME);
  
                            K

                   G               Q

       ADAMS *        JONES *           SCOTT *
       ALLEN *                          SMITH * 
       BLAKE *


 SQL>INSERT INTO EMP(EMPNO,ENAME,JOB,SAL)
             VALUES(4444,'BLAKE','CLERK',4000); => ERROR


 => PRIMARY KEY columns automatically indexed by oracle.
    Oracle creates a unique index on primary key column
    and unique index doesn't allow duplicates so pk also
    doesn't allow duplicates.

 BITMAP indexes :- 

 => bitmap indexes are created on low cardinality columns
    i.e. column that contains less distinct values is 
    called low cardinality column.

   EX :- gender,job,deptno

 => bitmap index stores bits (1,0)

  SQL>CREATE BITMAP INDEX BI1 ON EMP(JOB);
 



   



 






    

















 








 SQL

 creating tables
 writing queries
      using where
      using order by 
      using group by
      using joins
      using set operators
      using subqueries
 database transactions
 database security
 views
 synonyms
 sequences
 indexes  

			 PL/SQL

              PL  => procedural language 

                        oracle

                 sql            pl/sql
                (non proc)      (proc)
                commands         blocks


  pl/sql features :- 

  1 improves performance :- 

  => in pl/sql , sql commands can be grouped into one program
     and we can submit that program to oracle.so in pl/sql
     no of request & response between user and oracle are
     reduced and performance is improved

  2 supports conditional statements :- 

   => pl/sql supports conditional statements like if-then-else

  3  supports loops :-  

   => pl/sql supports loops like while,for etc.

 4   supports error handling :- 

  => in pl/sql if any statement causes error then we can handle
   that error and we can replace system generated messages
   with our own message.

 5  supports reusability :- 

  => pl/sql programs  can be centralized i.e. stored in database.
     so applications which are connected to db can reuse that
     pl/sql program.

 6  supports security :-  

 => because pl/sql programs are stored in database.so only
 authorized people can execute these programs.

 7  suports portability :- 

 => pl/sql programs can moved from one os to another os and
  without making changes we can execute that programs.

=> pl/sql programs are called pl/sql blocks and pl/sql blocks
 are 2 types 

  1 anonymous blocks
  2 named blocks 
        procedures
        functions
        packages
        triggers

anonymous blocks :- 

 => a block without name is called anonymous block

   DECLARE
     <variables>;    (declaration-part   optional)
   BEGIN
     statements;     (execution-part)
   END;
    /  

 how to print messages :-

 dbms_output.put_line(message);
 ----------- --------
  package    procedure

 => by default messages are not send to output . to send messages
  to output execute the following command

  SQL>SET SERVEROUTPUT ON 

 writing pl/sql program :- 

 1 Editors
 2 IDEs (integrated development environment)



                 Editors               IDEs

 coding          yes                    yes
 
 compile         no                     yes

 execute         no                     yes

 debug           no                     yes

  ex :-     notepad                     sql developer
                                        pl/sql developer
                                        toad

 => to write a prog open notepad and enter following code

  begin
    dbms_output.put_line('welcome');
  end;
  /

 => save the program in a file as d:\naresh\"prog1.sql"
 => go to sqlplus and compile & run the program as follows 

  SQL>@d:\naresh\prog1.sql
   welcome

 Datatypes in PL/SQL :- 

 => in pl/sql datatypes are categorized into 3 types 

  1 built-in types / scalar types 
  2 user define types
  3 reference types 

 built-in types :- 

 1 Number(p) / Number(p,s)
 2 char/varchar2/long/clob
 3 nchar/nvarchar2/nclob
 4 date/timestamp
 5 bfile/blob
 6 binary_float / binary_double
 7 binary_integer
 8 boolean

 1 TO 6  => allowed in sql,pl/sql
 7,8     => allowed only in pl/sql not allowed in sql

  Declaring variable :- 

       x   number(3);
       s   varchar2(10);
       d   date;
       
 Assigning value to variable :- 

      :=   => assignment operator

      x = 1000;  wrong
      x := 1000; right

 write a prog to add two numbers ?

 DECLARE
   a  number(3);
   b  number(3);
   c  number(4);
 BEGIN
   a := 100;
   b := 200;
   c := a+b;
   dbms_output.put_line(c);
 END;
  /
  
 how to input values at runtime :- 

 => to input values at runtime use variables prefixed with '&' .

  example 1 :-    a := &a;
            enter value for a := 100
                  a := 100;               
         
         2        a := &x;
             enter value for x :- 500
                  a := 500;

 DECLARE
   a  number(3);
   b  number(3);
   c  number(4);
 BEGIN
   a := &a;
   b := &b;
   c := a+b;
   dbms_output.put_line(c);
 END;
  /

 enter value for a :- 300
 enter value for b :- 200
 500

 write a prog to input date and print day of the week ?

 DECLARE
  d1 date;
 BEGIN
  d1 := '&date';
  dbms_output.put_line(TO_CHAR(d1,'day'));
 END;
  /
 
 DB programming with PL/SQL :- 

 => from pl/sql prog to perform operations over db execute
    sql commands from pl/sql program.

 => the following commands can be executed from pl/sql program.

  1 DML (insert,update,delete)
  2 DQL (select)
  3 TCL (commit,rollback,savepoint)

 select stmt syntax :- 

 SELECT columns INTO variables
 FROM  tabname
 WHERE condition ;

 SELECT ename,sal INTO x,y
 FROM emp
 WHERE empno = 105 ;

 write a prog to input empno and print name , salary and hiredate ?

 DECLARE
   veno   number(4);
   vename varchar2(10);
   vsal   number(7,2);
   vhire  date;
 BEGIN
   veno := &empno;
   SELECT ename,sal,hiredate INTO vename,vsal,vhire
   FROM emp
   WHERE empno=veno;
   dbms_output.put_line(vename||'  '||vsal||'  '||vhire);
 END;
  /
   
 write a prog to calculate experience of the employee ? 

 DECLARE
   veno  number(4);
   vhire date;
   vexpr number(2);
 BEGIN
   veno := &empno;
   select hiredate into vhire from emp where empno=veno;
   vexpr := (sysdate-vhire)/365;
   dbms_output.put_line('Experience = '||vexpr||' Years');
 END;
  /

 write a prog to input empno and calculate total sal ? 

   total sal = sal + comm 

 conditional statements :- 

 1 if-then-else :- 

   if cond then
     statements;
   else
     statements;
   end if;

 2 multi if :- 

   if cond1 then
     statements;
   elsif cond2 then
     statements;
   elsif cond3 then
     statements;
   else
     statements;
   end if;

 3 nested if :- 

  if cond then
     if cond then
       statements;
     else
       statements;
     end if;
  else
    statements;
  end if;

write a prog to input empno and increment sal by specific amount ?
after incr if sal exceeds 5000 then cancel that increment ?

 DECLARE
   veno   NUMBER(4);
   vamt   NUMBER(5);
   vsal   NUMBER(7,2);
 BEGIN
    veno := &empno;
    vamt := &amount;
    update emp set sal=sal+vamt where empno=veno;
    select sal into vsal from emp where empno=veno;
    if vsal>5000 then
       rollback;
    else
       commit;
    end if;
END;
 /

write a prog to input empno and incr sal based on their job ?

 if job=clerk incr sal by 10%
        salesman          15%
        manager           20%
        others            5%

 DECLARE
   veno  NUMBER(4);
   vjob  VARCHAR2(10);
   vpct  NUMBER(2);
 BEGIN
   veno := &empno;
   SELECT job INTO vjob FROM emp WHERE empno=veno;
   IF vjob='CLERK' THEN
       vpct := 10;
   ELSIF vjob='SALESMAN' THEN
       vpct := 15;
   ELSIF vjob='MANAGER' THEN
       vpct := 20;  
   ELSE
       vpct := 5;
   END IF;
   update emp set sal=sal+(sal*vpct/100) where empno=veno;
   commit;
 END;
 /

 write a prog to process bank transaction (w/d) ?

 ACCOUNTS
 ACCNO   BAL
 100	10000
 101	20000

 DECLARE
   vacno   number(4);
   vtype   char(1);
   vamt    number(5);
   vbal    number(7);
BEGIN
   vacno  := &accno;
   vtype  := '&type';
   vamt   := &amount;
   if vtype='w' then
      select bal into vbal from accounts where accno=vacno;
      if vamt > vbal then
          dbms_output.put_line('insufficient balance');
      else
          update accounts set bal=bal-vamt where accno=vacno;
      end if;
   elsif vtype='d' then
      update accounts set bal=bal+vamt where accno=vacno;
   else
      dbms_output.put_line('invalid transaction');
   end if;
   commit;
 END;
 /

 write a prog to process money transfer ? 

   DECLARE
     vsacno  NUMBER(4);
     vtacno  NUMBER(4);
     vamt    NUMBER(5);
     vbal    NUMBER(7);
  BEGIN
     vsacno := &sacno;
     vtacno := &tacno;
     vamt   := &amount;
    select bal into vbal from accounts where accno=vsacno;
    if vamt > vbal then
       dbms_output.put_line('insufficient balance');
    else
      update accounts set bal=bal-vamt where accno=vsacno;
      update accounts set bal=bal+vamt where accno=vtacno;
      commit;
    end if;
  END;
 /

 Reference types :- 

 1 %type
 2 %rowtype

 1 %type :- 

 => used to refer column datatype & size.

  ex :-  vsal   emp.sal%type;

 => whatever datatype & size declared for sal column then same
  type & size assigned to variable vsal.

        vename  emp.ename%type;
 
 2 %rowtype :- 

 => used to refer record type of a particular table.

      e   emp%rowtype;

 => a row from emp table can be assigned to variable "e" as 
    follows.
 
  SELECT * INTO e 
  FROM emp 
  WHERE empno = 107 ;

  e
  empno  ename  job        mgr  hiredate    sal  comm  deptno
  107    scott  analyst         09-DEC-82   4200      20

 => from the rowtype variable individual field values are accessed
   by using rowtypevar.fieldname.

      e.job => analyst
      e.sal => 4200

 => Adv of %rowtype is it reduces no of variables required in the
  program and reduces complexity.

 Example :- 

  write a prog to input empno and print employee details ? 

  DECLARE
    veno   emp.empno%type;
    r      emp%rowtype;
  BEGIN
    veno := &empno;
    SELECT * INTO r
    FROM emp	
    WHERE empno = veno;
    dbms_output.put_line('Name ='||r.ename);
    dbms_output.put_line('Sal ='||r.sal);
    dbms_output.put_line('Job ='||r.job);
  END;
   /

  write a prog to input sno and calculate total,avg,res 
  and insert into result table ?

  STUDENT
  SNO  SNAME  S1  S2  S3
  1    A      80  90  70
  2    B      30  60  50

  RESULT
  SNO  STOT  SAVG   SRES

  DECLARE
    vsno  student.sno%type;
    s     student%rowtype;
    r     result%rowtype;
  BEGIN
    vsno := &sno;
    SELECT * INTO s FROM student WHERE sno=vsno;
    r.stot := s.s1+s.s2+s.s3;
    r.savg := r.stot/3;
    if s.s1>=35 and s.s2>=35 and s.s3>=35 then
        r.sres := 'pass';
    else
        r.sres := 'fail';
    end if;
    INSERT INTO RESULT VALUES(vsno,r.stot,r.savg,r.sres);
    COMMIT;
 END;
  /
    
 Loops in pl/sql :- 

 => pl/sql supports 3 types of loops 

 1 simple loop
 2 while loop
 3 for loop 

simple loop :- 

loop
  statements;
  exit when cond;
end loop;

 if cond=false loop continues
 if cond=true loop terminates 

while loop :- 

 while(cond)
loop
   statements;
end loop;

 if cond=true loop continues
 if cond=false loop terminates

for loop :- 

  for <var> in <low>..<upp>
 loop
   statements;
 end loop;

 for x in 1..10            for(x=1;x<=10;x++)
loop
 statements;
end loop;

=> variable "x" declared implicitly as number type
=> by default x is incremented by 1
=> "x" is read only variable
=>  scope of the "x" is upto the for loop

 write a prog to print nos from 1 to 20 ?

using simple loop :-

 DECLARE
   x  number(2) := 1;
 BEGIN   
  LOOP
    dbms_output.put_line(x);
    x := x+1;
    exit when x>20;
 END LOOP;
 END;
  /

while loop :- 

 DECLARE
   x  number(2) := 1;
 BEGIN   
   while(x<=20)
 loop
    dbms_output.put_line(x);
    x := x+1;
 end loop;
 END;
  /

 for loop :- 

 BEGIN
  for x in 1..20
loop
  dbms_output.put_line(x);
 end loop;
END;
 /

 REVERSE for loop :- 
 
 BEGIN
  for x in REVERSE 1..20
loop
  dbms_output.put_line(x);
 end loop;
END;
 /

write a prog to print all even nos from 1 to 20 using while loop ?

declare
  x number(2) := 2;
begin
 while(x<=20)
 loop
    dbms_output.put_line(x);
    x := x+2;
 end loop;
end;
 /

write a prog to print 2020 calendar ? 

   date           day
   01-JAN-20      ?
   02-JAN-20      ?


   31-DEC-20       ?

  DECLARE
    d1 date;
    d2 date;
 BEGIN
    d1 := '01-JAN-20';
    d2 := '31-DEC-20';
    while(d1<=d2)
  loop
     dbms_output.put_line(d1||'    '||to_char(d1,'day'));
     d1 := d1+1;
  end loop;
 END;
  /

  write a prog to print sundays between two given dates ? 
    
 DECLARE
    d1 date;
    d2 date;
 BEGIN
    d1 := '&DATE1';
    d2 := '&DATE2';
    d1 := NEXT_DAY(d1,'sunday');
    while(d1<=d2)
  loop
     dbms_output.put_line(d1||'  '||to_char(d1,'day'));
     d1 := d1+7;
  end loop;
 END;
  /

1 write a prog to input number and print whether it is prime or 
  not ?

2  write a prog to input number and print sum of individual digits

   input :- 124
   output :- 1+2+4 = 7 

3  write a prog to print the following pattern ?

 *
 **
 ***
 ****
 *****

5  write a prog to input string and print as follows ?


  input :- NARESH
  output A:- 

  N
  NA 
  NAR
  NARE
  NARES
  NARESH

6  write a prog to input string and print reverse of that string ?

  input :- NARESH
  output :- HSERAN

7 write a prog to input string and print whether it is palindrome
  or not ?

  example :- madam

 CURSORS :- 

 => cursors are used to process multiple rows in pl/sql program.

 => from pl/sql prog if we submit select statement to oracle,
    it goes to db and fetch data and copies that data into
    temporary memory area called private sql area. using cursor
    we can give name to that memory and access one by one row
    from that memory to the pl/sql program and process the row.

 => follow below steps to use cursor in pl/sql program.

   1 declare cursor
   2 open cursor
   3 fetch records from cursor  
   4 close cursor

 Declaring cursor :- 
 
 cursor <name> is select statement ;

 ex :-  cursor c1 is select * from emp ;

Opening cursor :- 

     open <cursor-name>;
     open c1; 

 1 select stmt submitted to oracle.
 2 data returned by select stmt is copied to private sql area.
 3 cursor c1 points to that private sql area.

3 fetching records from cursor :- 

=> "FETCH" statement is used to fetch records from cursor

  syn :- FETCH <cursor-name> INTO <variables> ;

         FETCH c1 INTO x,y,z,--;

=> a fetch statement fetches one record at a time but to process
   multiple records fetch statement should be inside a loop.

4 closing cursor :- 

   close <cursor-name>;
   close c1; 

 cursor attributes :- 

 1 %found :- 

  TRUE    => if fetch successful
  FALSE   => if fetch unsuccessful

 2 %notfound :- 

  TRUE     => if fetch unsuccessful
  FALSE    => if fetch successful

 3 %rowcount :- 

  returns no of rows fetched successfully

 => all these attributes are used with cursor name for ex 

 c1%found
 c1%notfound
 c1%rowcount

 write a prog to print all employee names and salaries ?

 DECLARE
    cursor c1 is select ename,sal from emp ;  
    vename emp.ename%type;
    vsal   emp.sal%type;
 BEGIN
    open c1;
  loop
    fetch c1 into vename,vsal;
    exit when c1%notfound;
    dbms_output.put_line(vename||'   '||vsal);
  end loop;
    close c1; 
END;
 /
  
using while loop :- 

 DECLARE
    cursor c1 is select ename,sal from emp ;  
    vename emp.ename%type;
    vsal   emp.sal%type;
 BEGIN
    open c1;
    fetch c1 into vename,vsal;
    while(c1%found)
 loop
    dbms_output.put_line(vename||' '||vsal);
    fetch c1 into vename,vsal;
 end loop;
    close c1; 
END;
 /
          
using FOR LOOP CURSOR :- 

 => Adv of for loop cursor is opening cursor,fetching records
  from cursor,closing cursor is not required and all these
  operations performed implicitly.

  FOR <var> IN <CURSOR-NAME>
loop
   statements;
end loop;

 FOR r IN C1
loop
  statements;
end loop;

=> everytime for loop is executed  a record is fetched from
  cursor and assigned to variable "r". Loop variable "r"
  is also declared implicitly as rowtype.

 DECLARE
   cursor c1 is select ename,sal from emp;
 BEGIN
   for r in c1
 loop
    dbms_output.put_line(r.ename||' '||r.sal);
 end loop;
 END;
  /

 Write a prog to calculate total sal without using SUM function ?

 DECLARE
   cursor c1 is select sal from emp;
   t number := 0;
 BEGIN
   for r in c1
 loop
    t := t + r.sal;
 end loop;
 dbms_output.put_line('Total salary = '||t);
END;
 /

 Write a prog to display maximum salary ?

 write a prog to display minimum salary ? 

 write a prog to calculate all the students total,avg,res and
 insert into result table ?

 STUDENT
 SNO  SNAME  S1  S2  S3
 1    A      80  90  70
 2    B      60  50  30


 RESULT
 SNO STOT  SAVG  SRES 

 DECLARE
   cursor c1 is select * From student;
   r  result%rowtype;
 BEGIN
   for s in c1
 loop
    r.stot := s.s1+s.s2+s.s3;
    r.savg := r.stot/3;
    if s.s1>=35 and s.s2>=35 and s.s3>=35 then
       r.sres := 'pass';
    else
       r.sres := 'fail';
    end if;
    insert into result values(s.sno,r.stot,r.savg,r.sres);
 end loop;
     commit;
 END;
/ 

 write a prog to increment employee salaries based on the pct
 in raise_salary table ?

 RAISE_SALARY
 EMPNO   PCT
 7369   10
 7499   15
 7521   10
 7566   20
 7654   15

 DECLARE
   cursor c1 is select * from raise_salary;
 BEGIN
   for r in c1
 loop
     update emp set sal=sal+(sal*r.pct/100) 
                           where empno=r.empno;
 end loop;
    commit;
 END;
  /

 Error Handling / Exception Handling :- 

 1 syntax errors
 2 logical errors
 3 runtime errors (exception)

 => errors that are raised during program execution are called
    runtime errors or exceptions.

 => in pl/sql if any statement causes runtime error then 
    program execution is terminated and oracle displays
    error message. To replace system generated message with
    our own message then we need to handle that runtime error.

 => to handle runtime errors in pl/sql program include a block
    called exception block.

  DECLARE
    declaration-part;
  BEGIN
    statements; => statements causes exception
  EXCEPTION
    statements; => statements handles exception
  END;
  / 

 => exceptions are 2 types 

 1 system defined
 2 user defined 

 system defined :- 

1  zero_divide :- 

 => raised when we try to divide a number with 0
 
  a := &a; 10
  b := &b; 0
  c := a/b; => zero_divide

 2 value_error :- 

 => raised when variable datatype or size mismatches.

 1        x  number(4);
          x := &x; => 10000  => value_error

 2        x number(4);
          x := &x; => 'abc'  => value_error

 3 invalid_number :- 

 => raised when we perform invalid calculation.

      d   date;
      d := '01-JAN-20' + 10 ; =>  invalid_number

 4 no_data_found :- 

 => raised when data not found in the table

        veno := &empno; =>  9090
        select sal into vsal 
              from emp where empno=veno; => no_data_found

  5 dup_val_on_index :- 

  => raised when we try to insert duplicate value into primary key

      create table x(x number(2) primary key);
      insert into x values(10);
      insert into x values(10); => dup_val_on_index 

 Example :- 

1

  DECLARE
   a number(3);
   b number(3);
   c number(3);
 BEGIN
   a := &a;  
   b := &b; 
   c := a/b;
   dbms_output.put_line(c);
 EXCEPTION
    when zero_divide then
       dbms_output.put_line('divisor cannot be zero');
    when value_error then
       dbms_output.put_line('value exceeding size');
 END;
  /

 2

   write a prog to input empno and print name & salary ? 

  DECLARE
    veno  emp.empno%type;
    vename emp.ename%type;
    vsal   emp.sal%type;
  BEGIN
     veno := &empno;
     SELECT ename,sal INTO vename,vsal 
                        FROM emp WHERE empno=veno;
     dbms_output.put_line(vename||' '||vsal);
  EXCEPTION
    when no_data_found then
        dbms_output.put_line('employee not exists');
    when value_error then
        dbms_output.put_line('number exceeding size');
  END;
    /

 SQLCODE,SQLERRM  :- 

 SQLCODE  => returns error code
 SQLERRM  => returns error message

 => if any exception raised then code will passed to SQLCODE
  and message will be passed to SQLERRM.

Example :- 

  CREATE TABLE emp88
    (
     empno number(4) primary key ,
     ename varchar2(10) not null,
     sal   number(7,2) check(sal>=3000)
    );

  write a prog to insert data into emp88 table ?

  DECLARE
    veno   emp88.empno%type;
    vename  emp88.ename%type;
    vsal    emp88.sal%type;
 BEGIN 
    veno := &empno;
    vename := '&ename';
    vsal   := &sal;
    INSERT INTO emp88 VALUES(veno,vename,vsal);
    COMMIT; 
 EXCEPTION
    when dup_val_on_index then
        dbms_output.put_line('empno cannot be duplicated');
    when others then 
        if sqlcode = -2290 then
          dbms_output.put_line('sal>=3000');
        end if;
 END;
  /

 user defined exceptions :- 

 => exceptions declared by user are called user defined exceptions

 => when predefined exceptions are not meeting our requirements
    then we define our own exceptions called user defined
    exception.

 => user defined exceptions are raised by using 

 1 RAISE statement
 2 RAISE_APPLICATION_ERROR

 using RAISE statement :- 
 
     syn :-  RAISE <exception-name> ;
     ex  :-  RAISE abc;
 
 => exception "abc" must be declared in declaration section 
    as follows 
  
          abc  exception;
 
 Example :- 

 DECLARE
   a number(3);
   b number(3);
   c number(3);
   abc exception;
 BEGIN
   a := &a;  
   b := &b; 
   if b=1 then
     raise abc;
   end if;
   c := a/b;
   dbms_output.put_line(c);
 EXCEPTION
    when zero_divide then
       dbms_output.put_line('divisor cannot be zero');
    when value_error then
       dbms_output.put_line('value exceeding size');
    when abc then
       dbms_output.put_line('divisor cannot be one');
 END;
  /

 using raise_application_error :- 

  raise_application_error(error code,error msg);

  error code => -20001 to -20999
  error msg  => any text
 
  diff b/w raise & raise_application_error ? 

 => in raise statement exception is raised by using name

 => in raise_application_error exception is raised by using code

 => use raise statement to raise exception and to handle exception

 => use raise_application_error to raise exception and do not 
    want to handle.

   write a prog to increment specific employee sal by specific
   amount and sunday updates are not allowed ?

   DECLARE
     veno  emp.empno%type;
     vamt  number(4);
   BEGIN
     veno := &empno;
     vamt := &amount;
     IF TO_CHAR(sysdate,'dy')='sun' THEN
         RAISE_APPLICATION_ERROR(-20001,'sunday not allowed');
     END IF;     
     UPDATE emp SET sal=sal+vamt WHERE empno=veno;
     COMMIT;
   END;
    /

  Named PL/SQL blocks :- 

  1 procedures
  2 functions
  3 packages
  4 triggers 

  sub-programs :- 

  1 procedures
  2 functions 

  Advantages :- 

  1 modular programming :- 

  => with the help of procedures & functions a big program can
  be divided into small modules 

  2 reusability :- 

  => proc & func can be centralized i.e. stored in db.so 
     applications which are connected to db can reuse these
     proc & func.

 3 security :- 

  => because proc & func are stored in database , so they are
     secured only authorized users can execute these programs.

 4 invoked from front-end applications :- 
 
  => proc & func can be called from front-end applications like
    java,.net,php etc.

 5 improves performance :- 

 => proc & func improves performance because they are precompiled.
    i.e. compiled already and ready for execution. when we 
    create a procedure the program is compiled and stored in
    db and everytime we call the procedure only execution is
    repeated but compilation is not repeated.

  procedures :- 

 => a procedure is a named PL/SQL block that accepts some
    input and performs some action on database and may or
    may not returns a value.

 => procedures are created to perform one or more dml operations
    on database.

 => procedures are 2 types 

   1 standalone or stored procedures
   2 packaged procedures

 1 standalone or stored procedures :- 

 => these procedures are stored as seperate object in database.
 => these programs are created directly under schema.
 
   CREATE OR REPLACE
        PROCEDURE <name>(parameters if any) 
   IS
     <declaration-part>;
   BEGIN
      <execution-part>;
   END;
    /

  parameters :- 

 => we can declare parameters and we can pass values to parameters
 => parameters are 2 types 
  
       1  formal
       2  actual 

 => parameters declared while creating procedure are called formal.
 => parameters used while calling procedure are called actual.
 => formal parameters are again 3 types 

  1 IN
  2 OUT
  3 IN OUT

 IN :- 
 
  => always recieves value
  => default
  => read only

 OUT :- 

  => always sends value
  => write only 

 IN OUT :- 

 => recieves and sends value
 => read & write

 create a procedure to increment specific employee sal by  
 specific amount ?

 CREATE OR REPLACE PROCEDURE update_salary
 (
    p_eno in number,   
    p_amt in number
 )
 IS
 BEGIN
    UPDATE emp SET sal=sal+p_amt WHERE empno=p_eno;
    COMMIT;
 END;
   /

 procedure created (compiled + stored in db)

 Execution :- 

 1 from sql prompt
 2 from another pl/sql block
 3 front-end applications

 Executing from SQL prompt :- 

 SQL>EXECUTE update_salary(100,1000);

 Executing from another pl/sql block :- 

 1 positional notation
 2 named notation 

 1 positional notation :- 

 => in positional notation parameters are mapped through positions

   ex :-  procedure  :-   update_salary(p_eno  , p_amt)

          calling    :-   update_salary(100,1000);

2 Named notation :- 

 => in named notation parameters are mapped through names by 
    using => operator.

              formal => actual

   ex :- procedure :-  update_salary(p_eno,p_amt)

         calling  :- update_salary(p_eno=>100,p_amt=>1000)
                     update_salary(p_amt=>1000,p_eno=>100)

 =>  named notation is convenient than positional notation.
     because in named notation parameters can be passed in
     any order.

 Example :- 

 positional notation :- 

 DECLARE
   veno  emp.empno%type;
   vamt  number(4);
 BEGIN
   veno := &empno;
   vamt := &amount;
   update_salary(veno,vamt);
 END;
  /

 named notation :- 

DECLARE
   veno  emp.empno%type;
   vamt  number(4);
 BEGIN
   veno := &empno;
   vamt := &amount;
   update_salary(p_eno=>veno,p_amt=>vamt);
 END;
  /

out parameter example :- 

=> create procedure to increment specific employee sal by 
 specific amount ? after increment send the updated sal to
 calling program ?

 CREATE OR REPLACE PROCEDURE update_salary
 (
    p_eno in number,   
    p_amt in number,
    p_sal out number
 )
 IS
 BEGIN
    UPDATE emp SET sal=sal+p_amt WHERE empno=p_eno;
    COMMIT;
    SELECT sal INTO p_sal FROM emp WHERE empno=p_eno;
 END;
   /

 Execution :- 

 DECLARE
   veno  emp.empno%type;
   vamt  number(4);
   vsal  emp.sal%type;
 BEGIN
   veno := &empno;
   vamt := &amount;
   update_salary(veno,vamt,vsal);  /* 
                                    update_salary(p_eno=>veno,
                                                  p_amt=>vamt,
                                                   p_sal=>vsal)
                                   */
   dbms_output.put_line(vsal);
 END;
  /

Executing from sql prompt :- 

 SQL>VARIABLE K NUMBER ;

 SQL> EXECUTE update_salary(100,1000,:K);
 
 SQL>PRINT :K 

    7000

 Example 3 :- 

  create table emp88
    (
     empno number(4) primary key,
     ename varchar2(10) not null,
     sal  number(7,2) check(sal>=3000)
    );

 create a procedure to insert record into emp88 table ?
 if any exception raises then send error message to 
 calling program ?

 CREATE OR REPLACE PROCEDURE insert_emp88
 (
   p_eno  in number,
   p_name in varchar2,
   p_sal  in number,
   p_msg  out varchar2
 )
 IS
 BEGIN
   INSERT INTO emp88 VALUES(p_eno,p_name,p_sal);
   COMMIT;
   p_msg := 'record inserted successfully'; 
 EXCEPTION
   WHEN OTHERS THEN
     p_msg :=  SQLERRM;
 END;
  /
      
 user defined functions :- 

 => functions created by user are called user defined functions.

 => when predefined functions not meeting our requirements then
   we create our own functions called user defined functions.

 => a function is also a named PL/SQL block that accepts some
   input and performs some calculation and must return a value.

  CREATE OR REPLACE 
      FUNCTION <name>(parameters if any) RETURN <type>
 IS
   <declaration-part>;
 BEGIN
    <execution-part>;
    RETURN <expr>;
 END;
 /

Example :-

 CREATE OR REPLACE 
     FUNCTION CALC(a number,b number,op char) RETURN number
 IS
 BEGIN
    if op='+' then
       return(a+b);
    elsif op='-' then
       return(a-b);
    elsif op='*' then
       return(a*b);
    else
       return(a/b);
    end if;
 END;
 /

 function created (compiled + stored in db)

 Execution :- 

 1 sql commands
 2 another pl/sql block
 3 front-end application

 executing from sql command :-

 SQL>SELECT calc(10,20,'*') FROM DUAL ; => 200

 executing from another pl/sql block :- 

 DECLARE 
  x number(3);
  y number(3);
  z number(4);
 BEGIN
   x := &x;
   y := &y;
   z := calc(x,y,'*');  
   dbms_output.put_line(z);
 END;
  /

 create a function to check whether given year is leap year or
 not ? 

 create or replace 
   function is_leap(y number) return varchar2
 is
 d date;
 begin
    d := '29-FEB-'||y;
    RETURN 'leap year';
 exception
    when others then
       RETURN 'not a leap year'; 
 end;
 /

 execution :- 

 SQL>SELECT is_leap(2020) FROM DUAL ;
 
		
 SQL>SELECT ENAME,
           IS_LEAP(TO_CHAR(HIREDATE,'YYYY')) AS LEAP 
     FROM EMP ;

 
 create a function to check whether accounts exists or not ?

 ACCOUNTS
 ACCNO   BAL
 100     10000
 101     20000
   
 create or replace 
       function check_acct(a number) return boolean
 is
  cnt number;
 begin
   select count(*) into cnt from accounts where accno=a;
   if cnt=1 then
     return true;
   else
     return false;
   end if;
 end;
  /

 NOTE :- if function return type is boolean then it cannot be
 executed from sql commands and must be executed from another
 pl/sql block or front-end applications.

 create a function that accepts accno and returns balance ?

 create or replace 
    function getBalance(a number) return number
 is
  vbal number;
 begin
   select bal into vbal from accounts where accno=a;
   return vbal;
 end;
  /

 create a procedure for money withdrawl ? 

 create or replace 
     procedure debit(a number,amt number) 
 is
 begin
    /* check account exists or not */
     if check_acct(a)=false then
        raise_application_error(-20001,'account does not exists');
     end if;
    /* check balance is sufficient or not */
     if amt > getBalance(a) then 
         raise_application_error(-20002,'insufficient balance');
     end if;
     update accounts set bal=bal-amt where accno=a;
     commit;
 end;
  /

 create procedure for money deposit ?

 create a procedure for money transfer ? 

 Question :- 

   diff b/w procedures and functions ?

       procedures                  functions 

  1  may or may not returns       must return a value
     a value

  2  can return multiple values   returns only one value

  3  returns values using OUT     returns value using return
     parameter                     statement

  4  cannot be executed from      can be executed from sql 
     sql commands                   commands

  5  created to perform           created for select operation
       dml operations

  6 create procedure to           create function to get balance
    update balance

  USER_SOURCE :- table that stores procedures and functions
                 created by user

   NAME          TYPE         LINE         TEXT
   getBalance    function     1            create or replace
    "             "           2              function getBalance(a number) return number
                              3            is
                              4             vbal number;
                              5            begin

  display list of procedures and functions ?

  SQL>SELECT DISTINCT name,type  
      FROM user_source  
      ORDER BY type asc ; 
  
  display update_salary procedure code ? 

  SQL>SELECT text
      FROM user_source
      WHERE name='UPDATE_SALARY' ;

  packages :- 

  => a package is a collection of procedures,functions,variables,
     cursors etc
  => related procedures & functions are grouped into one package.
  
 Advantages :- 

 1 easy to manage :- because related procedures & functions
   are available in single package.so managing is easy.

 2 supports overloading :- 

 => standalone procedures/functions doesn't support overloading
    but packaged procedures/functions supports overloading.
    Inside the package we can define two or more procedures/
    functions with same name with different parameters.

 3 supports hiding :- 

 => in package we can make proc/func as public and private.
    public members can be called from anywhere but private
    members can be called within package.

4 improves performance :- 

 => when application requests for a proc/func in a package then
    oracle not only loads requested member but complete package
    loaded into memory. so next request will not go to db. so
    no of requests going to db are reduced and performance is
    improved.

 
 => a package contains two parts 

  1 package specification
  2 package body 

 package specification :- 

 => package specification contains declarations of procedures
  and functions.

  CREATE OR REPLACE PACKAGE <NAME>
  AS
  PROCEDURE DECLARATION ;
  FUNCTION DECLARATION;
  END;
  /
 
 package body :- 

 => package body contains definition of procedures & functions.

 CREATE OR REPLACE PACKAGE BODY <NAME>
 AS
 PROCEDURE DEFINITION ;
 FUNCTION DEFINITION;
 END;
  /

 create a package to implement various bank transactions ?

1  account opening (proc)
2  account closing (proc)
3  balance enquiry (function)
4  money deposit   (proc)
5  money withdrawl (proc)
6  money transfer  (proc)

 ACCOUNTS
 ACCNO  NAME  BAL
 100	      10000

 TRANSACTIONS
 TRID   TTYPE  TDATE   TAMT   ACCNO

 CREATE SEQUENCE S10
 START WITH 1
 INCREMENT BY 1
 MAXVALUE 99999

 package specification :- 

 create or replace package bank
 as
 procedure new_acct(a number,n varchar2,b number);
 procedure close_acct(a number);
 function getBalance(a number) return number;
 procedure credit(a number,amt number);
 procedure debit(a number,amt number);
 end;
  /

 package body :- 

 create or replace package body bank 
 as
 procedure new_acct(a number,n varchar2,b number)
 is
 begin
  insert into accounts values(a,n,b);
  commit;
 end new_acct;
 procedure close_acct(a number)
 is
 begin
   delete from accounts where accno=a;
   commit;
 end close_acct;
 function getBalance(a number) return number
 is
 vbal number;
 begin
   select bal into vbal from accounts where accno=a;
   return vbal;
 end getBalance;
 procedure credit(a number,amt number)
 is
 vtrid number;
 begin
   update accounts set bal=bal+amt where accno=a;   
   vtrid := s10.nextval;
   insert into transactions values(vtrid,'D',sysdate,amt,a);
   commit;
 end credit;
 procedure debit(a number,amt number)
 is
 vtrid number;
 vbal  number;
 begin
   vbal := getBalance(a);
   if amt > vbal then
       raise_application_error(-20001,'insufficient balance');
   end if;
   update accounts set bal=bal-amt where accno=a;   
   vtrid := s10.nextval;
   insert into transactions values(vtrid,'W',sysdate,amt,a);
   commit;
 end debit;
end;
 /
 
 Execution :- 

 => the whole package cannot be executed only the members of the
 package can be executed.

=> members of the package are invoked as follows

     PACKAGENAME.MEMBER(parameters)

  1  calling new_acct proc :-

  SQL>EXECUTE BANK.NEW_ACCT(100,'A',4000);

 2  calling credit proc :-
  
   SQL>EXECUTE BANK.CREDIT(100,5000);

 3  calling debit proc :-

    SQL>EXECUTE BANK.DEBIT(100,3000);

 Example 2 :- 

 create package to implement following operations 

 1 hire employee (proc)
 2 fire employee (proc)
 3 update salary (proc)
 4 update job    (proc)
 5 calculate experience (function)
 6 to get top N employees (function)

 droping package :- 

 SQL>DROP PACKAGE BANK ; => drops both specification & body
 SQL>DROP PACKAGE BODY BANK ; => drops only body 

 TRIGGERS :- 

  => trigger is also a named PL/SQL block like procedure but
    executed implicitly by oracle whenever user submits DML/DDL
    commands.

 =>  triggers are created  

  1 to control dmls.
  2 to enforce complex rules and validations.
  3 for auditing dml/ddl operations
  4 to maintain replicas
  5 to generate values for primary key columns 
  
  CREATE OR REPLACE TRIGGER <NAME>
  BEFORE / AFTER INSERT OR UPDATE OR DELETE
  ON <TABNAME>
  [FOR EACH ROW]
  [
    DECLARE
     variables;
  ]
  BEGIN    
     STATEMENTS;
  END;
  /

 Before triggers :- 

 => if trigger is before , then first oracle executes trigger then
    oracle executes DML.

   1 TRIGGER
   2 DML

 after triggers :- 

 => if trigger is after then first oracle executes DML then oracle
  executes trigger.

  1 DML
  2 TRIGGER

 Trigger Level :- 

 1  statement level (default)
 2  row level 

 statement level :- 

 => statement level triggers are executed once per the statement

 row level :- 

 => row level triggers are executed once per the row affected by 
    dml.

 create trigger to not to allow dml operations on emp table on 
 sunday ?

 create or replace trigger t1
 before insert or update or delete
 on emp
 begin
    if to_char(sysdate,'dy')='sun' then
        raise_application_error(-20001,'sunday not allowed');
    end if;
 end;
 /

create trigger to not to allow dmls as follows ?

    mon - fri  <10am and >4pm
    sat        <10am and >2pm
    sun        --------------

  create or replace trigger t2
  before insert or update or delete
  on emp
  begin
      if to_char(sysdate,'d')  between 2 and 6
         and
         to_char(sysdate,'hh24') not between 10 and 16  then
             raise_application_error(-20001,'only between 10am and 4pm');
      elsif to_char(sysdate,'dy')='sat'
            and
            to_char(sysdate,'hh24') not between 10 and 14 then
               raise_application_error(-20001,'only between 10am and 2pm');
      elsif  to_char(sysdate,'dy')='sun' then
                raise_application_error(-20001,'sunday not allowed');
      end if;
  end;
 /
 
 :NEW,:OLD variables :- 

 => these two variables are called bind variables.

 => using these two variables we can access data affected by dml
    inside the trigger. 

=> record user is trying to insert is copied to :NEW variable

 INSERT INTO EMP(EMPNO,ENAME,JOB,SAL) 
                 VALUES(121,'abc','clerk',4000)    => :NEW
  :NEW
  EMPNO  ENAME  JOB    SAL
  121    abc    clerk  4000

=> record user is trying to delete is copied to :OLD variable.

  DELETE FROM emp WHERE empno=101  => :OLD

  :OLD
  EMPNO  ENAME   JOB  		SAL
  101    ALLEN  SALESMAN	1600

 => record user is trying to update is copied to :NEW,:OLD
   variables.

   EMPNO   SAL
   100     2000

   UPDATE EMP SET SAL=3000 WHERE EMPNO=100 => :OLD, :NEW variables

   :OLD
   EMPNO   SAL
   100     2000

   :NEW
   EMPNO   SAL
   100     3000

  => these two variables are allowed only in row level triggers
     but not allowed in statement level triggers.

  create trigger to not to allow to decrement employee salary ?

  CREATE OR REPLACE TRIGGER T3
  BEFORE UPDATE 
  ON EMP
  FOR EACH ROW
  BEGIN
  IF :NEW.SAL < :OLD.SAL THEN
        RAISE_APPLICATION_ERROR(-20001,'sal cannot be decremented');
  END IF;
 END;
  /     
 
 create trigger to insert details into emp_resign when
 employee resigns from organization ?
 
  EMP_RESIGN
  EMPNO  ENAME   HIREDATE  DOR

  CREATE TABLE EMP_RESIGN
  (
    EMPNO  NUMBER(4),
    ENAME  VARCHAR2(10),
    HIREDATE DATE,
    DOR   DATE);

 CREATE OR REPLACE TRIGGER T4
 AFTER DELETE
 ON EMP
 FOR EACH ROW
 BEGIN
   INSERT INTO EMP_RESIGN VALUES(:OLD.EMPNO,:OLD.ENAME,
                                 :OLD.HIREDATE,SYSDATE);
 END;
 /

 USER_TRIGGERS :- 

 => system table or data dictionary table that stores information
    about triggers created by user.

	SELECT TRIGGER_NAME,TRIGGER_TYPE,TRIGGERING_EVENT
	FROM USER_TRIGGERS
	WHERE TABLE_NAME='EMP' ;

 Droping trigger :- 

  SQL>DROP TRIGGER T1;

 => if table is dropped then triggers created on table are also
   dropped.

 DATABASE
      BATCH2PM 
          TABLES
              ROWS & COLS
              CONSTRAINTS
              INDEXES
              TRIGGERS
          VIEWS
          SYNONYMS
          SEQUENCES
          PROCEDURES
          FUNCTIONS
          PACKAGES
    

 NVL() :- function used to convert null values.

       NVL(arg1,arg2)

       if arg1 = null returns arg2
       if arg1 <> null returns arg1 only

    NVL(100,200)      => 100
    NVL(NULL,200)     => 200

    display ENAME,SAL,COMM,TOTSAL ?

      TOTSAL = SAL + COMM 

    SELECT ENAME,SAL,COMM,SAL+NVL(COMM,0) AS TOTSAL FROM EMP 
