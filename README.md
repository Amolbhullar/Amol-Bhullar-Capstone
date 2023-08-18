# Amol Bhullar Capstone

# Project Overview

The objective of this Capstone project is to develop a machine learning model that can predict whether a product is gluten-free or not based on its ingredient list. The project will utilize two datasets: one containing a list of known gluten-free and gluten-containing ingredients and another containing ingredient lists of various products.

# Problem Statement

Gluten-free diets are essential for individuals with celiac disease or gluten sensitivity. However, identifying gluten-free products can be challenging, as gluten can hide under various ingredient names. The goal of this project is to create a tool that can automatically analyze ingredient lists and classify products as gluten-free or non-gluten-free, providing a convenient solution for consumers seeking gluten-free options.

# Proposed Data Science Solution:

1. Dataset 1: Gluten-Free Ingredients

This dataset will contain a comprehensive list of known gluten-free ingredients. It will serve as a reference for identifying gluten-free components in product ingredient lists.

2. Dataset 2: Product Ingredient Lists

This dataset will include ingredient lists from various products, some of which are gluten-free and others that may contain gluten. It will be used to train and evaluate the machine learning model.

3. Data Preprocessing:

Clean and preprocess the product ingredient lists by removing punctuation, converting text to lowercase, and handling any special characters.

4. Machine Learning:

Train a machine learning model using the preprocessed data from Dataset 2. By vectorizing the ingredient lists using CountVectorizer, and then training a Naive Bayes classifier to make predictions on the test set.

5. Model Evaluation:

Evaluate the model's performance using accuracy, precision, recall, and F1-score metrics.
Ensure the model effectively distinguishes between gluten-free and non-gluten-free products.

6. Deployment:

Deploy the trained model as a user-friendly tool where users can input product ingredient lists to determine their gluten-free status.

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
ProductName: The name of the product.
IngredientList: A text field containing the list of ingredients used in the product.
fdc_id: ID of the food in the food table.
brand_owner: Brand owner for the food.
branded_food_category: The category of the branded food, assigned by GDSN or Label Insight.
data_source: The source of the data for this food, either GDSN (GS1) or LI (Label Insight).
Is_gluten_free?: A binary target variable indicating whether the product is gluten-free (0: gluten-free, 1: non-gluten-free).
