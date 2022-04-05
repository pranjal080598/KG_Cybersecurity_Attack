# CMPUT-664 Knowledge Graph Construction for Detecting Cybersecurity Attacks

## Group Members
|Student name| CCID |
|------------|------|
| Shraddha Mukesh Makwana     | smakwana |
| Pranjal Dilip Naringrekar   | naringre |


## Directory Structure
- `colab-notebooks`: contains experiments and processing done over Colabs notebooks
- `data`: dataset of CVE vulnerabilities taken from kaggle
- `spacy-relation-extraction`: contains modified base relation extraction given by Spacy
- `reports`: contain the proposal, check-in and final report

## Execution Steps
- **Step 1:** Create a folder on GDrive and place the converted spacy files given over there (Colab contains this step, but in order to skip converting spacy files it's been placed over there, as it might take time)
- **Step 2:** Execute Google colab step to train the model for entity recognition (It currently finds entity like VULNERABILITY and OPERATING_SYSTEM)
- **Step 3:** After that clone spacy's based project and excute commands as per colab to train relation extraction model (It currently finds HAS_VULNERABILITY relation). Also once clone command is ran given in the notebook, then inside rel_component folder, which will create at runtime, create another folder called 'data' and place all 3 spacy files and then run remaining command
- **Step 4:** Last part of google colab is to feed the data to Neo4j using queries for visualization
1. In order to do this step one has to first create an account over here [https://sandbox.neo4j.com/?usecase=blank-sandbox]
2. Create a new project, this will give host, username and credential to login to this neo4j project
3. In google colab notebook, put these temporary credentials to run it
4. Note: Neo4j sandbox gets expired within 3 days. Hence, every time we need to create new instance of project if we want to run it

- (**Note:** In general provided google colab notebook contains all the step. However, it took us couple of hours[approx. 4-5 hours] to train the model hence we have also placed screenshot of our previous successful run into the output folder for reference)
 

## Data
For data we have used publically available data set on Kaggle. Click [here](https://www.kaggle.com/datasets/andrewkronser/cve-common-vulnerabilities-and-exposures) to get the dataset.

## Acknowledgement 
The project was done under coursework of Prof. Karim Ali

## Resources 
- Converting to spacy file format: https://spacy.io/api/cli#convert

- Reference tutorial for initial trial experiments - https://ashutoshtripathi.com/2020/04/02/spacy-installation-and-basic-operations-nlp-text-processing-library/

- NER using spacy: https://towardsdatascience.com/named-entity-recognition-ner-using-spacy-nlp-part-4-28da2ece57c6

- Cuda issues on google colab with spacy: https://stackoverflow.com/questions/62655694/spacy-gpu-process-not-working-while-installed-prerequisites

- Spacy base relation extraction template explanation: https://www.youtube.com/watch?v=8HL-Ap5_Axo

- Documentation for internal working, command and configurations to be done: https://spacy.io/usage/layers-architectures

- Relation extraction component issues: https://github.com/explosion/spaCy/discussions/9567

- Working of neo4j with google colab: https://colab.research.google.com/github/johnymontana/ggcd-samples/blob/master/notebooks/ggcd.ipynb & https://towardsdatascience.com/create-a-graph-database-in-neo4j-using-python-4172d40f89c4 & https://stackoverflow.com/questions/48613002/sha-256-hashing-in-python

- Neo4j queries to construct KG: https://neo4j.com/developer/graph-data-science/build-knowledge-graph-nlp-ontologies/ & https://neo4j.com/developer/cypher/guide-build-a-recommendation-engine/
