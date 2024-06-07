Project
Task Dataset: Molecular activity for 144 GPCR annotated proteins

Goal:
Students should be able to predict the activity of molecules for the file activity_test_blanked.csv given the data on activity_test.csv and eventually mol_bits.pkl

Data
The file activity_train.csv contains a list of interactions between molecules (identified by their ChEMBL IDs and proteins identified by their Uniprot IDs. The activity value is rated from 1 to 10, where 1 is INACTIVE and 10 is EXTREMELY POTENT
The file activity_test_blanked.csv has exactly the same structure as activity_train.csv, yet, the activiy values are all at Zero. The goal of the project is to predict the real values
Additionally it is provided the Fingerprints of molecules (mol_bits.pkl). Fingerprinting is a hashed structural representation of molecules, where each set bit represents a structural feature. Molecules that have a common bit set mean that they probably share a structural element. This file is a Zipped pickled file that contain a dictionary with keys corresponding the ChEMBL IDs and values corresponding to a list of the set bits of each molecule.
The total number of activities measured for the whole dataset is 140,339, of which 135,711 were selected for training and 4,628 for validation, out of 144 protein targets and 73,865 different molecules.
