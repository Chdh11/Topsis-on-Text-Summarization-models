# Project: Text Summarization Model Evaluation

## Overview
This project aims to evaluate the performance of various pre-trained text summarization models available on Hugging Face. The models under consideration are:

1. **facebook/bart-large-cnn**
2. **philschmid/bart-large-cnn-samsum**
3. **sshleifer/distilbart-cnn-12-6**
4. **google/pegasus-large**
5. **google/pegasus-cnn_dailymail**

## Steps:

### 1. Library and Model Setup
- Import necessary libraries for text processing, model loading, and evaluation metrics.
- Load the pre-trained models from Hugging Face.

### 2. Text Summarization
- Input text snippets into the models to generate summaries for each model.

### 3. Evaluation Metrics
- Apply various metrics to assess the quality of the generated summaries.
  - BLEU Score
  - BERTScore
  - METEOR Score
  - Jaccard Similarity
  - Flesch Reading Ease Score

### 4. DataFrame Creation
- Create DataFrames for each model to store evaluation metrics for different domains.

### 5. Grouping DataFrames
- Group the DataFrames according to the domain and text to facilitate analysis.

### 6. TOPSIS Analysis
- Apply the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method to determine the best model for each domain.

## Results:

From our analysis, we can conclude the following:

| Domain      | Best Model(s)                 |
|-------------|-------------------------------|
| Politics    | facebook/bart-large-cnn, sshleifer/distilbart-cnn-12-6  |
| Medicine    | facebook/bart-large-cnn       |
| Sports      | sshleifer/distilbart-cnn-12-6 |

- **facebook/bart-large-cnn** and **sshleifer/distilbart-cnn-12-6** exhibit superior performance across different domains.

**Note:** The evaluation is based on the specified metrics and can be subject to changes in the underlying models or datasets.

Rest of the details are provided in the notebook itself.