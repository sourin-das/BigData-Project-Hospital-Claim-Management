# BigData-Project-Hospital-Claim-Management
This is a project about Hospital Claim Management System, to filter, cleanse, transform raw data to Processed data and analyze insights from it with the help of Big Data.

Project Name: Hospital Claim Management System

Technologies used: Unix, Python, MySQL, Hive, SQOOP and Hadoop HDFS for data storage and processing.

We have considered 3 patient csvs for different countries, India, USA and Germany.
We have Claim, Insurer that is the Insurance Company, Hospital, Groups of disease and subgroups of disease modules.

Patient- This module is to display the patient name, insurance ID, address, phone number, age, type of insurance, nationality etc..gives the detailed information of patient.

Claim- This module is to display the claim id, claim type whether it is cashless or reimbursement, 
amount of claim, risk category level as High, Medium and Low, status etc.. This module is a request that a health insurance policyholder submits to the Insurance Company in order to obtain the services.

Insurer- This module is the Insurance company with insurance id, name, status, effective dates, 
insurance amount etc...This module is used to pay for the patient's healthcare cost according to the claim.

Group- This module will summarise the various disease parent type for every claim. Like Accidental, surgery etc.

Hospital- This module holds information about the hospitals that patients get admitted to, contains Hospital information.

Subgroup- This is a child module for group, that contains the detailed disease name under each group.

Then after applying data cleansing like removing Null values and duplicates we transfer these files as tables in MYSQL.

Then after applying Transformation logic to those data using python, we create the FINAL_TABLE and then import all the tables to HIVE, by using SQOOP, and HDFS for storage.

Finally, we output the graphs as necessary by using matplotlib library of python and display the same.
