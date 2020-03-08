# Movies-ETL
Assumptions:
1. The three arguments that the function takes refer to file path locations, and these file path locations must be able to be read into a data frame using pd.DataFrame()
2. The wikipedia file path and the kaggle file path must have imdb_id columns in order for the two columns to be joined with an inner join. 
3. The user must be connected to a postgres data base, and must change their password in the config file to their own file 
4. Within postgres, the user must have a database called 'challenge-movie' in order for the data to be loaded
5. the code assumes that the wiki_file_path argument in the function is a JSON file and can be read using the json.load method.
6. The wiki_file_path argument refers to a file path, and this file path must have a column for Director, or Directed By, as well as a column for the IMDB link. Otherwise, data will not be included in the final export. 
