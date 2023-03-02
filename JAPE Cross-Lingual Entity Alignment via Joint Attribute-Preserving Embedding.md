---
layout: 'jape: cross-lingual'
title: Embedding
date: 2021-02-27 14:30:03
tags:
---
JAPE is a method for cross-lingual entity alignment, which involves identifying equivalent entities across different knowledge graphs in different languages. The method is based on joint attribute-preserving embedding, which learns embeddings for entities and relations that preserve their attributes across different languages.

The JAPE model consists of two components: a monolingual component and a cross-lingual component. The monolingual component learns embeddings for entities and relations within each language-specific knowledge graph. The cross-lingual component learns embeddings that align the entities and relations across different languages.

The monolingual component is based on the TransE model, which represents each relation as a translation vector that connects the embeddings of the head and tail entities. The model is extended to include attribute embeddings, which capture the attributes of the entities and relations, such as their names and types.

The cross-lingual component is based on a joint embedding model, which learns a shared embedding space that captures the cross-lingual semantic similarity between entities and relations. The model is trained to preserve the attributes of the entities and relations across different languages, while also ensuring that the embeddings are close in the shared space.

To evaluate the performance of JAPE, the method is tested on several cross-lingual entity alignment tasks, including aligning entities across English and Chinese knowledge graphs. The results show that JAPE outperforms several state-of-the-art methods on these tasks.

The code for JAPE is available on GitHub at https://github.com/nju-websoft/JAPE. The code is implemented in Python and uses the PyTorch deep learning framework. The repository includes examples of how to use the code on different cross-lingual entity alignment tasks and provides detailed documentation on how to install and run the code.

TransE is a method for knowledge graph embedding, which involves representing entities and relations in a low-dimensional continuous space. The method is based on the idea that relations can be represented as translations between the embeddings of their associated entities.

In TransE, each entity and relation is represented as a low-dimensional vector. The method defines a scoring function that measures the plausibility of a triple (head entity, relation, tail entity) in the knowledge graph. The scoring function computes the distance between the embedding of the head entity and the embedding of the tail entity translated by the embedding of the relation.

During training, the TransE method optimizes the embeddings to minimize the distance between the embeddings of the head and tail entities, translated by the embedding of the relation, for true triples in the knowledge graph, while maximizing the distance between the embeddings for false triples.

TransE has been shown to perform well on various knowledge graph completion tasks, such as link prediction and entity prediction. The method is widely used in the field of knowledge graph embedding and has inspired many variants and extensions, such as TransH, TransR, and TransD.

The code for TransE is available on GitHub and implemented in various programming languages, including Python, Java, and C++.

import torch
import torch.nn as nn
import torch.nn.functional as F

class TransE(nn.Module):
    def __init__(self, num_entities, num_relations, emb_dim):
        super(TransE, self).__init__()
        self.entity_embeddings = nn.Embedding(num_entities, emb_dim)
        self.relation_embeddings = nn.Embedding(num_relations, emb_dim)
        
    def forward(self, heads, relations, tails):
        head_embeddings = self.entity_embeddings(heads)
        relation_embeddings = self.relation_embeddings(relations)
        tail_embeddings = self.entity_embeddings(tails)
        
        # Compute the score for each triple (head, relation, tail)
        scores = torch.norm(head_embeddings + relation_embeddings - tail_embeddings, p=1, dim=1)
        
        return scores


This code defines a TransE model using PyTorch, with entity and relation embeddings represented as nn.Embedding layers. The model takes as input the indices of the head entities, relations, and tail entities, and computes the score for each triple using the TransE scoring function, which is the L1 norm of the sum of the head entity and relation embeddings, subtracted from the tail entity embedding.

To train the model, you would use a loss function such as the margin-based ranking loss, which aims to maximize the margin between the scores of true triples and false triples. You would also use an optimizer such as stochastic gradient descent (SGD) to update the model parameters based on the gradients of the loss function.

In the context of knowledge graph embedding, a commonly used loss function for training TransE and other embedding methods is the margin-based ranking loss, which aims to maximize the margin between the scores of true triples and false triples.

The margin-based ranking loss is defined as follows:

L = sum(max(0, gamma + s_neg - s_pos))
where gamma is a hyperparameter that controls the margin, s_pos is the score of the true triple, and s_neg is the score of a negative triple that is constructed by replacing either the head or tail entity of the true triple with another entity in the knowledge graph.

The loss function encourages the scores of true triples to be higher than the scores of negative triples by at least the margin gamma. The max function ensures that the loss is only computed for negative triples that have a higher score than the true triple by less than the margin, so that the loss is zero when the model is already correctly ranking the triples.

Here is an example of PyTorch code for defining the margin-based ranking loss:

import torch.nn.functional as F

def margin_ranking_loss(scores, margin=1.0):
    # Split the scores into positive and negative triples
    s_pos = scores[::2]
    s_neg = scores[1::2]
    
    # Compute the loss for each pair of positive and negative scores
    loss = F.margin_ranking_loss(s_pos, s_neg, target=torch.ones_like(s_pos), margin=margin)
    
    return loss
This code takes as input a tensor of scores for positive and negative triples, where the scores are concatenated such that the first score is for a positive triple, the second score is for a negative triple, and so on. The margin_ranking_loss function from PyTorch is used to compute the margin-based ranking loss for each pair of positive and negative scores. The target argument is set to torch.ones_like(s_pos) to indicate that the loss should encourage the positive scores to be higher than the negative scores, and the margin argument is set to the desired margin value.

You would use this loss function during training to compute the gradients of the model parameters with respect to the loss, and update the parameters using an optimizer such as stochastic gradient descent (SGD).



