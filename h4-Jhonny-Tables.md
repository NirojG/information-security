
# h3 Jhonny Tables 
## x) Summary of OWASP 10: 2021
- OWASP stands for Open Worldwide Application Security Project. It is an open community, it is free and open to anyone interested in improving application security.
- The OWASP Top 10 is a standard awareness document for developers and web application security.  It represents the most critical security risks to web applications.
- Globally recognized by developers as the first step towards more secure coding.
- It has top 10 lists of most critical web security risks starting from the most serious ones leading to the 10th place of the most critical web security risks. 

### A01: 2021 - Broken Access Control 
- This is the no 1. serious web application security risks in the OWASP 10:2021. 
- Accessing the data or functions beyond their permissions.
- It includes bypassing the access checks by tampering the URLs, internatl states or API requests.
- Acting as administrators and or access other user's account by manipulating metadata such as JWT.

### A05: 2021 - Security Misconfiguration

- systems or cloud services set up incorrectly or improperly which creates vulnerability in the system.
- Unnecessary features are installed or enable that might compromise the system security like unnecessary ports, accounts, privileges etc.
- While upgrading system, the latest security features maybe disabled or not configured securely.
- The software of the systems or services is out of date or missing an update making it vulnerable.
- Default accounts of the system and their passwords are still the same and unchanged meaning they haven't been modified or made secure passwords.

### A06:2021 – Vulnerable and Outdated Components
- This risk involves using software libraries or frameworks that have known security holes.
- It covers everything from the operating system and database to nested dependencies.
- You are at risk if you don't have a full inventory of the component versions you use.
- Prevention requires a patch management process to remove unused code and update libraries regularly.

### A03:2021 - Injection 
- This risk occurs when hostile data is sent to an interpreter as part of a command or query.
- It commonly includes SQL, NoSQL, OS command, and LDAP injections.
- Applications are vulnerable when the user-supplied data is not validated, filtered, or sanitized.
- The best prevention method for injection is using secure, parameterized APIs or Object Relational Mapping (ORM) tools.

### Exploits of Mom
- I found this funny as this is a classic comical example of a malicious attack/ instruction to school system.
- The son's name being associated with DROP TABLE Students; actually instructs the database to drop the entire table of students from database records.
- There is also a good lesson to be understood in this story where the comic itself wants to make us to be aware of a critical security risks.

## a) Installing WebGoat 
- I tried installing first Java but $ sudo apt-get install openjdk-17-jre but unfortunately the package was not available anymore
- I installed Java 23.0.2 because it had some issues with webgoat. version check via java --version
<img width="822" height="550" alt="image" src="https://github.com/user-attachments/assets/eb88c934-fa21-4759-bccf-9e81800918c4" />

- I downloaded the local copy given in the website as the github link seems to not work with the terminal.
- I executed the command and we can observe WebGoat in action.

<img width="827" height="517" alt="image" src="https://github.com/user-attachments/assets/a2e90a35-a209-4788-a3e8-1eb7d0aaa867" />


<img width="943" height="558" alt="image" src="https://github.com/user-attachments/assets/1f97cea5-f71f-420c-96f8-41e0347ac3ea" />

-Finally We can browse in a normal browser to do the webgoat 

<img width="727" height="582" alt="image" src="https://github.com/user-attachments/assets/d7533ffd-780e-4bfd-981c-d1d9f329479b" />

- I created a new username and password while opening the WebGoat in my localhost. 

<img width="1251" height="808" alt="image" src="https://github.com/user-attachments/assets/7e41dc2f-4544-43e4-9684-f11dec8de56d" />

## b) F12. Solve Webgoat 2023.4: General: Developer tools.

- Developer tools lessons
<img width="1261" height="802" alt="image" src="https://github.com/user-attachments/assets/dcd0a361-d668-4c0d-8447-1becb057a4e6"/>

- Lesson1: opening up the developer tools 

- Lesson 2: Knowing the Elements Tab and CSS source.

- Lesson 3: The console Tab
- Console.log("Hello WebGoat"!)

- <img width="435" height="73" alt="image" src="https://github.com/user-attachments/assets/62065463-300e-4c8d-ab0f-ae034d11683b" />


- Lesson 4: Try it! Using the console
- First we use the the command webgoat.customjs.phoneHome()
<img width="980" height="833" alt="image" src="https://github.com/user-attachments/assets/5a323811-fb1f-4817-8c31-7134a9a98439" />

- Sucessfully generated teh phone home response number and moved on to the next level


<img width="1167" height="797" alt="image" src="https://github.com/user-attachments/assets/d265ecda-324d-4f6b-8d53-44278dfe3fe3" />

- Lesson 5: Learned in details about the sources tab & the network tab.
- Lesson 6: Try it! Working with the Network tab

I have sucessfully found out the request of Go button. 

- <img width="1178" height="812" alt="image" src="https://github.com/user-attachments/assets/809a5a7e-7889-4f5e-bf20-25da6c40fd91" />

## c) Updated every thing on my linux. 

<img width="742" height="532" alt="image" src="https://github.com/user-attachments/assets/11ec5c93-dff1-4830-ab3f-07d90c1ce7ae" />


<img width="987" height="702" alt="image" src="https://github.com/user-attachments/assets/0fcd3576-5b15-460b-a392-2329dc89d48e" />


## d) Sequel. Solve SQLZoo:
### 0 SELECT basics 

- <img width="840" height="777" alt="image" src="https://github.com/user-attachments/assets/3eb53371-3067-454a-99f5-272f59df74b5" />


- <img width="826" height="910" alt="image" src="https://github.com/user-attachments/assets/45273eaa-f755-4b6c-aece-f003d78eef88" />


- <img width="818" height="902" alt="image" src="https://github.com/user-attachments/assets/f1ff2993-62a3-46db-a8ef-ec5dadb3ca1b" />



### 2 SELECT from World: First two Subtasks 


- <img width="901" height="575" alt="image" src="https://github.com/user-attachments/assets/fd8ada7b-9cdd-4f05-b6e7-908cf9ff2f3b" />


- <img width="1028" height="780" alt="image" src="https://github.com/user-attachments/assets/7a1bf692-581e-4d57-a7b9-3d6693e8ecca" />


- <img width="913" height="691" alt="image" src="https://github.com/user-attachments/assets/86a76648-d534-4998-a2b4-075fb5328ee5" />


## Solving Portswigger Labs: 

- So I followed the instructions and opened up lab, had to create an account for it. Finally I finished my findings and succesfully did solved the Lab.
- I solved the lab by taking a peak at solution tab, it was unclear at first on what I was supposed to do there first, but, after I clicked the solution it got clearer and I applied to the Lab.
- Below is the result of its solution.

  <img width="1918" height="1025" alt="image" src="https://github.com/user-attachments/assets/0e9ba764-4673-445c-900f-bffce1a418be" />

- So, in this lab exercise I found the vulnerability of the website.
- Here in the URL parameter there is a possible SQL injection flaw.
- Adding ' to the parameter triggered a SQL syntax error.
- The payload uses OR 1 = 1, which always evaluates true.
- -- comments out the remaining SQL query.
- All data which were hidden are returned.

## m) Voluntary bonus: WebGoat: SQL Injection 

### Lesson-1 SQL Injection (Intro)
- This particular lesson in WebGoat describes the concept of Structured Query Language (SQL) and how it can be manipulated to perform malicious activities. SQL Injection is an attack which exploits vulneribilities in an application by inserting malicious SQL query into regular input. 

### Lesson - 2
- SQL is a standardized programming language which is used for managing relational databasees.
- Databases are collection of data, data are organized into rows, coloumn and tables.
- I sucessfully retrived data of the employee From employees in a specific deparment below is the action i performed.
<img width="898" height="648" alt="image" src="https://github.com/user-attachments/assets/b38b48b2-565a-420f-be9f-2283b3d218ed" />

### Lesson 3: Data manipulation Language (DML)
- So, I succesfully manipulated data in the SQL where I updated the employee named Tobi into department of sales. 
<img width="898" height="720" alt="image" src="https://github.com/user-attachments/assets/27890f29-b152-40e9-93ba-b9277988d312" />

### Lesson 4: Data Definition (DDL)
- DDL is focused on the structure of the database rather than the data inside.
- To modify an existing table without having to delete it, we must use the ALTER command combined with ADD for new coloumns.
- I solved this exercise by Inputing ALTER TABLE employees ADD phone varchar(20);
<img width="926" height="755" alt="image" src="https://github.com/user-attachments/assets/d684ca2e-7eda-4ac9-8e28-9896ad55cd9a" />


### Lesson 5: Data Control Language (DCL)

- It is used to implement access control logic in a database.
- Below I have solved this lesson too by granting all privileges. I tried grant_rights TO unauthorized_user;  

<img width="912" height="702" alt="image" src="https://github.com/user-attachments/assets/0be5909d-c30a-4ec9-809a-9cec7721af7c" />

### Lesson 6: What is SQL injection?
- It is the insertation or injection of the malicious code via the SQL query input from the client to the application.
- By using a statement that is always true, like 1=1, you can bypass filters or authentication to retrieve all records in a table instead of just one.


### Lesson 7: Consequences of SQL injection

- Modification of sensitive data
- execution of administrative operation on databases
- shutdown auditing or the DBMS
- adding users
- recover any content of the given file in DBMS.
- Issues command to the operating system.
- SQL injections allows attackers to spoof identity, tamper with data, allows complete disclousre of the data and much more. 

### Lesson 8: Severity of SQL injection
- I learned the severity of SQL injections here.
- They are more common in PHP, Classic ASP, Cold Fusion languages.
- Not all databases support command chaining.
- Not all databases are equal.

### Lesson 9: Try It! String SQL injection

- I did this lesson by using entering ' OR '1' = '1 so the final query becomes SELECT * FROM user_data WHERE first_name = 'John' AND last_name = '' OR '1' = '1'.
- The database gets confused here by the extra quotes and unexpected token.
<img width="1147" height="873" alt="image" src="https://github.com/user-attachments/assets/f0907c43-4f1f-47a5-a2f4-54f4f28d4bdc" />

### Lesson 10: Numeric SQL injection 
- In numeric SQL injection you can force the database to ignore the specific ID requirement by providing a dummy value followed by a statement that is always true.

<img width="906" height="662" alt="image" src="https://github.com/user-attachments/assets/35893d37-90a7-4f71-9102-5a1e443aaf4f" />

### Lesson 11: Compromising confidentiality with string SQL injection 
- I solved this by doing this: Entering Smith' OR '1'='1'-- in the employee name field on the forum leaving the authentication TAN blank. 

<img width="1151" height="787" alt="image" src="https://github.com/user-attachments/assets/42d6a6c3-0faa-4334-8213-ca3a8997dfe9" />

### Lessson 12: Compromising Integrity with Query chaining

- I did this task by inputing this into the input field of employee Name Smith'; UPDATE employees SET salary = '99999' WHERE last_name = 'Smith'-- .
- I left the TAN field blank too.
- SQL query chaining allows to change your own salary, first closing initial query's string and then writing a new DML statement targeting own record.
- I changed the salary to 480000 and earning the most money.

<img width="1148" height="792" alt="image" src="https://github.com/user-attachments/assets/912cd8ee-1195-496e-be07-516ab6b27ec0" />

### Lesson 13: Compromising Availability 

- To compromise the avilability in the SQL we have to use Drop statement to remove the data from the database.
- It removed entire table of access_log, which compromised Availability.
- Below is the work i have done i acheived it by executing '; DROP TABLE access_log;-- statements.

<img width="938" height="616" alt="image" src="https://github.com/user-attachments/assets/eb7d664f-222f-487c-b7d4-9d9c8c0ef3da" />



# Sources 

Karvinen, T. 2026.: Information Security. Available at: https://terokarvinen.com/information-security/

OWASP Foundation n.d.: Open Web Application Security Project (OWASP). Available at: https://owasp.org/

OWASP Foundation 2021: OWASP Top 10 – A01: Broken Access Control. Available at: https://owasp.org/Top10/A01_2021-Broken_Access_Control/

OWASP Foundation 2021: OWASP Top 10 – A05: Security Misconfiguration. Available at: https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

OWASP Foundation 2021: OWASP Top 10 – A06: Vulnerable and Outdated Components. Available at: https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

OWASP Foundation 2021: OWASP Top 10 – A03: Injection. Available at: https://owasp.org/Top10/A03_2021-Injection/

Munroe, R. n.d.: Exploits of a Mom (xkcd 327). Available at: https://xkcd.com/327/

Karvinen, T. 2023: WebGoat 2023 – Ethical Web Hacking. Available at: https://terokarvinen.com/2023/webgoat-2023-4-ethical-web-hacking/

SQLZoo Community n.d.: SQL Tutorial. Available at: https://sqlzoo.net/wiki/SQL_Tutorial

PortSwigger Ltd. n.d.: SQL Injection Lab – Retrieve Hidden Data. Available at: https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data
