## Movie Recommendation

Whenever I logon to my Netflix profile, I always see the right recommendations. I am mostly into sitcoms and comedy movies. Most of those recommendations are appropriate
for me. Let's try the same by using a small dataset and few libraries in python.
Dataset I am using is [here](https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view?pli=1)
Data is mostly clean.
Steps followed.
1. Load the dataset into a pandas dataframe.
2. Select few features which you think will help in better prediction and fill the na data with '' or any word of your choice.
3. Combine all the features to contruct a string and convert into a numeric value using TfidfVectorizer.\
   What is TfidfVectorizer?\
   TFIDF = TF*IDF \
   Term frequency = no. of times term repeated /total no. of terms\
   IDF Inverse document frequency = log(N/n) - N-Number of documents, n-number of documents term appeared in document
    )
4. Identifying the similarity between the records by using cosine similarity library.\
   What is Cosine similarity?\
   It is a measure of similarity between two non-zero vectors of an inner product space based on the cosine of the angle between them, resulting in a value between -1 and 1. The value -1 means that the vectors are opposite, 0 represents orthogonal vectors, and value 1 signifies similar vectors.\
   ![image](https://github.com/user-attachments/assets/6cc02736-fe01-4fe4-b594-70ead3e1e27a)

   
   
5. Creating an array of all the movie titles (when we combined and converted the features, we have the same index but unreadble data so we want to show the user readable title recommendation).
6. Take an input from the User on the movie they want to watch.
7. Using difflab python library, we can find the close match to the user's request.
8. By sorting the similarity score in descending order and matching with index number, we can display the titles of the movie recommendations.
9. When I entered Iron Man as my input, I see all the related super movies as the recommendations. Cool!\
    ![image](https://github.com/user-attachments/assets/c4b9a8d0-6cc8-4d24-8d89-ade6aa6c6cc8)
10. Let's try again with another input. Wow! i got the recommendations correctly. 
     ![image](https://github.com/user-attachments/assets/7d2b0646-ba3f-4520-9f70-2fa80fbaa773)

Happy ML!

References:
https://memgraph.com/blog/cosine-similarity-python-scikit-learn
https://www.youtube.com/watch?v=7rEagFH9tQg

