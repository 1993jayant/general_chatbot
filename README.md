# general_chatbot
Basic chatbot layout which can be modified according to one's requirements.

I have created the dataset on my own. The dataset is in .json format. It is a small dataset which covers some basic intents like 'greetings', basic infomation like name and age, etc.

This is a very simple chatbot which answers some basic questions like name, age greetings, etc. which are hardcoded in the 'intents.json file'.

I created this projet to learn to build a chatbot. Its functionality can be increased by adding data into the 'intents.json' file.

I have saved the model alsong with the weights so that one doesn't need to retrain the model again and again.

The words are encoded using 'glove model' vectors for each word.

As I created the data on my own, I didn't had to do any Exloratory Data Analysis or any significant data preprocessing.

I just read the data and stored it into the variables and then trained a simple neural network. It gave me 92 percent accuracy which can be increased by using other embeddings like BoW, TFIDF, avgw2v or TFIF weighted avgw2v.

BoW was giving around 99 percent accuracy, but I didn't used it as the chatbot that I am trying to build is general purpose so it must understand the relationship between the words.

I have not tried TFIDF or Word2Vec techniques as of now.

I saved the model architecture and weights to reuse them again, thus saving time.

Finally, the input of the user is encoded firstly and then used to predict the tag/intent, if the model is not sure more than 70 percent. The output simply is a default set of sentences asking to type again.
