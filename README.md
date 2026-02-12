# Bank Marketing Data Engineering Project
Clean, transform, and split Bank Marketing Campaign Data with Python into three structured CSV files:

Versions: 
 - V1: Working with CSV Files 
 - V2: Working with Snowflake
   
## Repository Structure

```
Bank-Marketing-Data-Engineering/
│
├── db_tables/
│   ├── bank_marketing.csv      # Raw source file – original dataset ingested into Snowflake
│   ├── CLIENT.csv              # Output – cleaned client demographics table
│   ├── CAMPAIGN.csv            # Output – cleaned campaign interactions table
│   └── ECONOMICS.csv           # Output – cleaned economic indicators table
│
├── scripts/
│   ├── transform_tables_with_Snowflake.ipynb   # Version 2.0 – Snowflake-native ETL pipeline
│   └── transform_tables_with_csv.ipynb         # Version 1.0 – Legacy CSV-based ETL processing
│
├── .gitignore                 # Git ignore configuration
└── README.md                 # Project documentation
```

                            



🔄 Data Transformations
Client Data Cleaning

✅ Replace "." with "_" in job and education fields
✅ Convert "unknown" to NaN in education column
✅ Convert credit_default to boolean (1 if "yes", else 0)
✅ Convert mortgage to boolean (1 if "yes", else 0)

Campaign Data Cleaning

✅ Convert previous_outcome to boolean (1 if "success", else 0)
✅ Convert campaign_outcome to boolean (1 if "yes", else 0)
✅ Create last_contact_date from day, month, and year (2022)
✅ Format date as YYYY-MM-DD

Economics Data

✅ Extract economic indicators with client_id linkage
