AUTHORS: Xiaoying Qu and Yiming Xia as a final project for CS257, Software Design


To use:
# first initialize the car2022 database
sudo service postgresql start
cat data.sql | psql -U postgres car2022_db
# api.py will access car2022_db with credentials in config.py

# run the flask webapp with
python3 app.py localhost 5000
# access this database-linked website on brower with
http://localhost:5000/

different properties of car models, can sort by fuel and co2 and engine size.
DATA: a dataset of 700+ car models manufactured in 2022 and their attributes, such as makes (e.g. Ford, Audi, Toyota etc.) and vehicle class (e.g. two-seater, compact, SUV: small etc.).

Our dataset comes from https://www.kaggle.com/datasets/rinichristy/2022-fuel-consumption-ratings.

STATUS:

- the home page works great.
- each car model's individual page is great.
- sort page displays directs user to individual car page.
- data visualization feature could be more robust. This includes implementing charts or scatter plots for to see correlations between makes and CO2 emission. If we had more time, we would add features that allow sorting with multiple parameters as well as choosing how many lines of data the users want to display on their screen in the sort page.

NOTES: no notes, but thanks professor Jeff Ondich for all your help this term
