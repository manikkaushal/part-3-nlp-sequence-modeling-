# Part 3 - NLP and Sequence Modeling

This is my submission for part 3 of the AI project. The goal here is to work with text data and understand how NLP pipelines work.

## What I did

I used the customer support text classification dataset. The dataset has customer messages and each message is labeled as positive, neutral, or negative.

I split the work into 6 tasks:

- Task 1: Looked at the dataset to understand what's in it
- Task 2: Cleaned the text by removing special characters, lowercasing etc
- Task 3: Converted text to numbers using TF-IDF
- Task 4: Built a logistic regression model as the baseline
- Task 5: Designed an LSTM architecture (did not fully train it due to compute constraints)
- Task 6: Wrote a short reflection on RNNs, LSTMs, Attention and Transformers

## Dataset

File used: `customer_support_text_classification.csv`

It has 1500 rows. The main columns I used are:
- `customer_message` - the actual text
- `sentiment_label` - the target (positive, neutral, negative)

## How to run

First install the required packages:

```
pip install -r requirements.txt
```

Then open the notebook:

```
jupyter notebook notebook.ipynb
```

Run all cells from top to bottom.

## Results

The results are saved in the `results/` folder:
- `model_evaluation.png` - confusion matrix and class distribution chart
- `model_evaluation.csv` - precision, recall, f1 scores for each class
- `sample_predictions.txt` - a few example predictions from the model

## Note

The accuracy came out really high (close to 1.0). I think this might be because the dataset is synthetic and the patterns are very clean. In a real world dataset the numbers would probably be lower.

## Folder structure

```
part-3-nlp-sequence-modeling/
│
├── README.md
├── notebook.ipynb
├── requirements.txt
└── results/
    ├── model_evaluation.png
    ├── model_evaluation.csv
    └── sample_predictions.txt
```
