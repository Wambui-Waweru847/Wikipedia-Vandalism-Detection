## Problem Statement
Wikipedia, as one of the largest collaborative knowledge platforms, constantly faces malicious edits that compromise content integrity and quality. This project aims to develop a machine learning system that can automaticall detect and flag vandalism in article revisions.By analyzing patterns in user behavior, edit history, and content changes, we seek to distinguish between vandalism and malicious edits with high accuracy.The solution will leverage both random forest and CART decision trees model to identify the most predictive features of vandalism. Ultimately, this tool will help Wikipedia moderators efficiently manage the vast number of daily edits, manage reliability of information and reduce response time to vandalism.

### High level steps

- Webscrap the data using Wikipedia API
- Explore data characteristics: vandalism cases, average word additions/removals
- Split data into training (70%) and test (30%) sets
- Build CART model using training data to predict vandalism
- Use cross validation to select the optimal cp parameter
- Plot CART tree and identify relevant variables
- Evaluate model accuracy on test set.
- Build random forest model with 200 trees and node size 25 
- Evaluate random forest model accuracy on test set

## Communication of insights
- The total number of revisions : 1067
- The total number of vandalism cases: 104
- Vandalism rate: 10 %
- The total number of significant changes (above 1000 characters): 26
- The percentage of significant changes : 2.44%
- The total number of revert mentions: 55
- The percentage of revert mention : 5.15%
- The total number of vandalism mentions: 5
- The model attained a baseline score of 90%
- The model itself attained a score of 100%, probably because of the small nature of the sample size
- Only two features - diff_size and contains_vandalism - were important in classifying the revisions as either harmful or harmless.
- Vandalism detection system can be used as a monitoring system to identify coordinated vandalism attack

## Recommendations
Future work could enhance the work through:
  - Incorporating natural language processing for deeper analysis
  - Creating specialized detectors for different vandalism types
