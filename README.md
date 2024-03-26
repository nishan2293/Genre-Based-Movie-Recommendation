# Genre Based Movie Recommendation

## Description

This project focuses on the development and application of a genre-based movie recommendation system, utilizing PySpark for sophisticated data processing and machine learning techniques. Central to our approach is the use of tokenization, stop words removal, feature transformation, vectorization, normalization, and the construction of machine learning pipelines. By processing large movie datasets, our system smartly categorizes films into genres and employs advanced algorithms to recommend movies tailored to users' preferences. This endeavor not only showcases the versatility of PySpark in handling complex data and predictive analytics but also enhances the user experience by providing personalized movie recommendations.

## Techniques Used

### Tokenization

Tokenization is the process of breaking text down into individual terms or tokens. This is a fundamental step in text analysis, allowing for further processing such as stop words removal or feature extraction.

**Implementation:**
We use PySpark's `Tokenizer` to convert input text into individual tokens, preparing the data for subsequent analysis steps.

### Stop Words Removal

Stop words are common words that are usually removed from the text before performing natural language processing. Removing these words helps in reducing the dataset size and improving the performance of the analysis.

**Implementation:**
PySpark's `StopWordsRemover` is utilized to filter out stop words from the tokenized data, enhancing the focus on more meaningful words in the dataset.

### Feature Transformation

Feature transformation involves converting textual data into a numerical format that machine learning algorithms can work with. This includes generating term frequency vectors and computing the inverse document frequency.

**HashingTF:**
The `HashingTF` function converts tokenized text into fixed-size feature vectors, effectively mapping features to indices in the feature vector.

**IDF (Inverse Document Frequency):**
The `IDF` component is used to measure how important a term is in the context of the entire dataset. It helps in weighting the features.

### Vectorization and Normalization

Vectorization is the process of turning a collection of text documents into numerical feature vectors. This is part of the feature extraction phase that converts text data into a format that is usable by machine learning algorithms.

**Normalization:**
Normalization is applied to standardize the feature vectors, ensuring that the vector values fall within a similar scale.

**Implementation:**
We use PySpark's `VectorAssembler` to combine multiple columns into a single vector column, and `Normalizer` to normalize these feature vectors.

### Machine Learning Pipelines

Machine learning pipelines are a way to codify and automate the process of data preparation, feature extraction, and model training. Pipelines help in ensuring that the data transformation and model application are performed consistently.

**Implementation:**
This project leverages PySpark's pipeline capabilities to streamline the process from data preprocessing to model training and evaluation.

## Getting Started

### Dependencies

- Apache Spark
- Python 3.x
- PySpark
- NumPy

### Output
The output displayed in the image appears to be the final result of a genre-based movie recommendation algorithm. The algorithm seems to process a given input, which is a search term for a movie genre or a keyword, and returns a list of movie titles along with their corresponding relevance scores. These scores represent the algorithm's confidence in how well each movie matches the search term based on the genre or content.
Here's how the results can be understood:

For the search term "funny movie," the algorithm has listed several movie titles along with scores that presumably represent how closely each movie aligns with the concept of a "funny movie." The higher the score, the more relevant the movie is to the search term.
The scores are likely calculated using a machine learning model that has been trained on movie data, including genres, descriptions, and possibly user ratings or reviews. The model evaluates the given search terms against this dataset to determine the relevance of each movie to the term.

The conclusion of this process is that the recommendation system is capable of understanding the context of search terms and providing a ranked list of movies that suit the user's interest in specific genres or types of movies. This output could then be used to guide users in a streaming service or movie database towards films they're more likely to enjoy based on their search preferences.
<img width="775" alt="image" src="https://github.com/nishan2293/PySparkKMeansImageCompression/assets/157925518/11645c71-8779-4dc5-9a2c-ee67678264c8">
