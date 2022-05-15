# Sequence based prediction of Protein-Carbohydrate binding sites :

Nucleic acids, proteins, carbohydrates and lipids are four important molecules for any organisms, among them carbohydrates come after the DNA and proteins and which is thought about the third important molecule of life. The carbohydrates communicate with other protein molecules and these protein-carbohydrate interactions have several roles in different biological processes (cellular adhesion, cellular recognition, protein folding, subcellular localization, ligand recognition as well as in human body. Moreover, they provide a protection of human cell against pathogens as well as they play an important role as biomarkers or drug targets.

In order to identify protein-carbohydrate interactions, there are several experimental techniques have been performed although weak binding affinity and synthetic complexity of individual carbohydrates has made the study more expensive, time consuming and challenging. Therefore, developing a computational technique for effectively predicting protein-carbohydrate binding sites has become an urgent necessity. The computational approaches concentrate on locating the sites of proteins
that bind to carbohydrates. 

The computational studies involve different structure based and sequence-based methods. There are several structured based methods which have used to predict binding sites from a known protein structure. The problem of above structed-based techniques is that they are dependent on protein structures that are often not available.

A method, SPRTNT-CBH[1] was proposed in which PSSM features along with other predicted sequence and sequence-derived structure based features were employed to train support vector machine(SVM) classifier and it achieved an average of 18.8% sensitivity and 99.6% specificity while tested using 10-fold cross validation on train dataset having 102 protein-carbohydrate complexes and 22.3% sensitivity and 98.8% specificity while tested using an independent test set of 50 protein-carbohydrate complexes. The above-mentioned methods were failed to effectively identify the binding sites as they either results high sensitivity and low specificity or vice versa.

In order to look into this issue, StackCBPred[2] was trained by the balanced training dataset and this dataset was obtained by performing the random under sampling technique. Several evolution-derived and predicted sequence and structure-based features were extracted and stacking-based ensemble classifiers were used to train the dataset. Although this method achieved significant advancement in sensitivity and specificity compared to the aforementioned sequence-based approaches, this technique can discard potentially useful information and might not represent the real dataset as random under sampling technique was involved. Moreover, utilization of more relevant features could make the prediction performance more significant.



## References 
<a id="1">[1]</a>
G. Taherzadeh, et al., Sequence-based prediction of protein−carbohydrate binding sites using support vector machines, J. Chem. Inf. Model. 56 (2016).
<a id="2">[2]</a>
Gattani, Suraj, Avdesh Mishra, and Md Tamjidul Hoque. "StackCBPred: A stacking based prediction of protein-carbohydrate binding sites from sequence." Carbohydrate research 486 (2019): 107857.
