The following folders contain codes corresponding to the various experiments implemented by the proposed architecture,
i.e., by combining 6 experiments of KACB methods with 6 experiments of CNN architecure.

FOLDER                      DESCRIPTION

1) fasttext_coef            Folder contains KACB_fasttext_coef.ipynb code which combines the 5 KACB experiments with
                            CNN architecture which uses fasttext as word embeddings for the representation of the words
                            and Pearson Correlation Coefficient as loss function.

2) fasttext_kl              Folder contains KACB_fasttext_kl.ipynb code which combines the 5 KACB experiments with
                            CNN architecture which uses fasttext as word embeddings for the representation of the words
                            and KL-Divergence as the loss function.

3) word2vec_coef            Folder contains KACB_word2vec_coef.ipynb code which combines the 5 KACB experiments with
                            CNN architecture which uses word2vec as word embeddings for the representation of the words
                            and Pearson Correlation Coefficient as the loss function.

4) word2vec_kl              Folder contains KACB_word2vec_kl.ipynb code which combines the 5 KACB experiments with
                            CNN architecture which uses word2vec as word embeddings for the representation of the words
                            and KL-Divergence as the loss function.

5) glove_kl                 Folder contains KACB_glove_kl.ipynb code which combines the 5 KACB experiments with
                            CNN architecture which uses glove as word embeddings for the representation of the words
                            and KL-Divergence as the loss function.

6) 2017_takelab+cnn         Folder contains KACB_glove_coef.ipynb code which combines the 5 KACB experiments with
                            CNN architecture which uses glove as word embeddings for the representation of the words
                            and KL-Divergence Pearson Correlation Coefficient as the loss function.

			    ***NOTE***

			    The code KACB_glove_coef.ipynb takes the best saved model parameters provided by the CNN which
		            used GLoVe vectors for representing words in the sentence and Peason Correlation Coefficient as 
			    a loss function. Therefore you need to first download the saved parameters from the link given below
			    and save them inside the folder "2017_takelab+cnn/". There are three saved parameters with their
			    respective links given below:

	 	            link1: https://drive.google.com/file/d/14PwedW7HM72TLU-XC2aDx-388voq-mL7/view?usp=sharing
			    link2: https://drive.google.com/file/d/1bOoRe7ZbMeQYrS1_NF4CpHZjyv0QkzBB/view?usp=sharing
			    link3: https://drive.google.com/file/d/10S7uE4hjvkEAggcj7jMZ-nSV76S9CRIr/view?usp=sharing

			    If everything goes right you will get a "weightfile0" file from link1, and you should paste it inside 
			    the folder 2017_takelab+cnn/.
			    
			    You will get a "weightfile1" file from link2, and you should paste it inside the folder 2017_takelab+cnn/.

			    You will get a "weightfile2" file from link3, and you should paste it inside the folder 2017_takelab+cnn/.


*****NOTE ON PREREQUISITES T0 RUN ALL THE CODES ABOVE****

Other than than the above mentioned "weightfile#" which are required particularly to run the code KACB_glove_coef.ipynb inside 
2017_takelab+cnn/, there are 5 text files more that are required by all the codes above, that you need to download. And should paste
all those text files inside 2017_takelab+cnn/ in order to run all the codes above. A link to all the text files with their corresponding
names is given below:

nyt_words.txt: 			https://drive.google.com/file/d/1lJFcCUHAD6bQ6vWL_WMv7U9yGq3-bnlk/view?usp=sharing
nyt_word_vectors.txt: 		https://drive.google.com/file/d/11TT2i3WGjrEZ6QJl1uxZTnIuk0K1IcV0/view?usp=sharing
wikipedia_words.txt:		https://drive.google.com/file/d/1M0hYI4N2v6DyBgHo-M9Te0dq9jhqCa3J/view?usp=sharing
wikipedia_word_vectors.txt:	https://drive.google.com/file/d/1uaizff-Nuv-WyUDt3kGJp6_kiDdFloLT/view?usp=sharing
word-frequencies.txt:		https://drive.google.com/file/d/1ddfI7Hob4eZZ3pWxCyw0JY_H440ywfWH/view?usp=sharing


Al the codes above requires a system with GPU and a RAM of above 12GB. Otherwise it can take more than a day or two to execute.
The output of each and every cell inside a code is saved and can be viewed for the reference. In order to run
and save the outputs once, these codes were executed on the GPU systems provided to users in NLE Lab by School of Computer
and Information Sciences(SCIS), University of Hyderabad, Hyderabad.
			    

Others
-----------------
sts-train.csv contains English sentence pairs for training from SemEval 2017 dataset
sts-dev.csv contains English sentence pairs for validaion from SemEval 2017 dataset
sts-tset.csv contains English sentence pairsfor testing from SemEval 2017 dataset


