# Methods, resources and technology on Hybrid NLP

## Overview
Both neural and knowledge-based approaches to natural language processing have strong and weak points. Neural methods are extremely powerful and consistently claim the top positions of current NLP leaderboards. However, they are also sensitive to challenges like the amount and quality of training data or linking the models to how humans use the language and their understanding of the world. On the other hand, although not entirely free from such challenges, NLP systems based on structured knowledge representations tend to be better suited to address some of them. However, they may require considerable knowledge engineering work in order to continuously curate such structured representations. 

We believe that data-driven and knowledge-based approaches can complement each other nicely to boost strengths and alleviate weaknesses. Although many advocate for the combined application of both paradigms in NLP as well as many other areas of Artificial Intelligence, the truth is that until now such combination has been unusual, due to reasons that may include a possible lack of principled approaches and guidelines to accomplish such goal and a shortage of compelling resources or success stories. 

This repository aggregates our work in the topic of hybrid NLP, understood as a collection of methods, techniques and technology involving both neural and knowledge based approaches to NLP and its applications. It contains links to other repositories and bibliography.

The content of this repository addresses a number of research questions related to hybrid NLP systems, including: 
* How can neural methods extend previously captured knowledge explicitly represented as knowledge graphs in cost-efficient and practical ways and vice-versa?
* What are the main building blocks and techniques enabling a hybrid approach to NLP that combines neural and knowledge-based approaches?
* How can neural and structured, knowledge-based representations be seamlessly integrated?
* Can this hybrid approach result in better knowledge graphs and neural representations?
* How can the quality of the resulting hybrid representations be inspected and evaluated?
* What is the impact on the performance of NLP tasks, the processing of other data modalities, like images or diagrams, and their interplay?

## Bibliography

The following book will give you a good insight on Hybrid NLP:

**_Jose Manuel Gomez-Perez, Ronald Denaux and Andres Garcia-silva. 2020. A Practical Guide to Hybrid Natural Language Processing - Combining Neural Models and Knowledge Graphs for NLP. https://doi.org/10.1007/978-3-030-44830-1_**

```bibtex
@book{10.1007/978-3-030-44830-1,  
author = {Gomez-Perez, Jose Manuel and Denaux, Ronald and Garcia-Silva, Andres},  
title = {A Practical Guide to Hybrid Natural Language Processing - Combining Neural Models and Knowledge Graphs for NLP.},  
year = {2020},  
isbn = {978-3-030-44830-1},  
publisher = {Springer Publishing Company, Incorporated},  
edition = {1st},  
abstract = {This book provides readers with a practical guide to the principles of hybrid approaches to natural language processing (NLP) involving a combination of neural methods and knowledge graphs. To this end, it first introduces the main building blocks and then describes how they can be integrated to support the effective implementation of real-world NLP applications. To illustrate the ideas described, the book also includes a comprehensive set of experiments and exercises involving different algorithms over a selection of domains and corpora in various NLP tasks. Throughout, the authors show how to leverage complementary representations stemming from the analysis of unstructured text corpora as well as the entities and relations described explicitly in a knowledge graph, how to integrate such representations, and how to use the resulting features to effectively solve NLP tasks in a range of domains. In addition, the book offers access to executable code with examples, exercises and real-world applications in key domains, like disinformation analysis and machine reading comprehension of scientific literature. All the examples and exercises proposed in the book are available as executable Jupyter notebooks in a GitHub repository. They are all ready to be run on Google Colaboratory or, if preferred, in a local environment. A valuable resource for anyone interested in the interplay between neural and knowledge-based approaches to NLP, this book is a useful guide for readers with a background in structured knowledge representations as well as those whose main approach to AI is fundamentally based on logic. Further, it will appeal to those whose main background is in the areas of machine and deep learning who are looking for ways to leverage structured knowledge bases to optimize results along the NLP downstream.}  
}
```

If you find these resources helpful, please cite it.

## Tutorial on Hybrid Techniques for Hybrid Natural Language Processing

This tutorial covers the foundations and modern practical applications of knowledge-based and neural methods, techniques and models and their combination for exploiting large document corpora. The tutorial first focuses on the foundations that can be used to this purpose, including knowledge graphs, word embeddings, and language models. Then it shows how these techniques can be effectively combined in NLP tasks and other data modalities in addition to text related to research and innovation projects. 

You can find the Jupyter notebooks of the different lessons of the tutorial directly [here](https://github.com/hybridnlp/tutorial).

## Vecsigrafo and Transigrafo

Knowledge graph embedding algorithms can capture structured knowledge about concepts and relations in a graph as embeddings in a vector space, which then can be used in downstream tasks. However, this type of approaches can only capture the knowledge that is explicitly represented in the graph, hence lacking in recall and domain coverage. Here we include tow examples of algorithms that address this limitation through the combination of information from both unstructured text corpora and structured knowledge graphs.

The first approach is [Vecsigrafo](http://www.semantic-web-journal.net/content/vecsigrafo-corpus-based-word-concept-embeddings-bridging-statistic-symbolic-1), which produces corpus-based word, lemma and concept embeddings from large disambiguated corpora. Vecsigrafo jointly learns word, lemma and concepts embeddings, bringing together textual and symbolic knowledge representations in a single, unified formalism for use in neural natural language processing architectures. 

The second and more recent approach is called [Transigrafo](https://github.com/hybridnlp/LMMS), which adopts recent Transformer-based language models to derive concept-level contextual embeddings, providing state of the art performance in word-sense disambiguation with reduced complexity.


