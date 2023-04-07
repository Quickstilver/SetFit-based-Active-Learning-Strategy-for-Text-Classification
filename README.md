# SetFit-based Active Learning Strategy for Text Classification

This project presents a novel active learning strategy for text classification tasks, which combines the selection of unique examples and instances for which the model is uncertain. The strategy calculates prediction entropy on already labeled data to identify examples where the model is most uncertain and then uses prediction entropy again as a strategy for the unlabeled pool. The model is updated with query results from the unlabeled pool and the example in which the model was most uncertain. SetFit is used as the underlying model for this strategy.


## Project Highlights:

- Designs an active learning strategy that selects novel examples and instances where the model is uncertain.
- Utilizes SetFit with Sentence Transformers for text classification.
- Employs the small-text and datasets libraries for dataset handling and model creation.
- Implements an active learning loop with a query strategy based on Prediction Entropy and Breaking Ties.
- Displays the results in terms of train and test accuracy for each iteration of the active learning process.

## Key Components:

### Dataset:

- Toxic Conversations 50k

### Libraries and Dependencies:

- small-text[transformers]==1.3.0
- setfit>=0.5.0
- datasets
- matplotlib

## Main Steps:
- Load and preprocess the dataset.
- Create a balanced initial labeled set for active learning.
- Create SetFit classifiers using the small_text library.
- Implement an active learning loop with a query strategy based on Prediction Entropy and Breaking Ties.
- Evaluate and store the train and test accuracy for each iteration.

## Conclusions:
This project showcases a unique active learning strategy for text classification tasks, combining the selection of novel examples and instances where the model is uncertain. The results can be used to inform future improvements in active learning techniques and text classification approaches.
