AUTHORS: Xiaoying Qu and Yiming Xia as a final project for CS257, Software Design


To use:
# first initialize the car2022 database
sudo service postgresql start
cat data.sql | psql -U postgres car2022_db
# api.py will access pokemon_db with credentials in config.py

# run the flask webapp with
python3 app.py localhost 5000
# access this database-linked website on brower with
http://localhost:5000/


DATA: a dataset of 500+ Pokemon and their attributes, such as types (e.g. water, fire, grass, electric, flying, etc.) and abilities (e.g. berserk, dazzling, fur coat, gluttony, etc.).

Our dataset comes from https://www.kaggle.com/mrdew25/pokemon-database.

STATUS:

- the home page works great.
- each Pokemon's individual page is great.
- the infinite scrolling mechanism is awesome.
- the handling of user input on the advanced search page could be more robust. The user isn't alerted if some non-digit character (other than a hyphen, which is allowed), is entered into a field that is supposed to contain digits. We also don't check for this when processing user input. We would add this if we had more time.




AUTHORS: Xiaoying Qu and Yiming Xia

DATA: different properties of car models, can sort by fuel and co2 and engine size.

our data comes from kraggle.com (https://www.kaggle.com/datasets/rinichristy/2022-fuel-consumption-ratings)

STATUS:

working:
- working html pages with css
- href between home page to serach page and sort page
- connection to database
- search page can search for car makes in database 
- sort page can sort by either fuel_consumption or co2
- carpage gets data from database to display to user
- the list sort page and sort page displays directs user to carpage

not-yet-implemented-but-would-like-to-if-we-have-more-time-features:
- sort with multiple parameters
- allow user to choose how many lines of data they want to display on their screen in the sort page.

NOTES: no notes, but thanks professor for all your help this term
