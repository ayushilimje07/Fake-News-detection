# Fake-News-detection
1. Data Preprocessing with NLP: The preprocessing phase involves cleaning and transforming the raw news articles into a suitable format for feature extraction and model training. This includes:
   o Tokenization: Splitting the text into individual words or tokens.
   o Stopword Removal: Filtering out common words that do not contribute significantly to the meaning of the text (e.g., 'the', 'is', 'and'). o Stemming and Lemmatization: Reducing words to their root forms, helping to standardize the dataset and reduce vocabulary size.
   o Vectorization: Utilizing FastText embeddings to represent words in a dense, semantic vector space, capturing both word meaning and context.
2. Feature Extraction with FastText: FastText is employed for feature extraction, as it provides rich word embeddings that consider subword information, improving the system's ability to generalize across different languages and misspelled words. FastText captures the relationships between words and their surrounding context, generating embeddings that serve as input to the CNN classifier.
3. Fake News Classification with CNN: The extracted FastText embeddings are fed into a Convolutional Neural Network (CNN), which is responsible for learning spatial patterns in the text data. The CNN architecture consists of:
   o Convolutional Layers: These layers detect relevant features and patterns in the text embeddings. o Pooling Layers: These layers reduce the dimensionality of the features, focusing on the most important patterns.
   o Fully Connected Layers: These layers classify the news articles as 'real' or 'fake' based on the extracted features.
