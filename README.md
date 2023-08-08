# Data 1202 Final Project - Data Archive

### This assignment compounds with Data extraction, Data transformation, and Data loading system.
<br/>

# 1. Data Selection - Find the datasets from kaggle.com for select the data to process.

### Select the Airline Passenger Satisfaction dataset from kaggle.com for analyzing.

__URL :__ [Airline Passenger Satisfaction](https://www.kaggle.com/datasets/mysarahmadbhat/airline-passenger-satisfaction)

When extract the downloaded a zip file, there is a CSV file name "airline_passenger_satisfaction.csv". It has <b>24</b> variables and <b>129,880</b> observations.  

![Screenshot](./img/data_selection/airline_satis_csv.png)

The zip file also give a data dictionary file as a CSV file named "data_dictionary.csv" to reference.

![Screenshot](./img/data_selection/airline_satis_datadict.png)

### Summary

Once the gathered datasets are ready. Now it should move to another process which is uploaded into database.

<br/>

# 2. Data Extraction - Upload dataset into database

### Step 1: Create a schema

Before upload the datasets, it requires to create a schema named "airline_quality" with SQL command below

```sql
CREATE SCHEMA `airline_quality`;
```

When execute the command above, the MySQL database creates a new schema as entered the command.

![Screenshot](./img/data_extraction/create_schema.png)

<br/>

### Step 2: Uploaded datasets into the created schema

Use the MySQL Workbench tool to upload the datasets with this step below

1. Right-Click on tab __tables__, select __Table Data Import Wizard__.

![Screenshot](./img/data_extraction/selected_table_data_import_wizard.png)

2. Select the dataset file path

#### Before Select file

![Screenshot](./img/data_extraction/choose_file_path.png)

Select the CSV file by click on __Browse...__ button

#### After Select file

![Screenshot](./img/data_extraction/selected_file_path.png)

Click __Next__ button

3. Review default generate table name, or change the table name

![Screenshot](./img/data_extraction/view_table_name.png)

Click __Next__ button

4. Review auto generate data type from imported CSV file

![Screenshot](./img/data_extraction/view_imported_datatype.png)

Click __Next__ button

5. Review overall process 

![Screenshot](./img/data_extraction/view_overview_before_import.png)

Click __Next__ button

6. Importing the data

![Screenshot](./img/data_extraction/importing_data.png)

Click __Next__ button

7. Import result

![Screenshot](./img/data_extraction/import_result.png)

Click __Finish__ button

8. View data result

![Screenshot](./img/data_extraction/imported_table.png)

<br/>

9. Select data from imported dataset into table with SQL command

```sql
SELECT * FROM airline_passenger_satisfaction;
```

#### Result

![Screenshot](./img/data_extraction/select_query_result.png)

### Step 3: Create dimension tables what are related to the Airline Passenger Satisfaction as the fact table as shown as diagrams below

![Screenshot](./img/data_extraction/ER_Diagram.png)

#### Create class type table to store class type as structure

```sql
-- Create class_type table
```

<br/>

# 3. Data Transformation

<br/>
<br/>

# 4. Data Loading

<br/>
<br/>

# 5. Reflection

```sql
SELECT * FROM TABLE;
```

```py
print("hello world")
```

```py
print("something")
```

```sql
select * from TABLE;
```