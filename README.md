# DutchParliamentCoreference
This repository contains both the code and instructions on how to run the experiments and obtain the data used in this article.
In the paper, two systems are run on the DutchParliament dataset, namely the DutchCoref model (https://github.com/andreasvc/dutchcoref) and the e2eDutch model(https://github.com/Filter-Bubble/e2e-Dutch). The code in this repository is a copy of the code found in the original repositories, with some minor adjustements.

## Downloading the dataset
  - The DutchParliament dataset is publicaly available, and can be downloaded from the following link: https://doi.org/10.17026/dans-x86-adrt
  
  
## Running the experiments
- For the experiments using the speaker metadata, the e2eDutch coference resolution model was adapted so that it works with the addition of speaker metadata.

### DutchCoref model
- For the DutchCoref model, the text data of the Parliament dataset has to be augmented with dependency tree information.
- The first step in this process is to run the `prepare_data_for_dutchcoref.py` script, which will create a new folder with the `xml` files containing the parsed sentences of the original text file.


## Extra notes

- Depending on the desired settings, the model can be run with either gold mentions, or the setting in which the model also predicts the mentions of the documents.
