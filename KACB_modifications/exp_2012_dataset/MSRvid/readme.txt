Five different types of experiments have been conducted for modifications in knowledge based
and corpus techniques, the abbreviations and interpretation of them are as follows:

Eexperiment_name                Description

1) jc                           It contains results for the changes made in WordNet-Augmented Word Overlap,
                                where pathlen similarity is replaced by JC similarity keeping rest of the techniques
                                same.

2) lin                          It contains results for the changes made in WordNet-Augmented Word Overlap,
                                where pathlen similarity is replaced by JC similarity keeping rest of the techniques
                                same.

3) jc_lin                       It contains results for the changes made in WordNet-Augmented Word Over-
                                lap, where pathlen similarity is replaced by Lin similarity in one feature and by
                                JC similarity in another, keeping rest of features same.

4) ww wwv                       It contains results for the changes made in Vector Space Sentence Similarity,
                                where LSA vectors are replaced by Word2Vec vectors and also an additional
                                feature is used where LSA vectors is replaced by weighted Word2Vec vectors, rest all the features 
				are the same.

5) jc lin wv wwv                In this technique all the proposed changes are merged together
                                keeping rest of the features same.


So, all these experiments with their corresponding scores can be found in the python code "msr_par.ipynb" which is taking
MSRpar dataset as input for sentence pairs. This code can only run on Jupyter Notebook and works fast on CPU of RAM more than 4GB, otherwise it may take more than one hour to run . You can run this code on Google Colab Notebook as well,as it provides a GPU and a CPU of RAM upto 25GB,
which is sufficient for these codes run.

**NOTE ON PREREQUISITES**
You need to download 5 text files in order to run the code in this folder. The name of the text files and their corresponding link is given 
below:

nyt_words.txt: 			https://drive.google.com/file/d/1lJFcCUHAD6bQ6vWL_WMv7U9yGq3-bnlk/view?usp=sharing
nyt_word_vectors.txt: 		https://drive.google.com/file/d/11TT2i3WGjrEZ6QJl1uxZTnIuk0K1IcV0/view?usp=sharing
wikipedia_words.txt:		https://drive.google.com/file/d/1M0hYI4N2v6DyBgHo-M9Te0dq9jhqCa3J/view?usp=sharing
wikipedia_word_vectors.txt:	https://drive.google.com/file/d/1uaizff-Nuv-WyUDt3kGJp6_kiDdFloLT/view?usp=sharing
word-frequencies.txt:		https://drive.google.com/file/d/1ddfI7Hob4eZZ3pWxCyw0JY_H440ywfWH/view?usp=sharing


Details on other files and folder:
-----------------------------------
"nyt_words.txt" containts all the words from the New York Times dataset. Which are required to calculate LSA word vectors.

"nyt_word_vectors" contains vector representation of all the words present in nyt_words.txt.

"wikipedia_words.txt" containts all the words from the WikiPedia dataset. Which are required to calculate LSA word vectors.

"wikipedia_words_vectors" contains vector representation of all the words present in wikipedia_words.txt.

Output folder contains all the text file given as output from each experiment, which is further taken as input into the
code to calculate Pearon Correlation.
