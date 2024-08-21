# IMDB Sentiment Analysis

This project implements sentiment analysis on IMDB movie reviews using various machine learning techniques, including traditional methods and advanced approaches like topic modeling and out-of-core learning.

## Project Overview

We analyze a large dataset of IMDB movie reviews to:
1. Classify reviews as positive or negative (sentiment analysis)
2. Identify underlying topics in the reviews (topic modeling)
3. Demonstrate handling of large datasets (out-of-core learning)

## Techniques Used

### Sentiment Analysis
We use machine learning to classify movie reviews as positive or negative. This involves:
- Text preprocessing
- Feature extraction (bag-of-words, TF-IDF)
- Training a logistic regression model

### Topic Modeling with LDA
Latent Dirichlet Allocation (LDA) is used to discover abstract topics in the review collection:
- LDA is an unsupervised learning method
- It identifies patterns of word use and connects documents that share similar patterns
- We use it to find the main themes discussed across the reviews

Key aspects:
- Uncovers hidden thematic structure in the document collection
- Allows us to summarize, organize, and search the reviews more effectively
- Provides insights into common themes in movie reviews

### Out-of-Core Learning
To handle the large IMDB dataset efficiently, we implement out-of-core learning:
- Processes data in smaller batches that fit in memory
- Allows analysis of datasets larger than the available RAM
- Uses stochastic gradient descent for incremental model updates

Benefits:
- Scalability: Can work with very large datasets
- Memory efficiency: Doesn't require loading all data at once
- Practical for real-world, large-scale text analysis

## Setup

### Environment Setup

1. Clone this repository:
   ```
   git clone https://github.com/your-username/imdb-sentiment-analysis.git
   cd imdb-sentiment-analysis
   ```

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

### Data Acquisition

This project uses the IMDB movie review dataset. Due to its large size, the dataset is not included in this repository. To obtain the data:

1. Visit http://ai.stanford.edu/~amaas/data/sentiment/
2. Download the file named 'aclImdb_v1.tar.gz'
3. Extract the contents into a directory named 'aclImdb' in your project folder
4. Run the data preprocessing script (included in the notebook) to create 'movie_data.csv'

Note: The 'movie_data.csv' file created by the preprocessing script is also too large for the repository. It will be created locally when you run the preprocessing code.

## Usage

1. Start Jupyter Notebook:
   ```
   jupyter notebook
   ```

2. Open and run the notebooks in the following order:
   - `1_data_preprocessing.ipynb`
   - `2_sentiment_analysis.ipynb`
   - `3_topic_modeling_with_LDA.ipynb`
   - `4_out_of_core_learning.ipynb`

## File Descriptions

- `1_data_preprocessing.ipynb`: Prepares the IMDB dataset for analysis
- `2_sentiment_analysis.ipynb`: Main notebook for sentiment analysis
- `3_topic_modeling_with_LDA.ipynb`: Demonstrates LDA for topic modeling
- `4_out_of_core_learning.ipynb`: Shows out-of-core learning techniques

## Results and Insights

[Add a brief summary of your findings here once you have results]

## Contributing

Contributions to improve the analysis or extend the project are welcome. Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
