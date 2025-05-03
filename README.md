##Problem Statement
Wikipedia, as one of the largest collaborative knowledge platforms, constantly faces malicious edits that compromise content integrity and quality. This project aims to develop a machine learning system that can automaticall detect and flag vandalism in article revisions.By analyzing patterns in user behavior, edit history, and content changes, we seek to distinguish between vandalism and malicious edits with high accuracy.The solution will leverage both random forest and CART decision trees model to identify the most predictive features of vandalism. Ultimately, this tool will help Wikipedia moderators efficiently manage the vast number of daily edits, manage reliability of information and reduce response time to vandalism.

### High level steps

1.Webscrap the data using Wikipedia API
2.Explore data characteristics: vandalism cases, average word additions/removals
3.Split data into training (70%) and test (30%) sets
4.Build CART model using training data to predict vandalism
5.Use cross validation to select the optimal cp parameter
6.Plot CART tree and identify relevant variables
7.Evaluate model accuracy on test set.
8.Build random forest model with 200 trees and node size 25 
9.Evaluate random forest model accuracy on test set
