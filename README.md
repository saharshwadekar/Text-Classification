# Text Classification with Naive Bayes

This repository contains a Python implementation of a text classification system using Naive Bayes. The system is trained on a dataset from the BBC, classifying news articles into categories such as business, entertainment, politics, sport, and tech.

## Project Structure

The project is organized as follows:

- `data/`: Contains the dataset used for training and testing.
- `models/`: Stores the trained Naive Bayes classifier and vectorizer.
- `src/`: Contains the source code for data preprocessing, model training, and deployment.

## Setup

1. Clone the repository:

   ```
   git clone https://github.com/your-username/text-classification-naive-bayes.git
   cd text-classification-naive-bayes
   ```

2. Install the required dependencies:

   ```
   pip install -r requirements.txt
   ```

## Data Preparation

The dataset is prepared using the create_data_set function, and documents are set up using the setup_docs function. The most frequent words for each category are printed using the print_frequent_dist function.

## Model Training

The Naive Bayes classifier is trained using the train_classifier function. The data is split into training and testing sets, vectorized using CountVectorizer, and then used to train the classifier.

## Deployment

To use the trained classifier for new data, the classify function is provided. Simply load the saved classifier and vectorizer and use them to predict the category of new text.

```
# Example Usage
new_data = "Your text here"
classify(new_data)
```

## Files

### naive_bayes_classifier.pkl:
  Pickled file containing the trained Naive Bayes classifier.
### count_vectorizer.pkl: 
  Pickled file containing the CountVectorizer used for vectorization.

## Acknowledgments
The dataset used in this project is sourced from the BBC and covers various news categories.
Feel free to explore, contribute, and use this repository for your text classification tasks!


