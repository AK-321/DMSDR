# DMSDR
## Folder Specification
- data/ folder contains necessary data or scripts for generating data.
  - idx2SMILES.pkl: Drug ID to drug SMILES string dictionary
  - ddi_mask_H.pkl: A mask matrix containing the relations between molecule and substructures
  - substructure_smiles.pkl: A list containing the smiles of all the substructures.
  - ehr_adj_fianl.pkl/ehr_adj_fianl_4.pkl:Patient ehr representations on the MIMIC-III and MIMIC-IV datasets.
  - ddi_A_fianl.pkl/ddi_A_fianl_4.pkl:Patient ddi representations on the MIMIC-III and MIMIC-IV datasets.
  - records_fianl.pkl/records_fianl_4.pkl:Preprocessed MIMIC-III and MIMIC-IV datasets.
  - voc_fianl.pkl/voc_fianl_4.pkl:The index correspondence table.

- src/ folder contains all the source code.
  - modules/: Code for model definition.
  - utils.py: Code for metric calculations and some data preparation.
  - training.py: Code for the functions used in training and evaluation.
  - main.py: Train or evaluate our DFHD Model.


## STEP1:Package Dependency

- Make sure your local environment has the following installed:
  
  - python 3.8.5, scipy 1.10.1, pandas 1.1.3, torch 1.12.1, numpy 1.19.2, dill, rdkit 

## STEP2:Run Model

  ```
  python main.py 
  ```
