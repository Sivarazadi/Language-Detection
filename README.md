# Language-Detection
This code is implementing a deep learning model for text-to-language detection using the Keras library. The model is trained on a dataset consisting of text in 18 different languages, including English, Greek, Turkish, Spanish, Arabic, Dutch, Kurdish, Portugeese, Swedeish, Kannada, Danish, French, Russian, Malayalam, Tamil, Italian, German, and Hindi. The dataset is loaded into a Pandas dataframe and cleaned, then the text and language labels are shuffled and split into training and test sets.

Before being passed into the model, the text is preprocessed by removing special characters and lowercasing the letters. It is then vectorized using a CountVectorizer, which converts the text into a numerical representation that can be used for training. The language labels are encoded and transformed into categorical data using a LabelEncoder and the to_categorical function. 

The model is compiled using the Adam optimizer and categorical crossentropy loss, and is fit to the training data using the fit function.

After training, the model is evaluated on the test set using the evaluate function and achieves an accuracy of 97.9%. This model can be used to detect the language of a given piece of text with high accuracy, using both the [Language Detection dataset](https://www.kaggle.com/datasets/basilb2s/language-detection) and [4000+ Kurdish words dataset](https://www.kaggle.com/datasets/jagaryousef/4000-kurdish-words).
