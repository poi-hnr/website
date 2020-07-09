---
title: "Methodology"
draft: true
---

Network perspective is nothing more than a way to look at interpersonal relationships, and in the context of the present study this concept should be understood as intentional behavior targeted at building a social network. The basic research tool is the Social Network Analysis, a method that uses the network theory and the graph theory to investigate the structure of relations between different types of social subjects. Therefore, the subject matter of the analysis is not the characteristics of the subjects analyzed, but the wide range of relations between them - from simple interpersonal relationships to economic or political connections. By applying this method to the Portuguese colonial society, it is intended to explore the position of individuals in the structure, to isolate the individual groups, to focus on connections and relationships, and finally to conduct a global analysis of the structure of the entire network. The network analysis is the tool that serves only for interpreting the dynamics of links between individuals (nodes) in Portuguese colonies. It complements the qualitative analysis, which will be carried out in the Overseas Historical Archive in Lisbon, as well as in archives located in Brazil. The source is provided by the correspondence between selected individuals and the Lisbon administration, constituting key nodes in networks. The following elements of those letters will be analyzed: rhetoric, structure and technique of writing letter, patterns, narration of the problem, social attributes, how they identified themselves and what was their location in the network structure like.

Techniques

- Natural Language Processing
- Named-entity Recognition (NER)
- Regular Expressions Techniques
- Latent Dirichlet Allocation (LDA)

Step by step:

- Perform Analysis of the corpus of around 170,000 documents from Portuguese Overseas Archives, to get standard structures of the documents and to prepare for Natural Language Processing (Python/SpaCy)
- Create new specific entities in the in the Named Entity Recognizer (NER) model to match the needs of the communication documents (Python/SpaCy), as a result of which a formData in a JSON were created.
- Train a NER model to capture key information in the documents in Portuguese (Python/SpaCy) as a result of which Python script and the resulting database in theform of a JSON file.
- Perform topic model analysis (LDA) of the whole corpus (Python/Mallet) as a result of which a Python script was created and a document/elaboration of the analysis results.
- Create networks with rich node information (node attributes) for posterior social network analysis of the Portuguese Empire (Python/Networkx) as a result of which a Python script and processed network data in the form of CSV files with (1) nodes and their attributes, (2) edges and their attributes were created.

