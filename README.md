# Machine-Translation-NLP
Implemented Naive Machine Translation system with K-NN
<a name="2"></a>

# Translations

<div style="width:image width px; font-size:100%; text-align:center;"><img src='./images/e_to_f.jpg' alt="alternate text" width="width" height="height" style="width:700px;height:200px;" /> Figure 2 </div>

Program that translates English words to French words using word embeddings and vector space models. 

<a name="2-1"></a>
## Translation as linear transformation of embeddings

Given dictionaries of English and French word embeddings you will create a transformation matrix `R`
* Given an English word embedding, $\mathbf{e}$, you can multiply $\mathbf{eR}$ to get a new word embedding $\mathbf{f}$.
    * Both $\mathbf{e}$ and $\mathbf{f}$ are [row vectors](https://en.wikipedia.org/wiki/Row_and_column_vectors).
* You can then compute the nearest neighbors to `f` in the french embeddings and recommend the word that is most similar to the transformed word embedding.
