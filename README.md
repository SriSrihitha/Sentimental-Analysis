Sentiment Analysis on Amazon Reviews
This project applies sentiment analysis to Amazon food reviews using two models: VADER (Valence Aware Dictionary and sEntiment Reasoner) and RoBERTa (Robustly Optimized BERT Pretraining Approach). The analysis compares the performance of these models in classifying customer reviews into positive, neutral, or negative sentiments.

Table of Contents
1.Overview
2.Project Structure
3.Requirements
4.Usage
5.Sentiment Analysis Models
6.Results and Visualizations
7.Contributing
8.License


Overview:
This project provides a detailed comparison of sentiment analysis models using the VADER sentiment analysis tool and the RoBERTa model. We analyze Amazon food reviews and visualize the results to understand how these models differ in their sentiment classification performance.

Project Structure:
bash
Copy code
.
├── Reviews.csv                 # Dataset containing Amazon food reviews
├── Internship.ipynb             # Jupyter notebook with the sentiment analysis workflow
├── README.md                    # Project documentation
├── requirements.txt             # Dependencies for the project

Requirements:
Python 3.x
Jupyter Notebook
Libraries:
pandas
numpy
matplotlib
seaborn
nltk
transformers
tqdm
scipy
Install the dependencies using:

bash
Copy code
pip install -r requirements.txt

Usage:
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/sentiment-analysis-amazon-reviews.git
Open the Jupyter notebook Internship.ipynb and run the cells to execute the code.
The notebook includes sections for:
Preprocessing Amazon food reviews
Applying VADER sentiment analysis
Applying RoBERTa model for sentiment analysis
Visualizing the results

Sentiment Analysis Models:
VADER: A rule-based model for general sentiment analysis that works well with social media text.

The SentimentIntensityAnalyzer is used to analyze the polarity of the reviews, outputting negative, neutral, positive, and compound sentiment scores.
RoBERTa: A transformer-based model fine-tuned on Twitter sentiment analysis (cardiffnlp/twitter-roberta-base-sentiment).

RoBERTa analyzes the sentiment of the reviews and provides probabilities for negative, neutral, and positive sentiments.

Results and Visualizations:
The notebook includes visualizations comparing sentiment scores from both VADER and RoBERTa models:

Bar charts show the distribution of sentiment scores based on review star ratings.
Pair plots display correlations between sentiment scores (negative, neutral, positive) from both models.
Review examples with the highest and lowest sentiment scores are shown for both models.
Example of visualizations:

Review Star Ratings vs Sentiment Scores: 
Comparison of how the sentiment models classify reviews with 1 to 5-star ratings.
Detailed Review Comparisons: Examples of reviews with extreme sentiments.
