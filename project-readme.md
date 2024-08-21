# Sentiment Analysis on Movie Reviews

This project implements sentiment analysis on movie reviews using machine learning techniques. It's based on the IMDb dataset and uses various NLP techniques such as bag-of-words, tf-idf, and Latent Dirichlet Allocation (LDA) for topic modeling.

## Setup

1. Clone this repository
2. Create a conda environment:
   ```
   conda create -n sentiment-analysis python=3.9
   conda activate sentiment-analysis
   ```
3. Install required packages:
   ```
   conda install pandas scikit-learn nltk jupyter
   pip install pyprind
   ```
4. Download NLTK data:
   ```
   python -c "import nltk; nltk.download('stopwords')"
   ```

## Usage

Open and run the Jupyter notebook `sentiment_analysis.ipynb` to see the implementation and results.

## Contents

- Data preprocessing
- Text cleaning
- Bag-of-words model creation
- Logistic regression model training
- Out-of-core learning implementation
- Topic modeling with LDA

## License

This project is open source and available under the [MIT License](LICENSE).
