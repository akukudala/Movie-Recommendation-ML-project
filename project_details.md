## Movie Recommendation

Whenever I logon to my Netflix profile, I always see the right recommendations. I am mostly into sitcoms and comedy movies. Most of those recommendations are appropriate
for me. Let's try the same by using a small dataset and few libraries in python.
Dataset I am using is [here](https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view?pli=1)
Data is mostly clean.
Steps followed.
1. Load the dataset into a pandas dataframe.
2. Select few features which you think will help in better prediction and fill the na data with '' or any word of your choice.
3. Combine all the features to contruct a string and convert into a numeric value using TfidfVectorizer
4. Identifying the similarity by using cosine similarity library.
5. Creating an array of all the movie titles (when we combined and converted the features, we have the same index but unreadble data so we want to show the user readable title recommendation)
6.  

