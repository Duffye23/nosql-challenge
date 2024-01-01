# nosql-challenge

The point of this challenge was to create a non-sql database and to connect to the provided UK Food database in order to evaluate the ratings data in order to decided where journalists and food critics should focus future articles.</br>
The first part of the challenge was to create the MongoDB database and import the UK Food database.</br>
The challenge specified to do so via the command line, but MngoDB Compass has a feature which bypasses this and makes it much more intuitive. Described below:</br>
Create a new database via the plus symbol and name the database and collection appropriately and clicke "create database".
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/80bd2a1f-a092-402d-9e5f-0ddfd3919edb)
Next, simply click "Add DATA" and then select the appropriate file type, JSON in this case.
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/73cb2bfa-8e49-40ba-82c9-5e0a2f910935)
Then, navigate to where the file resides in your storage, and import it into your database.
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/41dc723d-e646-46db-951e-7d870ca1fc0e)
You will be sent to a final page confirming that the data is correct and to import it.
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/51b5930b-4abd-4c1c-9b79-0d0cc6254f4b)
Once imported, your database will be compiled by Compass and ready in seconds.
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/5e1e2b5c-00d0-4d20-86a7-4a1cb9224bcb)</br>

Once the database was created, it had to be connected to the notebook in order for any analysis to be run.</br>
Showing which libraries were used and how the connection to the database was created</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/af2c1052-b92a-488e-a92e-9136c4aa5af2)

The next part was to update the database with a restaurant called "Penang Flavours", the restaurant data was provided in the challenge criteria. We took the data provided and created a new variable, containing a dictionary with the data and simply inserted the variable into the database. We then verified that it had been inserted by checking for its id.</br>
The variable with "Penang Flavours":</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/c5025b60-0d28-462c-b827-61bc11628e65)</br>

Inserting and checking the ID:</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/6a8e4f30-7bd5-4ce1-9929-8a9e236b8dbc)</br>

Exploratory Analysis was then performed which culminated in finding which establishments had a hygiene score of 20, which establishments had ratings 4 or higher, finding the top 5 establishments sorted by hygiene score that were fclosest to "Penang Flavours", and finally finding how many establishments in each local authority had a hygiene score of 0. These were then transformed into pandas dataframes.</br>

Establishments with Hygiene Scores of 20:</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/4cb08956-3966-4111-9370-c7bb9d241075)</br>

Establishments with ratings equal or greater than 4:</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/e502a693-815a-4e9c-8c48-abf33e7951bc)</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/522cc14e-fe19-47d2-b4cf-f596eddd3f95)</br>

Top 5 Establishments closest to Penang Flavours sorted by hygiene score:</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/f5af4ef4-5d48-4a05-8b55-407ba2961c91)</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/a74e3b18-a7be-4c48-bea7-80d05817435b)</br>

Establishments with a hygiene score of 0:</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/6b6aba4e-2cf3-4bff-9f81-c9b51ed31e00)</br>
![image](https://github.com/Duffye23/nosql-challenge/assets/58863493/0959d646-e59f-4cf5-8a7e-87d2c04d53ea)</br>

Sources Cited:
- Carleton Bootcamp materials, including zoom replays and learning activities.













