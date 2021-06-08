# ETL_Project
We are aiming to have clean datasets that allow us to compare multiple variables and how they relate to Covid vaccine rollouts around the globe.

Members: <br/>
William Powell<br/>
Jungkyu Kim<br/>
Kaixin Yang<br/>
Hannah Slay<br/>
Alex Gainer<br/>


1.	Extract: the original data sources and how they were formatted <br/>
  a.	 Covid World Vaccination Progress: <br/>
    i.	https://www.kaggle.com/gpreda/covid-world-vaccination-progress <br/>
  b.	World Happiness Data: <br/>
    i.	https://www.kaggle.com/unsdsn/world-happiness  <br/>
  c.	UN Country Statistics: <br/>
    i.	https://www.kaggle.com/sudalairajkumar/undata-country-profiles <br/>
  d.	All three files were found on Kaggle and were csv format <br/>
  e.	Used pandas to read cvs files <br/>

2.	Transform: what data cleaning or transformation was required <br/>
  a.	Dropped unnecessary columns <br/>
  b.	Retrieve most recent date from individual datasets using the .max() function <br/>
  c.	Merged most recent date dataframe with individual dataset to isolate latest date <br/>
  d.	Set index to country <br/>
  e.	Changed formatting on erroneous records using .replace() <br/>

3.	Load the final the database, tables, and collections and why this was chosen <br/>
  a.	Created ERD using Quick DB Diagrams <br/>
  b.	Created tables and relationships in Postgres <br/>
  c.	Loaded cleaned tables into Postgres using .to_sql in our Jupyter Notebook <br/>
