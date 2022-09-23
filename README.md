# FreeSolv_df
Predicting free solvation energy for organic 

Termines here:
* Virtual screening - is a computational technique used in drug discovery to search libraries of small molecules in order to identify those structures 
which are most likely to bind to a drug target (typically a protein receptor or enzyme).
* RDKit - is a collection of cheminformatics and machine-learning software (module to process and work with chemical data);
* SMILES - Simplified Molecular Input Line Entry System;
* Morgan's fingerprints - binary molecular features of organic;

Annotation:
The work (and the steps described below of course) is targeted on reaching optimal "light" model for predicting the parameter of free solvation energy of 
organic substances for virtual screening.

Summary (according attached files):
* 1st step include extraction chemical data from SMILES, "raw" learning of some classic ML methods and perceptron ("raw" - without hyperparameters tuning) to estimate 
quality of "raw" models for the task permorming.
* 2nd step include extraction Morgan's fingerprints substances (instead of classic chemical features) with different bits lenght to check whether these one 
ensure greater accuracy in comparison with classical features. 
  Here is also tested dimensional reduction (PCA) to estimate how much data could be  compressed on with little loss of quality.
* Tuning files include search of optimal topology for 3 ML models (Bagging, Random forest and GradBoost regression) and perceptron.
