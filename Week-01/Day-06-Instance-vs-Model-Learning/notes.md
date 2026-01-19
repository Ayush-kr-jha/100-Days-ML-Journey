# Model (Conventional) Based Learning

1. We need to prepare the data for model training, i.e., data cleaning, data preprocessing, EDA, etc.
2. Train a model using the prepared data to estimate model parameters or discover patterns.
3. Store the trained model.
4. Use the learned parameters to generalize and predict new, unseen queries (data).
5. After learning the model parameters or rules for prediction, the training data is no longer required.
6. Storing the trained model requires less storage.

# Instance-Based Learning

1. We need to prepare the data, i.e., data cleaning, data preprocessing, EDA, etc.
2. We do not explicitly train a model; instead, predictions are made by comparing a query with stored instances.
3. There is no trained model to store.
4. No generalization is performed in advance; decisions are made at query time based on similarity to training data.
5. The training data must be stored since each query uses part or all of the training observations.
6. Storing the training data requires more storage capacity.
