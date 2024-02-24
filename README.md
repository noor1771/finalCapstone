# Sentiment Analysis of Amazon Product Reviews

## Table of Contents
- [Project Overview](#project-overview)
- [Installation and Usage](#installation-and-usage)
- [Dataset Description](#dataset-description)
- [Methodology](#methodology)
- [Results and Evaluation](#results-and-evaluation)
- [Limitations and Further Work](#limitations-and-further-work)
- [Credits](#credits)

## Project Overview

Led by Noor Younes, this project delves into the sentiment analysis of Amazon product reviews, employing advanced Natural Language Processing (NLP) techniques to decipher the underlying sentiments expressed by customers. The project aims to parse through an extensive dataset of reviews, applying the pandas library for data handling and the TextBlob library for conducting sentiment analysis. The insights garnered from this analysis are intended to shed light on customer satisfaction levels across various products, providing valuable feedback to businesses aiming to enhance their product offerings and customer service.

## Installation and Usage

To run this project locally, follow these steps:

1. Ensure Python is installed on your machine.
2. Clone this repository or download the project files.
3. Install the required Python libraries by opening a terminal and running:

```bash
pip install pandas textblob spacy
python -m textblob.download_corpora

Dataset Description

The analysis is based on the amazon_product_reviews.csv file, a comprehensive dataset containing customer reviews for a wide array of products available on Amazon. This dataset has been crucial in providing a textual overview of customer feedback, encapsulating experiences, satisfaction levels, and varied opinions on the products purchased. Such a dataset is instrumental in extracting nuanced insights into consumer sentiment, offering a broad perspective on customer perceptions across different product categories.

Methodology

The project employs a structured approach to preprocess and analyze the textual data:

Removal of Special Characters: Utilising regular expressions to clean the review texts of all non-alphanumeric characters.
Text Normalization: Leveraging the spaCy NLP library for tokenization, followed by lemmatization to reduce words to their base form.
Stopwords and Punctuation Removal: Refining the text by excluding stopwords and punctuation to focus on the key elements that contribute to sentiment.
Sentiment Analysis: Applying the TextBlob library to each review to assign a polarity score, indicating the sentiment from -1 (negative) to +1 (positive).
Results and Evaluation

The sentiment analysis, powered by the TextBlob library, assigned polarity scores to each review, with the majority showcasing positive sentiments. This indicates a general trend of satisfaction among Amazon customers regarding their purchases. However, reviews with negative polarity scores highlighted specific areas of concern, providing valuable feedback for potential improvements.

Limitations and Further Work

While the sentiment analysis model has proven effective in categorizing sentiments of reviews, it faces limitations in detecting nuanced expressions of human emotions, such as sarcasm. Future work could explore more sophisticated models or incorporate additional linguistic features to enhance the accuracy of sentiment detection.
