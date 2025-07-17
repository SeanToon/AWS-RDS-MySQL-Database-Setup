# AWS-RDS-MySQL-Database-Setup

Search for and select RDS in AWS Home Console

<img width="1714" height="394" alt="image" src="https://github.com/user-attachments/assets/06272076-8f81-492c-894b-6b9a758c4e11" />

Select Create a database 

<img width="802" height="362" alt="image" src="https://github.com/user-attachments/assets/76a8f8c0-04a8-4ccc-99f2-66b2fd7d9d25" />

Select database creation method and engine option (for this setup, will be using "Standard Create" and "MySQL"

<img width="2988" height="1128" alt="image" src="https://github.com/user-attachments/assets/ba3f318d-fc3e-4a9d-b2dd-8ab826c2a0b3" />

Select the Edition, Engine Version, and Template (I selected version 8.0.42, and free tier to avoid charges)

<img width="3006" height="1356" alt="image" src="https://github.com/user-attachments/assets/5e88dffd-321f-412a-a74a-9c404fa1e67a" />

Name the database and master username, Create a master password

<img width="2388" height="1134" alt="image" src="https://github.com/user-attachments/assets/6d739a62-0453-4802-a336-bb53344b2345" />

For Instance config, select free tier version (selected db.t3.micro)

<img width="2216" height="786" alt="image" src="https://github.com/user-attachments/assets/afc21d2f-e2e9-4b24-98db-fb9a6c1df303" />

Storage and connectivity defaults are ok to be left alone except in connectivity allow public access 

<img width="2970" height="912" alt="image" src="https://github.com/user-attachments/assets/406d8447-7587-4acb-a162-cbd4dbe23661" />

Database successfully created!

<img width="2962" height="326" alt="image" src="https://github.com/user-attachments/assets/45b84420-4b53-405b-97fe-fb517e56710d" />

Connect to MySQL Workbench by first copying the endpoint

<img width="818" height="231" alt="image" src="https://github.com/user-attachments/assets/03d7ca7a-0940-4e0e-b95d-05a00081e8fb" />

In MySQL Workbench make a new MySQL Connection, name the connection, paste endpoint in hostname, enter username of database, enter password of database, and then click test connection 

<img width="2358" height="1366" alt="image" src="https://github.com/user-attachments/assets/52ac9b79-6d71-4bb1-b5da-5dc80bf4da52" />

If failure to connect 

<img width="508" height="252" alt="image" src="https://github.com/user-attachments/assets/591625f4-58be-42f8-b8b6-69540b8c9da7" />

Click on VPC security groups

<img width="1178" height="282" alt="image" src="https://github.com/user-attachments/assets/72a3f9f8-0820-4fe0-9ed1-37ed0cc1529b" />

Edit inbound rules 

<img width="1430" height="314" alt="image" src="https://github.com/user-attachments/assets/4f9343cb-74ac-49cf-b035-5b592fa555db" /> 

Create a new rule, Select "All Traffic" for type and "Anywhere-IPv4" for source type and save rule.

<img width="1482" height="1110" alt="image" src="https://github.com/user-attachments/assets/f76066b0-b7eb-4e13-8e83-bb1ba7f51731" />

Confirm connection in MySQL Workbench, run some simple queries, and there you go!

<img width="1164" height="970" alt="image" src="https://github.com/user-attachments/assets/2d8f3775-df93-4031-ba34-efa51d8ab245" />
