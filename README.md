# Text-Summarisation
Text Summarization using TF/IDF and TextRank Algorithm

Text Summarization is one of those applications of Natural Language Processing (NLP) which is bound to have a huge impact on our lives. With growing digital media and ever growing publishing – who has the time to go through entire articles / documents / books to decide whether they are useful or not? Thankfully – this technology is already here.

Have you come across the mobile app inshorts? It’s an innovative news app that converts news articles into a 60-word summary. This is done by Automatic Text Summarization.

Based on these classes, each comment was classified and this data set was posted online for reference. Based on this, a test dataset will be used to verify the accuracy of the model. A lot of feature engineering is used here as there are no obvious features that can be deciphered.

Automatic Text Summarization is one of the most challenging and interesting problems in the field of Natural Language Processing (NLP). It is a process of generating a concise and meaningful summary of text from multiple text resources such as books, news articles, blog posts, research papers, emails, and tweets.
The demand for automatic text summarization systems is spiking these days thanks to the availability of large amounts of textual data.

Automatic Text Summarization gained attention as early as the 1950’s. A research paper, published by Hans Peter Luhn in the late 1950s, titled “The automatic creation of literature abstracts”, used features such as word frequency and phrase frequency to extract important sentences from the text for summarization purposes.

Another important research, done by Harold P Edmundson in the late 1960’s, used methods like the presence of cue words, words used in the title appearing in the text, and the location of sentences, to extract significant sentences for text summarization. Since then, many important and exciting studies have been published to address the challenge of automatic text summarization. 


**ALGORITHMS:**

-> TF/IDF


TF-IDF algorithm is made of 2 algorithms multiplied together.

Term Frequency
Term frequency (TF) is how often a word appears in a document, divided by how many words there are.
TF(t) = (Number of times term t appears in a document) / (Total number of terms in the document)
Inverse document frequency
Term frequency is how common a word is, inverse document frequency (IDF) is how unique or rare a word is.
IDF(t) = log_e(Total number of documents / Number of documents with term t in it)
Example, 
Consider a document containing 100 words wherein the word apple appears 5 times. The term frequency (i.e., TF) for apple is then (5 / 100) = 0.05.
Now, assume we have 10 million documents and the word apple appears in one thousand of these. Then, the inverse document frequency (i.e., IDF) is calculated as log(10,000,000 / 1,000) = 4.
Thus, the TF-IDF weight is the product of these quantities: 0.05 * 4 = 0.20.



-> TextRank Algorithm


TextRank is an extractive and unsupervised text summarization technique.
 
Let’s take a look at the flow of the TextRank algorithm that we will be following:
 

![image](https://user-images.githubusercontent.com/87649285/223955339-d9935632-0df9-4724-b992-007029344e51.png)



**CONCLUSION**



We looked at two text extraction methods for text summarization. TF-IDF and TextRank Algorithm. In the td-idf method we calculate the td-idf score of an entire sentence by adding the tf-idf score of the individual words in that sentence, in this way we get the importance score for an entire sentence. In contrast to this we use a simillarity matrix in the textrank algorithm method. We get better results with the textrank algorithm method because we use glove word embeddings in it which is the best performing method to get word embeddings and also because textrank is a more complex algorithm than tf-idf.
