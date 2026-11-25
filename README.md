# Email Spam Detection Using Hugging Face

## Group 29
Applied AI - Data Science and AI Final Project

## Project Overview

This project implements a pre-trained machine learning
model to distinguish spam emails from legitimate emails.

## Dataset

Source:
https://huggingface.co/datasets/diegovelilla/email-classification-dataset

- Original dataset: 10,900 emails
- Training split: 8,175 emails
- Testing split: 2,725 emails
- Cleaned analysis dataset: 2,699 emails
- Spam: 1,375
- Not spam: 1,324

## Pre-trained Model

Model:
https://huggingface.co/diegovelilla/message-classifier

- Algorithm: Multinomial Naive Bayes
- Text representation: TF-IDF
- Seven additional numerical features
- No additional training or fine-tuning

Original preprocessing source:
https://github.com/mlops-2627q1-mds-upc/MLOps-Datatouille

## Methodology

1. Dataset loading and inspection
2. Data cleaning and preprocessing
3. Exploratory data analysis
4. Pre-trained model implementation
5. Feature engineering
6. Model evaluation
7. Error analysis
8. Interactive Gradio application

## Evaluation Results

| Metric | Basic Test (6) | Extended Test (20) |
|---|---:|---:|
| Accuracy | 100% | 80% |
| Precision (spam) | 100% | 87.5% |
| Recall (spam) | 100% | 70% |
| F1-score (spam) | 100% | 77.78% |

The extended evaluation produced three false negatives
and one false positive.

## Visualizations

Six visualizations are available in results/figures:

- Class distribution
- Email length distribution
- Frequent spam words
- Frequent legitimate email words
- Basic confusion matrix
- Extended confusion matrix

## Interactive Application

A Gradio interface allows users to enter fictional
email messages and receive spam classification predictions.

## How to Run

1. Download the project notebook.
2. Open the notebook in Google Colab.
3. Install the libraries listed in requirements.txt.
4. Run the notebook cells in order.
5. Use the Gradio interface to test new emails.

An internet connection is required to download
the dataset, model and preprocessing functions.

## Limitations

- Small synthetic evaluation samples.
- Possible topic and labelling bias in the original dataset.
- Potential overlap between the dataset and training data.
- Difficulty detecting certain financial scams.
- Possible misclassification of legitimate promotional emails.
- Scikit-learn version compatibility warning.

The reported evaluation metrics apply only to the
custom examples, not the entire original dataset.

## Future Improvements

- Evaluate larger independent email datasets.
- Include more diverse email examples.
- Compare alternative classification models.

## Use of AI Tools

ChatGPT and Gemini assisted with code development,
debugging, explanations and project documentation.
The experiments were executed in Google Colab,
and the reported results were obtained from actual
model predictions.

## Conclusion

The project successfully implemented a functional
email spam detection system. Further independent
evaluation is needed to establish real-world reliability.