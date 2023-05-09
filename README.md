# Question-Generation
## objective :
The goal of this project is to develop a question generation model that can assist in learning and education so we tried multiple models to compare between their results and get the best accuracy 
## Requirements:
nltk.tokenize
,pke
,Wikipedia-API
## Approach :
By following this pipeline belowe, I ensure that my data is cleaned and processed effectively,relevant keyphrases are extracted and questions are generated based on the keyphrases and text as this helps in structuring the information, generating meaningful questions and facilitating learning or information retrieval tasks

![Alt text](https://github.com/menna566/Question-Generation/blob/main/steps%20.png)
 
#### -keyword Extraction step
Then I used the TF-IDF model and additional models like YAKE (Another Keyword Extractor) to measure the accuracy of generated keyphrases

-TF-IDF : stands for Term Frequency-Inverse Document Frequency, which calculates the importance of a term in a document relative to a collection of documents. This model can identify important keywords or phrases based on their frequency and rarity across the document corpus.

-YAKE : is an unsupervised keyword extraction algorithm that uses statistical features and ranking functions to identify relevant keyphrases.
 
 -Then I determined the best keyphrases:
Based on the evaluation results, I compared the performance of the TF-IDF model and the YAKE model I Analyzed the accuracy scores and identify which model provides better keyphrase extraction results for your specific task and dataset.
#### -Mapping 
I mapped between keywords and the corresponding sentences in which those keywords are found with this step we provide :

Contextual Analysis: The mapping provides a way to analyze the context in which keywords appear as by examining the sentences associated with each keyword I can gain insights into how the keywords are used and the surrounding context in which they appear

Text Summarization: The mapping can be utilized as a source of information for text summarization as by selecting the most relevant sentences associated with each keyword I can generate summaries that capture the main points related to the keywords.

then I applied pipline for question generation to generate questions from the preprocessed keywords and it worked effectively :

![Alt text](https://github.com/menna566/Question-Generation/blob/main/modeeel.png)


then we tried the process again but with Wikipedia-API and it worked effectively :

![Alt text](https://github.com/menna566/Question-Generation/blob/main/moss%3B.png)

