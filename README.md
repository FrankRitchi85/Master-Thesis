 
# Multimodal vs Multi-Model: A Comparative Analysis of Metadata Utilization in Skin Lesion Classification


Welcome. This repository contains all files related to my Master Thesis.

DELIVERABLES
- Thesis in PDF format

DATASET
- The used dataset, HAM 10000, is publicly accessible: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T 

NOTEBOOKS
- Preprocessing                                                        # Run first
- 16 Notebooks containing the one model each (8 multiclass, 8 binary)  # Run after preprocessing
- Evaluation                                                           # Run after model training creation
- Output                                                               # Run after Evaluation

PROCEDURE:
- Change the data folders to your own at the beginning of each notebook. As long as the data is stored in the same way it was downloaded 
- (images in 2 folders + a metadata .csv file), no further action is required.
- The final dataset used in the classification models is stored as a pickle-file after running the preprocessing file. This file should be used as input for the models
- After running the models, the trained models and relevant variables (e.g. y_tests and y_preds) are stored in pickles-files. These are used as input for the evaluation notebook.
- The Evaluation notebook runs on the test sets and outputs pickle-files of the evaluated models, that are used as input for the Output notebook
- The Output notebook creates the appropriate tables and plots.
