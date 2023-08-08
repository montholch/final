# Data 1202 Final Project - Data Archive

### This assignment compounds with Data extraction, Data transformation, and Data loading system.
<br/>

# 1. Data Selection - Find the datasets from kaggle.com for select the data to process.

### Step 1: Select the Airline Passenger Satisfaction dataset from kaggle.com for analyzing.

__URL :__ [Airline Passenger Satisfaction](https://www.kaggle.com/datasets/mysarahmadbhat/airline-passenger-satisfaction)

When extract the downloaded a zip file, there is a CSV file name "airline_passenger_satisfaction.csv". It has <b>24</b> variables and <b>129,880</b> observations.  

![Screenshot](./img/data_selection/airline_satis_csv.png)

The zip file also give a data dictionary file as a CSV file named "data_dictionary.csv" to reference.

![Screenshot](./img/data_selection/airline_satis_datadict.png)

### Step 2: Create the dimension tables to store information what related to Airline Passenger Satisfaction dataset.

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

#### After Select file



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