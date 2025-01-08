### DB_Lemmatization
Includes codes I created within Mentalism project for lemmatization of a db, calculating n_grams matrixies, tfidf matrixies, baseline estimates

## File Descriptions

- **`Lemmatization_reserach.ipynb`**: In this file I created function for downloading, cleaning, and after lemmatizing tweets (for Stanza ans Spacy packages). Also I tried to experiment and customize pipiline for text processing. In the result it was decided to use spacy package, since it was less aggressive.
- **`Script_for_lemmatizing_db.py`**: Script for leammtizing a db in batches adapted to SBATCH.
- **`delete.py`**: Script for deleting empty batches after lemmatization.
- **`upload_to_sql.py`**: Script to upload lemmatized tweets from parquet files to sql db.
- **`n_gram.py`**: Script for creating n_gram matrix with top 50000 frequent n_grams.
- **`tfidf.py`**: Script for creating tfidf matrices for each group.
- **`Baseline Estimates/el_net_cv.py`**: Script leverages ElasticNet regression with k-fold cross-validation on survey data enriched with TF-IDF features, derived from a lemmatized Twitter database, to predict survey responses.
