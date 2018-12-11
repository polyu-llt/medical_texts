# Medical texts processing

Annie Xiaowen (Principal invistigator), Chu-Ren Huang (project supervisor), Natalia Klyueva, Emmanuele Chersoni (technical assistants)

This projects aims at processing medical texts with the possible goal of terminology extraction,
ontology generation and other possible NLP-related experiments with data.

The corpus of medical texts from PLOS ONE provided by Annie contains more than 12574840 words for all domains. 

## Relationship extraction

Data: 
- terminology list (Extracted by Annie from the corpus)
- CONCEPT.csv (indexer file)
- CONCEPT_RELATIONSHIP.csv

### linux commands to operate with the files:
`cat CONCEPT_RELATIONSHIP.csv| cut -f3 | sort | uniq -c | sort -nr | less` - get the sorted list of relationship with counts of how frequent are relationships 


## Parsing
We parsed the data with UD-pipe, scripts are available in the repository.

## Ontology generation
Work in progress...  Possible links that might be useful in our research:

https://www.nlm.nih.gov/research/umls/implementation_resources/metamap.html


More NLP-oriented:

https://www.cse.iitb.ac.in/~pb/papers/bionlp-acl17-medical-coding.pdf

https://ieeexplore.ieee.org/document/7776412
