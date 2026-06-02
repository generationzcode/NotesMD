- For proper training, you need a proper set of features from a dataset for a model to learn from
- If the set of features provided is well composed, there is no feature engineering problem. All that is required is a domain based sanity check - don't want to classify buffaloes on the type of mayonnaise served at the burger king nearest to the object
## Dimensionality Issues
- The number of features given usually outnumber the number required to train a model
- How to pick and choose, and why?
- This is done for readability, avoiding the curse of dimensionality, reduce overfitting risk, reduce computation time
- The curse of dimensionality: When you increase the dimensions of data, the volume of the space required to train a model properly increases much faster than the amount of data you have. So for the same data, you'll have less information to train a model with when you have more dimensions. The available data becomes sparse
- One can imagine this causes a mode to "overfit" on the training data and perform badly to test data
- Feature selection is how we select relevant features. There are many methods checking the informativeness, covariance with other features, etc.
- Feature extraction is the process of deriving new features from what you already have. Eg. one hot encoding