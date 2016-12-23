# Spam-Classifier
This Python Program, built using the Jupyter Notebook, is used to classify whether a specific E-mail is either a Spam, or a Ham(Non-Spam).

It is implemented using the [Naive Bayes Algorithm](https://en.wikipedia.org/wiki/Naive_Bayes_classifier).

####Dataset Description
The Training and Testing Mails have been downloaded from [here](http://openclassroom.stanford.edu/MainFolder/DocumentPage.php?course=MachineLearning&doc=exercises/ex6/ex6.html).
The dataset is split into two subsets: a 700-email subset for training and a 260-email subset for testing.
Each of the training and testing subsets contain 50% spam messages and 50% nonspam messages.
Additionally, the emails have been preprocessed in the following ways:

1. Stop word removal: Certain words like "and," "the," and "of," are very common in all English sentences and are not very meaningful in deciding spam/nonspam status, so these words have been removed from the emails.
2. Lemmatization: Words that have the same meaning but different endings have been adjusted so that they all have the same form. For example, "include", "includes," and "included," would all be represented as "include." All words in the email body have also been converted to lower case.
3. Removal of non-words: Numbers and punctuation have both been removed. All white spaces (tabs, newlines, spaces) have all been trimmed to a single space character.

####Using Inbuilt Naive Bayes Library
MultinomialNB() is an inbuilt library found in the sklearn package used for the purpose of implementing Naive Bayes.

After training the model, the predictions made on the testing mails are 97.69% accurate.

####Using Self-built Naive Bayes Library
Here, I implemented the Naive Bayes Algorithm on my own, using basic mathematics. It was made for learning purposes.

After training the model, the predictions made on the testing mails are 92.30% accurate. Although the self built model is slower and less accurate than the inbuilt one, it helped in the strengthening of concepts.
