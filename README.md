# Movie-Recommendation-System

There are 3 types of recommendation system.

1. Content Based Recommendation System : recommends based on the content of the movie user watched.
2. Popularity Based Recommendation System : recommends based on popularity on the particular platform user is using.
3. Collaborative Recommendation System : recommends based on user's behavioiur and watching pattern.

### In this project, I have incorporated **"Content based and popularity based recommendation system"**

Workflow of the system:

1. Data Collection
2. Data Pre-processing
3. Feature Extraction
4. User Input
5. Cosine Similarity Algorithm
6. Recommending list of Movies**

Environment and Tools used:

1. Language : **Python**
2. Libraries : Pandas, Scikit learn, difflib
3. Functions : Tfidf Vectorizer, Cosine Similarity

### **Cosine Similarity**

Cosine similarity is a metric used to measure the similarity between two vectors in a multi-dimensional space.

In sklear librarity, Cosine Similarity is often used to compare the similarity between documents represented as " vectors " in a high dimensional space.

It is particularly useful in **NLP ( Natural language processing ) tasks** such as **Text Classification** , **Information Retrieval**, and **Clustering**.

### How Cosine Similarity Algorithm Works ? 

 1. Vector Representation: Each document is represented as a vector in a high dimensional space. Each dimension of the vectpr corresponds to a feature / attribute of the document.

 2. Normalization: Before computing the cosine similarity, the vectors are normalized to unit length. This step is essential because cosine similarity is invariant to the scale of vectors.

 3. Cosine Similarity Calculation: Once vectors are normalized, the Cosine similarity between the vectors is calculated using the formula

              Cosine Similarity ( A, B ) = A . B / ||A|| ||B||

    where
    > A & B are two vectors being compared
    
    > A . B represents the dot product of vectors A & B
    
    > ||A|| & ||B|| represents Euclidean norms of vectors A & B

Interpretation :

      The Cosine Similarity ranges from -1 to 1, where ;
    
    > 1 indicates, the vectors are perfectly similar and point in same direction.
    
    > -1 indicates, the vectors are exactly opposite in direction.
    
    > 0 indicates, the vectors are perpendicular to each other, meaning they have no similarity.


The function to use Cosine Similarity,

          from sklearn.metrics.pairwise import cosine_similarity

This function takes the vectors as inp;it and returns a similarity matrix where each elements represents the cosine similarity betwenn the corresponding pair of vectors. 

