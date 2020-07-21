Five different types of experiments have been implemented by modifying the existing CNN architecture (by changing the loss
function and word vector embeddings) for computing similarity between two sentences. The description for each of them
corresponding to the code name is given below.

Experiment                      Description

1) fasttext_coef.ipynb          In this experiment embeddings are replaced with fasttext embeddings, keeping the loss function
                                same.

2) fasttext_kl.ipynb            Here also, both embeddings and loss functions have been replaced with word2vec and
                                KL-Divergence respectively.

3) glove_kl.ipynb               In this experiment we have replaced loss function correlation coefficient
                                with KL-Divergence loss function.

4) word2vec_coef.ipynb          In this experiment we have replaced pretrained GloVe word embeddings
                                with pretrained word2vec embeddings.

5) word2vec_kl.ipynb            Here both embeddings and loss functions have been replaced with
                                word2vec and KL-Divergence respectively.

There is one more code named glove_coef.ipynb,it is actually the reimplementation of the existing CNN architecture and it
contains the combination of correlation coefficient and Glove as the loss function and word vector respectively.

This code can only run on Jupyter Notebook and works fast on CPU of RAM more than 4GB, otherwise it may take more than
one hour to run . You can run this code on Google Colab Notebook as well,as it provides a GPU and a CPU of RAM upto 25GB,
which is sufficient for these codes run.

*NOTE*
The codes "fasttext_coef.ipynb" and "fasttext_kl.ipynb" cannot run here in Google Colab from the directory which is
shared here, because the fasttext word embedding file size is around 7GB, and the Google Storage is not sufficient to
store it. As, already word2vec embedding and Glove word vectors embedding is uploaded here on the drive, which are
3GB and 5GB in size. Therefore, we need a total of more than 15GB of size as STS dataset also need some storage. But
excluding fasttext word embedding we have already filled 12GB of space.