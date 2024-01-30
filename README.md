# java-DB-datatypes

#### 1. Enum data type usage

- Create enum that will contain statuses 'NEW', "PAID", "WAITING FOR PAYMENT".
- Create table "Invoices" with columns: buyer, seller, value, account number, status. Chose the right column types.
- Insert a few rows into this table with different statuses.
- Select only those invoices with status = "NEW"

#### 2. UUID data type usage

- Modify table "Invoices" - add column that will keep "internal_id". 
- Update each row with a value in a column "internal_id". You can use this generator: https://www.uuidgenerator.net/

#### 3. JSON data type usage

- Modify table "Invoices" - add 2 columns that will keep json view of an entity. One column should be with type json and other with type jsonb.
- Try to fill newly created columns with below json:

'{
  "buyer": "company a",
  "seller": "company b",
  "status": "NEW",
  "account_number": 123321123
  "value": 23.43
}



#### 4. Array data type usage

- Modify table "Invoices". Add a column where phone numbers of buyer will be kept. Maximum number of those number is 3.
- Insert a list of phone numbers for an invoice with id = 3: 123211233, 125433221, 127643454
- Insert a list of phone numbers for an invoice with id = 2: 432323112, 123344311
- Select buyer name and his LAST phone number for invoice with id = 3;
- Select an invoice which contains phone: 432323112 

#### 5. Binary data type usage

- Create a file, can be an image or just a text file
- Create a new column in Invoices table that will keep this file
- Insert this file into database for invoice with id = 1


#### 6. Date/time data types usage

- Modify table "Invoices", add 4 new columns: payment deadline, transaction time, transaction hour, cyclic payment. Choose the right column types. 
- Update each column with values
- Update timezone in transaction type, set it to be Melbourne, Australia. 
- Update timezone in transaction time column, set it to be Melbourne, Australia. 
- Select transaction time column, make sure that 10 hours has been added to the time that previously was set.
