# LGPD Standards for CATE Project

## Data:

The data will go through 5 steps, including:

1. **Extraction:** Excel base extracted to the database. 
<br> As agreed with the company Dom Rock (parent company) no data will be discarded on the basis provided, i.e. the analysis must be done with all data. 
<br> This data will be stored in a Mongo Cloud database that has NoSQL structure.  <><br>
2. **Data cleansing:** Checking for errors in the bank data. 
<br> This step will be checked if there is any data with error or null and it will be treated or discarded according to the guidance of the parent company.  <><br>
3. **Data scope:** Creation of a new collection of data needed for the final product. 
<br> In this step the clean data will be inserted into a new collection containing only the information needed for reporting.  <><br>
4. **Relational bank:** Creation of a DW relational bank. 
<br> A new relational database will be created with the data coming from the previous step, thus preparing for display in the Power BI tool.  <><br>
5. **Display of data:** Display of data in chart form. 
<br> The data is displayed bringing the information through charts and reports by beneficiaries of the four possible cases that may occur. 

## Hits:

Data manipulation will be done through two levels of access. 

* **Level 1:** Users responsible for steps *1 - Extraction* and *2 - Data cleansing*. 
<br> Only these users will have access to the complete database and the Mongodb Cloud database. 

* **Level 2:** Users responsible for steps *3 - Data scope*, *4 - Relational bank* and *5 - Data display*, being able to manipulate the data already processed by Level 1 users. 

## Logs:

In this project there is the traceability of the data through logs, where for this purpose there are 
the following models:

1. **General:** Saves information from all project data manipulation.  <><br>
2. **Anonymizer:** Saves all anonymization information from the data used in the processes.  <><br>
3. **Backuplog:** Concatena all processes executed on the day thus generating a backup of the logs executed.
<br><br> Logs are generated automatically when a process starts. At the end, files are generated that can be consulted later, facilitating the traceability of information.
<br><br> Below project-generated log model: <br><br>
 ! [](https://github.com/API-6-SEMESTRE/Documentacao/blob/main/LGPD/imagens/imagemLog.png)

<br><br> Being the stages of processing project data exposed and explained in the body of this document, it is agreed with the company Dom Rock that accepts the processes in the way it was presented.

<br> Both parties to agreement, we The Velopers firm the commitment to the realization of the steps mentioned and described.
