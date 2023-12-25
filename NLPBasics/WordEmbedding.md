***NOTE:*** The content of this page is from [HERE](https://www.turing.com/kb/guide-on-word-embeddings-in-nlp)  
***
Word embedding in NLP is a technique where words or phrases from the vocabulary are mapped to vectors of real numbers.  
We have 5 solutions:
+ TF-IDF
+ Bag of Words(BOW)
+ Word2vec
+ GloVe
+ BERT

# TF-IDF: Term frequency-inverse document frequency
TF-IDF is the machine learning algorithm that is used for word embedding for text. It comprises two metrics, namely **term frequency(TF)** and **inverse document frequency(IDF)**.
This algorithm works on a statistical measure of finding word relevance in the text that can be in the form of a single document or various documents that are referred to as corpus(a collection of written or spoken texts).

## Term Frequency
The TF score measures the frequency of words in a particular document.
$$
TF_{i,j} = \frac{\text{Term i frequency in document j}}{\text{Total number of terms in document j}}
$$

## Inverse Document Frequency
The IDF score measures the rarity of the words in the text. It is given more importance over the term frequency score because even though the TF score gives more weightage to frequently occurring words, the IDF score focuses on **rarely used words** in the corpus that may hold significant information.
$$
IDF_i=log(\frac{\text{Total documents}}{\text{Number of documents containing term i}})
$$

## Combined
$$
TF-IDF_{i,j}=\frac{TF_{i,j}}{IDF_i}
$$
