# NPL HOMEWORK

We used NLTK’s PorterStemmer to normalize the text — run the code to see how it does. (It may take a few seconds for the code to run.)

2. In the output terminal you’ll see our program counts "go" and "went" as different words! Also, what’s up with "mani" and "hardli"? A lemmatizer will fix this. Let’s do it.

Where lemmatizer is defined, replace None with WordNetLemmatizer().

Where we defined lemmatized, replace the empty list with a list comprehension that uses lemmatizer to lemmatize() each token in tokenized.

(Don’t know Python that well? No problem. Just check the hints for help throughout the lesson.)

lemmatized = [lemmatizer.lemmatize(token) for token in tokenized]

3. Why are the lemmatized verbs like "went" still conjugated? By default lemmatize() treats every word as a noun.

Give lemmatize a second argument: get_part_of_speech(token). This will tell our lemmatizer what part of speech the word is.

Run your code again to see the result!
