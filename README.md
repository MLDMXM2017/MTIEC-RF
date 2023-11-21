## MTIEC-RF
the source code, supplementary file of "Multi-task Multi-view and Iterative Error-Correcting Random Forest for Acute Toxicity Prediction".

##Annex_1
A supplementary file contains a table and a section to the manuscript.
SUPPLEMENTARY TABLE I, "INFORMATION ON THE MULTI-SPECIES ACUTE TOXICITY DATASET USED IN THIS STUDY"
Section G, "Parameter Analysis of MTIEC-RF"

## Requirements
Python==3.7.6    
numpy 
pandas      
sklearn    

## CodeAndData
(1)The feature folder contains 59 toxicity datasets, the feature type is Avalon.
(2)The label folder contains 59 label files corresponding to 59 toxicity datasets.
(3)The label is in the last column of the label file.

## GetResults

#Run the following commands in linux environment to obtain 5 reports corresponding to 5-fold cross-verification
nohup python ./Fold1_avalon.py > ./Avalon_fold1_report.log 2>&1 &
nohup python ./Fold2_avalon.py > ./Avalon_fold2_report.log 2>&1 &
nohup python ./Fold3_avalon.py > ./Avalon_fold3_report.log 2>&1 &
nohup python ./Fold4_avalon.py > ./Avalon_fold4_report.log 2>&1 &
nohup python ./Fold5_avalon.py > ./Avalon_fold5_report.log 2>&1 &

