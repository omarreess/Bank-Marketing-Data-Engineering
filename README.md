# Bank Marketing Data Engineering Project
Clean, transform, and split Bank Marketing Campaign Data with Python into three structured CSV files:

client.csv - Customer demographic information
campaign.csv - Marketing campaign interactions
economics.csv - Economic indicators

🗂️ Project Structure
Bank-Marketing-Data-Engineering/
│
├── notebook.ipynb           # Main notebook
├── bank_marketing.csv       # Source data (raw)
├── client.csv              # Output: Client demographics
├── campaign.csv            # Output: Campaign data
├── economics.csv           # Output: Economic indicators
└── README.md               # Project documentation

🔧 Technologies Used

Python 3.x
Pandas - Data manipulation and transformation
NumPy - Numerical operations and data type handling


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
