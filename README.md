# Kovida-Samir-Kshatri_Hack-to-Hire
Indigo Hack to Hire - Data Science(4010)


The problem statement presented requires us to build a question answering system, specifically a closed book question answering system i.e., it does not use any context and answers based on the universal knowledge of the subject. 

The code shows the initial preprocessing of the data set by removing duplicate rows. Further cleaning could not take place due to the nature of text data. Further text preprocessing like lowercasing, stopword removal, stemming and lemmatization have been performed.

Next the dataframe is converted into a huggingface dataset and further tokenized(All these steps are performed on both the train and test sets - 80:20; shuffled). 
This tokenized data is then sampled due to GPU constraints into a smaller dataset.

I have employed BERT, T5 and GPT language models. These models were used to generate predictions. These models could not be entirely trained due to GPU constraints but the pre-trained model of T5 and GPT were used to generate predictions and references based on the test set.
Further some visualizations have been made of what could be processed using the computational capacity available to me.

**Novelty/Additions to the work**:
Keeping aside GPU constraints, Named Entity Recognition(NER) should be used since we lack context. Also, the data set must be annotated to gather context so as to further apply techniques like word embeddings and cosine similarity.

****There is a major need of GPU.**
