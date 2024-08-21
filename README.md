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

## Data

This project uses the IMDb movie review dataset. Due to its large size, the dataset is not included in this repository. To obtain the data:

1. Visit http://ai.stanford.edu/~amaas/data/sentiment/
2. Download the file named 'aclImdb_v1.tar.gz'
3. Extract the contents into a directory named 'aclImdb' in your project folder
4. Run the data preprocessing script (included in the notebook) to create 'movie_data.csv'

Note: The 'movie_data.csv' file created by the preprocessing script is also too large for the repository. It will be created locally when you run the preprocessing code.

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
