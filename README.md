# Title
Local Housing Market Intelligence Engine
## Project Goals
* Analyze local housing market trends
* Predict fair market home prices
* Explain predictions in a human-readable way
## Non-Goals
* Not building a full MLS (multiple listing service) replacement
* Not guaranteeing real-world pricing accuracy
* Not supporting every city initially
## Initial Market
* Region: San Diego County, CA
* Level of Analysis: ZIP-code level housing market analysis
## Dataset (Initial)
* File: ca_san_diego.csv
* Source: app.regrid.com, San Diego County, CA
* Records: 20 properties (sample)
* Columns: 203
* Data type: Property assesor and transaction records
* Level of Analysis: Parcel/ZIP-code level
### Key Fields Available:
* Sale price ('saleprice')
* Sale data ('saledata')
* Bedrooms ('num_bedrooms')
* Bathrooms ('num_bath','num_bath_partial')
* Year built ('yearbuilt')
* Assessed values ('improvval', 'landval', 'parval')
### Note: This initial dataset is intentionally small. The same pipeline will later be applied to a larger county-level dataset.
## Planned Approach
1. Acquire and inspect raw housing transaction data
2. Clean and preprocess data using pandas and NumPy
3. Use data analysis to show trends
4. Create predictive features
5. Train pricing models
6. Show predictions and insights through an API and simple UI
## Project structure
housing-intelligence/
  data/
      raw/
      processed/
  notebooks/
  src/
  api/
  app/
  README.md

# Tech Stack
* Python (pandas, NumPy, etc.)
* Jupyter Notebooks
* FastAPI (model inference)
* Streamlit (visualization)

