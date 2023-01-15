
For the Veris dataset, data wrangling is needed to reformat the data in order to conduct visualisations. 
The following steps are done for veris dataset (More info can be found here http://veriscommunity.net/vcdb.html):

Veris dataset preprocess and visualisation:

Dataset is curated in a way that all non-numerical column values are treated as a column with a true/false value.

Example:\
Normal dataset:\
Column: food\
Column value: rice, noodles, bread

Veris dataset:\
Column: food.rice, food.noodles, food.bread\
Column value: true,false


**Steps to perform on data:**
  1) Select features to look into (revenue, incident type, incident year, employee count, assets lost) 

  **Preprocess**: get each feature into a column and combine all columns to get the proper dataframe for visualisation

  2) Get all revenue entries (in many different currencies)
     Convert all currencies to USD

  3) Get the average employee count as employee count is only given in ranges(eg. 1-100)

  4) Get the incident types(total 7) which also has many subtypes for each of the 7 types, 
     located in column 'action. <incident type> .variety. <incident subtype>'

  4) Get all asset loss entries (in many different currencies)
     Convert all to USD

**Analysis**: Visualise trends


