# Toxic-Comment-Classifier

Link for Dataset : <a href = "https://www.kaggle.com/datasets/yashs07/toxic-comment-classification" > Dataset</a>

This project aims to remove toxic comments from a social media platform using machine learning. The goal is to develop a model that can accurately identify and classify toxic comments, thereby improving the quality of interactions on the platform.

## Project Structure
Data Preprocessing: Convert text data into vectors using TextVectorization.

Pipeline: Utilize a data pipeline with the MCSHBAP method: Map, Cache, Shuffle, Batch, and Prefetch.

Model Architecture: Build a Sequential model using embedding layers, LSTM, and dense layers.

Evaluation: Measure the performance of the model using precision and recall metrics.

  


## Pipeline
The data pipeline leverages the MCSHBAP method:

Map: Apply transformations to the dataset.

Cache: Cache the data to improve performance by avoiding the recomputation of data.

Shuffle: Shuffle the dataset to ensure that the model does not learn any order dependencies.

Batch: Batch the data to allow the model to process multiple samples simultaneously.

Prefetch: Prefetch data to prevent bottlenecks by loading data while the model is training.


## Model Architecture
The model is built using the Sequential API with the following layers:

Embedding Layer: Converts input data into dense vectors of fixed size.

Bidirectional LSTM Layer: Captures information from both past and future states in the sequence.

Dense Layers: Three dense layers with ReLU activation for deep learning.

Output Layer: Uses sigmoid activation for multi-label classification.


## Evaluation Metrics
The model's performance is evaluated using precision and recall:

Precision: 0.8753308057785034
Recall: 0.8039427399635315
These metrics indicate how well the model can identify toxic comments while minimizing false positives and false negatives.

Conclusion
This project demonstrates an effective approach to identifying and removing toxic comments from a social media platform using a deep learning model. By leveraging the MCSHBAP method for pipelining and a robust neural network architecture, we achieve high precision and recall in classifying toxic comments.

References
TensorFlow documentation
Keras API documentation
