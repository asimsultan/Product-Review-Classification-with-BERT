
# Product Review Classification with BERT

Welcome to the Product Review Classification with BERT project! This project focuses on classifying product reviews using the BERT model.

## Introduction

Product review classification involves categorizing reviews as positive or negative based on their content. In this project, we leverage the power of BERT to perform product review classification using a dataset of labeled reviews.

## Dataset

For this project, we will use a custom dataset of product reviews. You can create your own dataset and place it in the `data/review_data.csv` file.

## Project Overview

### Prerequisites

- Python 3.6 or higher
- PyTorch
- Hugging Face Transformers
- Datasets
- Pandas

### Installation

To set up the project, follow these steps:

```bash
# Clone this repository and navigate to the project directory:
git clone https://github.com/your-username/bert_product_review_classification.git
cd bert_product_review_classification

# Install the required packages:
pip install -r requirements.txt

# Ensure your data includes product reviews and their labels. Place these files in the data/ directory.
# The data should be in a CSV file with two columns: text and label.

# To fine-tune the BERT model for product review classification, run the following command:
python scripts/train.py --data_path data/review_data.csv

# To evaluate the performance of the fine-tuned model, run:
python scripts/evaluate.py --model_path models/ --data_path data/review_data.csv
