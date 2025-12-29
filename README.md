# Databricks_assignment


# Question 1



# Create 3 folders as source_to_bronze, bronze_to_silver, silver_to_gold.

<img width="1913" height="597" alt="Screenshot 2025-12-26 235406" src="https://github.com/user-attachments/assets/345a5677-eb96-412e-8882-677e978f729f" />


# 2. Create 4 notebooks in this respective order. 
* 2 Notebooks named in source_to_bronze as utils (add all common functions in this notebook) and employee_source_to_bronze (driver notebook)
* 1 Notebook in bronze to silver as employee_bronze_to_silver
* 1 Notebook in silver to gold as employee_silver_to_gold

#  2 Notebooks named in source_to_bronze as utils (add all common functions in this notebook) and employee_source_to_bronze (driver notebook)

<img width="1917" height="742" alt="Screenshot 2025-12-26 235951" src="https://github.com/user-attachments/assets/27fd832b-05c7-4652-a7f5-9d19159d2dbb" />


#   1 Notebook in bronze to silver as employee_bronze_to_silver

<img width="1919" height="722" alt="Screenshot 2025-12-27 000056" src="https://github.com/user-attachments/assets/beb73d22-b5b8-4bcb-a19c-713a5af23093" />


#  1 Notebook in silver to gold as employee_silver_to_gold


<img width="1919" height="790" alt="Screenshot 2025-12-27 000206" src="https://github.com/user-attachments/assets/5e15a248-bfa6-4f5f-bffc-35b373601312" />


# 3 . Read the 3 datasets as Dataframe in employee_source_to_bronze, call utils notebook in this notebook, and write to a location in DBFS, as /source_to_bronze/file_name.csv (employee, department_df, country_df) as CSV format
<img width="1913" height="1060" alt="Screenshot 2025-12-27 005117" src="https://github.com/user-attachments/assets/e858a2b2-48a3-4a26-a417-6c1c5603e86a" />

<img width="1811" height="879" alt="Screenshot 2025-12-27 005142" src="https://github.com/user-attachments/assets/22a84947-b69d-4621-aac2-7e021924dbbf" />

<img width="1908" height="945" alt="Screenshot 2025-12-27 005159" src="https://github.com/user-attachments/assets/39039a58-90ac-4c33-8be1-c96f7bf83058" />

<img width="1904" height="590" alt="Screenshot 2025-12-27 005214" src="https://github.com/user-attachments/assets/a6b00010-f162-4cfc-99e5-80050e223c49" />


# 4. In employee_bronze_to_silver, call utils notebook in this notebook. Read the file located in DBFS location source_to_bronze with as data frame different read methods using custom schema.


<img width="1919" height="1057" alt="Screenshot 2025-12-27 131151" src="https://github.com/user-attachments/assets/120aa89d-e454-4f79-a494-4b2e68a62b55" />
<img width="1918" height="750" alt="Screenshot 2025-12-27 131211" src="https://github.com/user-attachments/assets/a6f70cec-ad7f-4fb6-ab68-8231e8875b98" />
<img width="1919" height="660" alt="Screenshot 2025-12-27 131244" src="https://github.com/user-attachments/assets/fa702c08-6f9e-4053-8b28-af8f6cd8c7de" />


# 5.convert the Camel case of the columns to the snake case using UDF. 
<img width="1919" height="1073" alt="Screenshot 2025-12-27 132007" src="https://github.com/user-attachments/assets/5e388028-53ef-452f-962d-ea00a7df0d1e" />

<img width="1919" height="761" alt="Screenshot 2025-12-27 132038" src="https://github.com/user-attachments/assets/189f61db-584d-4577-8b67-f73ae0f18de6" />

# 6. Add the load_date column with the current date.

<img width="1911" height="1075" alt="Screenshot 2025-12-27 132452" src="https://github.com/user-attachments/assets/425343d5-c356-47ab-ad2c-7c40cc52086f" />


# The primary key is EmployeeID, the Database name is Employee_info, Table name is dim_employee. 
 # write the DF as a delta table to the location /silver/db_name/table_name. 


<img width="1275" height="562" alt="Screenshot 2025-12-28 164234" src="https://github.com/user-attachments/assets/29db5e58-15c8-4347-a4a7-0abad90ac25f" />
<img width="1014" height="435" alt="Screenshot 2025-12-28 164249" src="https://github.com/user-attachments/assets/19c4906e-ceed-437b-a78a-2f5a71ad2965" />

 write the DF as a delta table to the location /silver/db_name/table_name. 

# 8. Gold Layer Requirements
# Salary of each department (descending)
<img width="1274" height="560" alt="Screenshot 2025-12-29 231238" src="https://github.com/user-attachments/assets/e5024004-dbb1-469a-bd5d-c16c67af3292" />

 
 # Employee count per department per country
<img width="793" height="544" alt="Screenshot 2025-12-29 231255" src="https://github.com/user-attachments/assets/197966c6-b09c-47b2-ab1e-5ca9544648ae" />


 # Map of departments ↔ countries
<img width="1104" height="507" alt="Screenshot 2025-12-29 231308" src="https://github.com/user-attachments/assets/bff55ccc-98a1-4ead-81b8-ea288e323cf2" />


 # Average age by department
<img width="946" height="492" alt="Screenshot 2025-12-29 231320" src="https://github.com/user-attachments/assets/7b325456-14e7-4250-bb69-1d366830215e" />


 # Add at_load_date
 <img width="1112" height="581" alt="Screenshot 2025-12-29 231340" src="https://github.com/user-attachments/assets/f1fc32b9-284f-47ca-8e72-aa8af9ce612c" />


# Write GOLD table to Delta
 <img width="866" height="251" alt="Screenshot 2025-12-29 231438" src="https://github.com/user-attachments/assets/b0464de6-b6c6-46ce-80ad-c37ec050451d" />

