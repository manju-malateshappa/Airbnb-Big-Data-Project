# Airbnb-Big-Data-Project
Must have things for running the code (IMPORTANT):

An active AWS account for accessing various AWS services
Tableau software for visualization.
Textblob library for calculating polarity of the review

Instruction for running the project:

run web_crawler.py file so as to download the data for the following cities:
a) Vancouver b) Montreal c) Toronto
The data will be downloaded and stored into the root directory in your local computer.
Create an AWS EC2 instance to transfer data from local computer to AWS S3 bucket
Create a cluster using AWS EMR to run Jupyter notebooks with pyspark
Use ListingsCleaner.py to do ETL for listings data on AWS EMR. ListingsCleaner.py will save the output back to AWS S3 bucket.
Use ReviewsCleaners.py to clean the reviews data on AWS EMR. ReviewsCleaners.py will save the output back to AWS S3 bucket.
Use ReviewsPolarityCalculator.py which calculates the polarity score and generates ReviewsPolarity.csv puts it back to AWS S3 bucket.
Use SuperhostClassifier.py to calculate whether the host is a super host or not on AWS EMR. The results will be printed in the console. The SuperhostClassifier.py will merge two data frames (listings and reviews) and create FinalListings.csv It will write the merged data into AWS S3 bucket.
Use AWS Athena to run SQL like queries on AWS S3 bucket which contains FinalListings.csv.
Transfer FinalListings.csv data from AWS S3 bucket to AWS redshift.
10.Load the data from AWS redshift into AWS Quichsight to create various dashboards.
Establish the connection between AWS redshift and tableau to make dashboards on the tableau.
PS: As we also provided the code of our website, please install all the node dependencies prior to run the application.

#Our Website can be reached at -> https://team404-732project.herokuapp.com

