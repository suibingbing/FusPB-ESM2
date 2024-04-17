# FusPB-ESM2 file structure
The FusPB-ESM2 folder contains 4 files and 1 word folder. Here is a description of them:

1.data
The data folder is the dataset folder. Inside, "trainCPP.csv" is the training set; "testCPP.csv" is the independent test set.

2.Five_fold_esm.ipynb
This file is the 5 fold cross-validation code for the three versions of the ESM2 model to make separate predictions.

3.Five_fold_protbert.ipynb
This file is the 5 fold cross-validation code for the two versions of the ProtBert model to make separate predictions.

4.Five_fold_fusion.ipynb
This file is the 5 fold cross-validation code for feature fusion with different versions of ESM2 and ProtBert.

5.Five_fold_d_mapping.ipynb
This file is the 5 fold cross-validation code for different dimensional mappings.

6.Independent_testing.ipynb
This file is the code that was tested on the independent test set.

7.environment.yml
This file documents the environment required for the code to run.

# Run
1.Run the following command to install the environment：conda env create -f environment.yml.

2.Just open each jupyter notebook and run it. There are corresponding instructions in each Jupyter Notebook.
