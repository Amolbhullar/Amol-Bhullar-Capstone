# Amol Bhullar Capstone

# Project Overview

The objective of this Capstone project is to develop a machine learning classifier that can predict whether a product is gluten-free or not based on its product description. The project will leverage a dataset containing product descriptions and their corresponding gluten-free status labels.


# Problem Statement

Gluten-free diets are crucial for individuals with celiac disease or gluten sensitivity. However, identifying gluten-free products can be challenging, especially when the product description does not explicitly state its gluten content. The goal of this project is to create a machine learning model that can automatically analyze product descriptions and classify products as gluten-free or non-gluten-free, providing a convenient solution for consumers seeking gluten-free options.


# Proposed Data Science Solution:

1. Dataset 1: Gluten-Free Ingredients

This dataset will contain a comprehensive list of known gluten-free ingredients. It will serve as a reference for identifying gluten-free components in product ingredient lists.

2. Dataset 2: Product Descriptions and Labels


This dataset will include product descriptions along with their gluten-free status labels. The labels will indicate whether the product is gluten-free (0: gluten-free, 1: non-gluten-free).

3. Data Preprocessing:

Clean and preprocess the product ingredient lists by removing punctuation, converting text to lowercase, and handling any special characters.

4. Machine Learning:

Train a machine learning model using the preprocessed data from Dataset 2. By vectorizing the ingredient lists using CountVectorizer, and then training a Naive Bayes classifier, Logistic Regression, Decision Tree and distilbert-base-uncased Model to make predictions on the test set.

5. Model Evaluation:

Evaluate the model's performance using accuracy, precision, recall, and F1-score metrics.
Ensure the model effectively distinguishes between gluten-free and non-gluten-free products.

6. Deployment:

Deploy the trained model as a user-friendly tool where users can input product descriptions to determine their gluten-free status.

# Impact of the Solution:

The developed gluten-free product classifier will have several benefits:

1. Empower consumers: Individuals with celiac disease can confidently identify safe gluten-free products to include in their diet.
2. Time-saving: The classifier will provide quick and automated results, saving consumers time spent manually analyzing ingredient lists.
3. Promote gluten-free choices: The tool can encourage individuals to adopt gluten-free diets by simplifying product selection.

# Dataset Description:

Dataset 1: Gluten-Free Ingredients

This dataset will contain a list of gluten-free ingredients sourced from reliable gluten-free certification organizations, health authorities, and research papers (labeled as 1 for gluten-free and 0 for non-gluten-free).

Dataset 2: Product Ingredient Lists

This dataset will include ingredient lists from various products, some of which are gluten-free, and others that may contain gluten. It will be used to train and evaluate the machine learning model.
Each entry in this dataset will include the ingredient list of a product along with its gluten-free status (labeled as 1 for gluten-free and 0 for non-gluten-free).

# Data Dictionary (Dataset 1):

Ingredient: The name of the ingredient.
Gluten?: A binary target variable indicating whether the ingredient is gluten-free (0: gluten-free, 1: non-gluten-free).

# Data Dictionary (Dataset 2):
1. fdc_id: ID of the food in the food table
2. brand_owner: Brand owner for the food
3. gtin_upc: GTIN or UPC code identifying the food
4. ingredients: The list of ingredients (as it appears on the product label)
5. serving_size: The amount of the serving size when expressed as gram or ml
6. serving_size_unit: The amount of the serving size when expressed as gram or ml
7. household_serving_fulltext: The amount and unit of serving size when expressed in household units
8. branded_food_category: The category of the branded food, assigned by GDSN or Label Insight
9. data_source: The source of the data for this food. GDSN (for GS1) or LI (for Label Insight).
10. modified_date: This date reflects when the product data was last modified by the data provider, i.e., the manufacturer
11. available_date: This is the date when the product record was available for inclusion in the database.
12. discontinued_date: This is the date when the product was discontinued.
13. market_country: The primary country where the product is marketed.

# Data Dictionary (Dataset 3):
1. fdc_id: ID of the food in the food table
2. foodClass: For internal use only
3. data_type: Type of food data (see Files tab for possible values).
4. description: Description of the food
5. food_category_id: Id of the food category the food belongs to
6. publication_date: Date when the food was published to FoodData Central
7. scientific_name: scientific_name
8. food_key: A string of characters used to identify both the current and all historical records for a specific food.