# ETL_Project
We are aiming to have clean datasets that allow us to compare multiple variables and how they relate to Covid vaccine rollouts around the globe.


1.	Extract: the original data sources and how they were formatted <br/>
  a.	 Covid World Vaccination Progress:
    i.	https://www.kaggle.com/gpreda/covid-world-vaccination-progress
  b.	World Happiness Data:
    i.	https://www.kaggle.com/unsdsn/world-happiness 
  c.	UN Country Statistics:
    i.	https://www.kaggle.com/sudalairajkumar/undata-country-profiles
  d.	All three files were found on Kaggle and were csv format
  e.	Used pandas to read cvs files

2.	Transform: what data cleaning or transformation was required
  a.	Dropped unnecessary columns
  b.	Retrieve most recent date from individual datasets using the .max() function
  c.	Merged most recent date dataframe with individual dataset to isolate latest date
  d.	Set index to country
  e.	Changed formatting on erroneous records using .replace()

3.	Load the final the database, tables, and collections and why this was chosen
  a.	Created ERD using Quick DB Diagrams
  b.	Created tables and relationships in Postgres
  c.	Loaded cleaned tables into Postgres using .to_sql in our Jupyter Notebook
