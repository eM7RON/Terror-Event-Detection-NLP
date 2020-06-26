# Terror Event Detection NLP

This is some of the code from my masters thesis 2019 which explored the possibility of detecting `terror events` in text, more specifically news documents.

It's a somewhat rudimentary method designed to eventually work in a pseudo online setting.

The idea is that a document stream is quantized into time intervals. At each interval, the new documents are projected into a latent space by a Doc2Vec model. Documents that contain information about a specific terror event are seperated out by an SVM. The positive documents then go through named entity detection (NER) using StanfordCoreNLP. I then performed some network analysis which can be seen in the thesis. 

<p align="center">
     <img src="https://github.com/eM7RON/Terror-Event-Detection-NLP/blob/master/img/method_outline.png" alt="nlp" width="500"/>
</p>

### Installing

There are some helpful instructions and hints on how to get the code running in each jupyter notebook. The code requires some large pretrained doc2vec models which I have not included but can be obtained from a link below.

## Requirements
Python 3  
Java 8  
StanfordCoreNLP  

## License & copyright

© Simon Tucker, eM7RON  

Pretrained doc2Vec models were obtained from [*https://github.com/jhlau/doc2vec*](https://github.com/jhlau/doc2vec)  

Jey Han Lau and Timothy Baldwin (2016). [An Empirical Evaluation of doc2vec with Practical Insights into Document Embedding Generation.](https://arxiv.org/abs/1607.05368) In Proceedings of the 1st Workshop on Representation Learning for NLP, 2016.
