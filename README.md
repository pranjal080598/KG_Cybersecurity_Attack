# 

# CMPUT-664-cybersecurity-knowledge-graph

## Group Members
|Student name| CCID |
|------------|------|
| Shraddha Mukesh Makwana     | smakwana |
| Pranjal Dilip Naringrekar   | naringre |


## Directory Structure
- `colab-notebooks`: contains experiments and processing done over Colabs notebooks
- `data`: dataset of CVE vulnerabilities taken from kaggle
- `spacy-relation-extraction`: contains modified base relation extraction given by Spacy

## Execution Steps


## Data
For data we have used publically available data set on Kaggle. Click [here](https://www.kaggle.com/datasets/andrewkronser/cve-common-vulnerabilities-and-exposures) to get the dataset.

## Acknowledgement 
The project was done under coursework of Prof. Karim Ali

## Resources 
- Converting to spacy file format: https://spacy.io/api/cli#convert
- Reference tutorial for initial trial experiments - https://ashutoshtripathi.com/2020/04/02/spacy-installation-and-basic-operations-nlp-text-processing-library/
- NER using spacy: https://towardsdatascience.com/named-entity-recognition-ner-using-spacy-nlp-part-4-28da2ece57c6
- Cuda issues on google colab with spacy: https://stackoverflow.com/questions/62655694/spacy-gpu-process-not-working-while-installed-prerequisites
- spacy base relation extraction template explanation: https://www.youtube.com/watch?v=8HL-Ap5_Axo
- documentation for internal working, command and configurations to be done: https://spacy.io/usage/layers-architectures
- relation extraction component issues: https://github.com/explosion/spaCy/discussions/9567
- working of neo4j with google colab: https://colab.research.google.com/github/johnymontana/ggcd-samples/blob/master/notebooks/ggcd.ipynb & https://towardsdatascience.com/create-a-graph-database-in-neo4j-using-python-4172d40f89c4 & https://stackoverflow.com/questions/48613002/sha-256-hashing-in-python
- neo4j queries to construct KG: https://neo4j.com/developer/graph-data-science/build-knowledge-graph-nlp-ontologies/ & https://neo4j.com/developer/cypher/guide-build-a-recommendation-engine/
