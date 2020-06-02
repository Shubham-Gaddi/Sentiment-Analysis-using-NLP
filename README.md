# Sentiment-Analysis-using-NLP
The algorithm uses an NLP model called the Bag of Words to train on reviews and classify them as good or bad. Approximately 10k reviews were used for training the model. The python libraries used include numpy,pandas and nltk(Natural Language ToolKit).
The process starts by cleaning the texts and converting it entirely to lowercase, change words to the same tense (Love = Loved) and group similar words together. Post cleaning all characters apart from alphabets are replaced by blank spaces to make sure that spepcial symbols do not cause any unexpected anomalies in the algorithm. Stemming is done and then all the reviews are split into distinct words and all stopwords are removed using nltk. Whatever is remaining after cleaning the texts is joined to form one string. Once cleaning is done , the model creates a bag od words model - each review is kept in a rwo and is represented by the frequency of all the words used. The number of columns becomes the total number of distinct words left after cleaning and the number of rows become equal to the number of datapopints. 
Finally we use Naive Bayes to classify the testing set and plot results. The dataset is available in the repository to use along with the code. 
