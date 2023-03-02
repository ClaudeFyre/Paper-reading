---
layout: 'mtranse: multilingual'
title: MTransE Multilingual Knowledge Graph Embeddings for Cross-lingual Knowledge Alignment
date: 2021-02-27 13:18:53
tags:
---
MTransE is a method for learning multilingual knowledge graph embeddings to facilitate cross-lingual knowledge alignment. The goal of cross-lingual knowledge alignment is to align entities and relations between two or more knowledge graphs in different languages.

The MTransE method learns a set of low-dimensional embeddings for entities and relations in multiple knowledge graphs simultaneously. The embeddings are learned by optimizing a loss function that captures both the intra-lingual and cross-lingual information in the knowledge graphs. The loss function is based on the TransE model, which represents each relation as a translation vector that connects the embeddings of the head and tail entities.

To learn multilingual embeddings, MTransE uses a shared space model that learns a common embedding space for all the languages. It also incorporates a translation matrix for each language that maps the common embedding space to the language-specific embedding space. This allows the method to capture the cross-lingual semantic similarity between entities and relations.

MTransE has been shown to be effective on various cross-lingual knowledge alignment tasks and is widely used in the field of multilingual knowledge representation and reasoning. The method can be extended to handle more than two languages and can be combined with other methods for further performance improvement.


The methodology of MTransE for learning multilingual knowledge graph embeddings for cross-lingual knowledge alignment can be summarized as follows:

    Data preparation: MTransE takes as input a set of knowledge graphs in different languages that share a common set of entities and relations. It also requires a set of cross-lingual links that connect entities across the different knowledge graphs.

    Multilingual embedding learning: MTransE learns a set of low-dimensional embeddings for entities and relations in all the knowledge graphs simultaneously. It uses a shared space model that learns a common embedding space for all the languages and a translation matrix for each language that maps the common embedding space to the language-specific embedding space. The embeddings are learned by optimizing a loss function that captures both the intra-lingual and cross-lingual information in the knowledge graphs. The loss function is based on the TransE model, which represents each relation as a translation vector that connects the embeddings of the head and tail entities.

    Alignment learning: MTransE uses the learned embeddings to align entities and relations across the different knowledge graphs. It does this by finding the nearest neighbors of each entity in each of the other language-specific embedding spaces. It then maps the entity to the language-specific entity with the highest similarity score.

    Evaluation: MTransE evaluates the quality of the entity alignment by comparing the aligned entities with a gold standard set of cross-lingual entity alignments. It uses various evaluation metrics, such as precision, recall, and F1-score, to measure the effectiveness of the alignment.

Overall, MTransE learns multilingual knowledge graph embeddings using a shared space model and translation matrices and uses the embeddings to perform cross-lingual knowledge alignment. The method has been shown to be effective on various cross-lingual knowledge alignment tasks and is widely used in the field of multilingual knowledge representation and reasoning.