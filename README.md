# pLDDT-prediction

deepchain.bio | Prediction AlphaFold pLDDT score

## pLDDT conda environment

From the root of this repo, create a virtual environment:
```conda create --name pLDDT python=3.7 -y
   conda activate pLDDT
```
you will need to manually install Bio-transformers by running:

```pip install bio-transformers```


## Overview 

Protein structures can provide invaluable information, both for reasoning about biological processes and for enabling interventions such as structure-based drug development or targeted mutagenesis. To frame that importance, they would fold into complex three-dimensional shapes. Thus, knowing how proteins fold is both difficult and absolutely costly, and time-consuming. Thanks to AlphaFold, we now have 3-D structures for virtually all __(98.5%)__ of the proteome. Alphafold produces a per-residue estimate of its confidence on a scale from 0 to 100 __"pLDDT"__ corresponds to the model’s predicted score on the IDDT-C alpha metric. To put this in perspective, we plan to predict pLDDT scores for a given protein sequence and, therefore we can estimate how mutagenesis can be confident in terms of pLDDT score. 

## Details
|                   |                           pLDDT-app                                               |
|------------------ | --------------------------------------------------------------------------------- |
| __Input__         |            Protein sequences                                                      |
| __Model__         |            RandomForest Regressor                                                 |
| __Output__        |            Predicted pLDDT score                                                  |
| __Dataset__       |            364171 PDBs                                                            |
| __Accuracy__      |            Root Mean Square Error (_RMSE_), coefficient of determination (_R2_)   |



