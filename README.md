# Targetome ETL

This repository contains scripts that support the Targetome ETL pipeline. The Targetome dataset is available as a MySQL dump, and can be found here: https://github.com/ablucher/The-Cancer-Targetome. 

Steps to export the required TSV files from the Targetome MySQL dump.

1. Download the MySQL dump from the repo: https://raw.githubusercontent.com/ablucher/The-Cancer-Targetome/master/database/Druggability_070717.sql. 

2. Load the SQL file into a MySQL instance. 

3. Run the targetome-etl-flatten.sh script in this repo. The shell script may need to be updated to point to your MySQL instance. 

The exported TSV files can then be used in the Targetome ETL pipeline.

The targetome-etl.sh script is an older script and remains in the repo for historical purposes. 


