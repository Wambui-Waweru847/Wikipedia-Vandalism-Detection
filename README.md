# Wikipedia-Vandalism-Detection
Problem Statement
Wikipedia faces constant challenges with vandalism, where users intentionally make harmful edits to articles. This project aims to develop machine learning models that can automatically detect vandalism in Wikipedia revision history data, helping to maintain the integrity and reliability of Wikipedia content.

Framework
1. Data Collection and Scraping
Develop scraping pipeline for Wikipedia revision history using Wikipedia API
Extract revision metadata (timestamps, user info, edit comments)
Collect revision content differences (added/removed text)
Implement rate limiting and ethical scraping practices
Store scraped data in structured format

2. Data Analysis and Preprocessing

Explore collected revision history dataset
Analyze dataset characteristics (vandalism cases, average word additions/removals)
Identify patterns in confirmed vandalism cases
Clean and preprocess data for model training
Split data into training (70%) and test (30%) sets

3. Feature engineering
4. CART Model Development

Build Classification and Regression Tree (CART) model using training data
Use cross-validation to select optimal complexity parameter
Generate and visualize decision tree structure
Identify and analyze most relevant variables in tree splits
Tune model parameters to improve performance

5. Random Forest Implementation

Construct random forest model with 200 trees
Set node size to 25 for tree growth control 
