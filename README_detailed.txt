README.txt

Title: Integrating Eco-Translatology with Artificial Intelligence:
Enhancing Cultural Adaptation in Multilingual Educational Content
Translation

Description: This project develops a multilingual sentiment analysis
system using Artificial Intelligence to enhance cultural adaptation in
translation, aligned with Eco-Translatology principles. The framework
leverages a pretrained multilingual BERT model to classify sentiment
across English, Spanish, French, and German datasets. The goal is to
capture linguistic and emotional nuances that improve the quality of
multilingual educational content translation.

Dataset Information: - Dataset: Amazon Reviews Dataset - Files Used:
train.csv test.csv validation.csv

-   Original Dataset Size: Training: ~1.2 million samples Testing:
    ~30,000 samples Validation: ~30,000 samples

-   Filtered Languages: English (en) Spanish (es) French (fr) German
    (de)

-   Final Subset: Total: 84,000 samples Training: 70% Validation: 20%
    Testing: 10%

-   Features: review_body: textual review stars: rating (1–5) polarity:
    0 = Negative (1–2 stars) 1 = Neutral (3 stars) 2 = Positive (4–5
    stars)

Code Information: The code is implemented in Python and includes the
following steps:

1.  Data Loading: Reads CSV files from Google Drive.

2.  Data Exploration: Displays dataset sizes and distributions.

3.  Preprocessing: Filters selected languages. Converts star ratings to
    sentiment polarity.

4.  Stratified Sampling: Maintains class distribution while reducing
    dataset size.

5.  Visualization: Generates sentiment and rating distribution plots.

6.  Dataset Conversion: Converts data into Hugging Face Dataset format.

7.  Tokenization: Uses multilingual BERT tokenizer with padding and
    truncation.

8.  Model: Pretrained model:
    nlptown/bert-base-multilingual-uncased-sentiment Configured for
    3-class classification.

9.  Training: Uses Hugging Face Trainer API. Includes early stopping.

10. Evaluation: Accuracy, Precision, Recall, F1-score. Confusion
    matrices. ROC-AUC curves.

Usage Instructions: Step 1: Open Google Colab Step 2: Mount Google Drive
Step 3: Upload dataset to: /content/drive/MyDrive/amazonreview/ Step 4:
Install required libraries: pip install transformers datasets
imbalanced-learn seaborn plotly nltk Step 5: Run all code cells
sequentially Step 6: Analyze outputs and evaluation metrics

Requirements: - Python 3.x

Libraries: - pandas - numpy - matplotlib - seaborn - nltk -
scikit-learn - transformers - datasets - imbalanced-learn - plotly -
tqdm - wordcloud

Methodology: 1. Filter multilingual data (en, es, fr, de) 2. Convert
ratings to sentiment polarity 3. Apply stratified sampling to maintain
balance 4. Preprocess and map text-label pairs 5. Tokenize using BERT
tokenizer 6. Train multilingual BERT model 7. Evaluate using multiple
performance metrics 8. Interpret results for cultural adaptation
insights

License: This project is for academic and research purposes. Reuse is
allowed with proper citation.

Contribution Guidelines: - Improve preprocessing - Extend to more
languages - Enhance model performance - Add explainable AI techniques
(SHAP, LIME)

Steps: 1. Fork the project 2. Create a new branch 3. Submit a pull
request
