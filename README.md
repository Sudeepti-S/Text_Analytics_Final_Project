# Exploratory Text Analytics Project 


The objective of this project was to produce a digital analytical edition of a corpus that will support exploration of the cultural contents of that corpus. Cultural content is broadly conceived—it may be about language use, social events, cultural categories, sentiments, identity, taste, etc. 

After acquiring a collection of texts written by Luisa May Alcott and Edgar Allen Poe from the Gutenburg Project, the following operations were performed:

1. Converted the collection from their source formats (F0) into a set of tables that conform to the Standard Text Analytic Data Model (F2) and to the Machine Learning Corpus Format (F1). 
2. Annotated these tables with statistical and linguistic features using NLP libraries such as NLTK (F3). 
3. Created a vector representation of the corpus to generate TFIDF values to add to the TOKEN and VOCAB tables (F4). 
4. Extended the annotated and vectorized model with tables and features derived from the application of various unsupervised methods, including PCA, LDA, and word2vec (F5). 
5. Explored your results using statistical and visualization methods. 
6. Presented conclusions about cultural patterns observed in the corpus by means of these operations.


The following data is also included as features in the appropriate core table or as separate tables. 

# Principal Components 
        * Table of documents and components. 
        * Table of components and word counts (i.e., the “loadings”), either added to the VOCAB table or as a separate table with a shared index with the VOCAB table. 
# Topic Models (LDA) 
        * Table of document and topic concentrations. 
        * Table of topics and term counts, either added to the VOCAB table or as a separate table with a shared index with the VOCAB table. 
# Word Embeddings (word2vec) 
        * Terms and embeddings, either added to the VOCAB table or as a separate table with a shared index with the VOCAB table. 
# Sentiment Analysis 
         * Sentiment and emotion values as features in VOCAB or as a separate table with a shared index with the VOCAB table. 
        * Sentiment polarity and emotions for each document. 
        
        
# Data Source 

Luisa May Alcott - https://www.gutenberg.org/wiki/Children%27s_Literature_(Bookshelf) 
Her texts(a collection of 8 books) were derived from the children's literature bookshelf.


Edgar Allen Poe - https://www.gutenberg.org/wiki/Horror_(Bookshelf)#Edgar_Allan_Poe.2C_1809-1849
His works (5 volumes of short stories) were derived from the horror bookshelf.
Of these volumes, only short stories written by Poe were included in the corpus. His poems, novel and biography were left out.


# Description: What is the general subject matter of the corpus?

The literary genre of the corpus is children literature. Luisa May Alcott wrote stories regarding family life, sisterhood, family dynamics, and being a women in the nineteenth century. Through her works, she explored themes associated with family dynamics, marriage, housewives, and love to name a few. Edgar Allen Poe, on the other hand, explores themes associated with death, love, ephemerality. 

Format: A description of both the file formats of the source files, e.g., plaintext, XML, CSV, etc., and the internal structure where applicable. For example, if XML then specify document type (e.g., TEI or XHTML).

All the file formats of the source files were plaintext files (.txt). 
The OHCO model chosen for Poe's short stories was volumes, stories, paragraphs, sentences and tokens, while the OHCO for Alcott's books was books, chapters, paragraphs, sentences and tokens. When combined for our our entire corpus, we use the generic OHCO levels where volumes are treated as books and short stories are treated as chapters.
