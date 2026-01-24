# Instance-Based vs Model-Based Learning

Machine Learning algorithms can be broadly categorized into **Instance-Based Learning**
and **Model-Based Learning** based on how they learn from data and make predictions.



## Model-Based Learning

In model-based learning, we first **train a model** that learns patterns or parameters from the data.

### Key Characteristics
- Data is cleaned, preprocessed, and analyzed (EDA) before training.
- A mathematical or statistical model is trained using the prepared data.
- The trained model stores learned parameters or rules.
- After training, the original training data is **not required** for prediction.
- Predictions are made using the trained model, not the raw data.

### Storage
- Requires storing only the trained model.
- Lower storage requirement compared to instance-based learning.

### Examples
- Linear Regression
- Logistic Regression
- Decision Trees
- Neural Networks



## Instance-Based Learning

Instance-based learning does **not explicitly train a model**.  
Instead, it stores the training data and makes predictions by comparing new queries to existing instances.

### Key Characteristics
- Data preprocessing and cleaning are still required.
- No separate training phase to build a model.
- Predictions are made at **query time** using similarity measures.
- No prior generalization is performed.
- The entire (or partial) training dataset is used during prediction.

### Storage
- Requires storing the full training dataset.
- Higher storage requirement compared to model-based learning.

### Examples
- K-Nearest Neighbors (KNN)
- Case-Based Reasoning Systems




## Key Takeaway

> Model-based learning generalizes **before prediction**,  
> Instance-based learning generalizes **during prediction**.
