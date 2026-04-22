# Shelter-Dog-Adoption-Rates-Project
This project aims to predict the adoptability of shelter dogs based on various features in order to help animal shelters more efficiently identify dogs that are unlikely to be adopted. With this quick identification, shelters can allocate their resources more efficiently to the dogs that need the most help and boost their chances of being adopted. This increases the shelter’s adoption rate and the amount of time dogs spend in shelters, and thus decreases the shelter’s cost per dog. 

You will find the data used and our initial modeling and EDA in the “Data and EDA” folder, and our Jupyter notebooks in the folder labeled as such. The final tableau dashboard is named “Shelter Dogs Dashboard”.

To replicate this project in AWS:
1. Store the San Jose Animal Shelter CSV file in an S3 bucket.
2. In a SageMaker AI Notebook, upload the Jupyter Notebooks “predictions-2.ipynb” and “train_ml_models-3.ipynb”. These notebooks clean the data, train logistic regression and random forest models, and generate prediction scores on each dog in the dataset. The notebooks finish by saving to Amazon RDS, where the scored animal records and prediction outputs are stored in a structured table.
3. To create a Tableau dashboard with the data, simply connect Tableau to RDS using MySQL. This dashboard enables shelter staff to immediately glean useful information about any dog they may have in the shelter.
