# Darija Sentiment Analysis with DarijaBERT

This project performs sentiment analysis on Darija (Moroccan Arabic) text using the DarijaBERT model. It takes input from an Excel file containing tweets and an Excel file containing dialect information. The sentiment analysis is performed on each tweet, and the results are saved to a new Excel file.

## Overview

The code provided in this repository includes:

- Loading tweets and dialect information from Excel files.
- Tokenizing the tweets for dialect analysis and sentiment analysis using the DarijaBERT tokenizer.
- Running the DarijaBERT model for dialect analysis.
- Running the DarijaBERT model for sentiment analysis.
- Classifying the sentiment of each tweet (e.g., Positive or Negative).
- Saving the sentiment analysis results to a new Excel file.

## Getting Started

Before running the code, make sure to set up your environment and specify the paths to your Excel files containing tweets and dialect information:

```python
# Usage example
tweet_file = '/content/drive/MyDrive/Sentiment Analysis/ElecMorocco2016 (1).xlsx'
dialect_file = '/content/drive/MyDrive/Sentiment Analysis/MOROCCODialect Stop-Words.xlsx'

perform_sentiment_analysis(tweet_file, dialect_file)
```

Ensure that you have the required libraries installed:

```bash
!pip install transformers
```

## DarijaBERT Model

The code loads the DarijaBERT tokenizer and model for both dialect and sentiment analysis. These models are designed for processing Darija (Moroccan Arabic) text.

## Sentiment Analysis

The sentiment analysis process involves:

1. Tokenizing each tweet for dialect and sentiment analysis.
2. Passing the input through the DarijaBERT models for dialect and sentiment analysis.
3. Classifying the sentiment of each tweet, for example, as Positive or Negative.

You can further customize the sentiment analysis process or extract additional information from the model outputs as needed.

## Saving Results

The sentiment analysis results, including the original tweet, dialect information, and sentiment classification, are saved to a new Excel file:

```python
results_df.to_excel('/content/drive/MyDrive/Sentiment Analysis/sentiment_analysis_results.xlsx', index=False)
```

Please adjust the paths and customize the code according to your specific dataset and requirements. For any questions or issues, please don't hesitate to reach out.

**Note**: Ensure that your dataset files are correctly formatted in Excel and that you have access to the required models and libraries before running the code.
