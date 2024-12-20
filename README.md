# Classification of Substances’ Permeability Through the Blood Brain Barrier Using Pretrained ChemBERTa Transformer Model 
The aim of this study is to develop a machine learning model for the classification of substances’ permeability through the blood-brain barrier using a pretrained ChemBERTa transformer. The dataset used in this study is the B3DB curated dataset, which contains 7,807 molecules in SMILES format, each labeled as either BBB+ (permeable – 4,956 instances) or BBB− (non-permeable – 2,851 instances). Python packages RDKit and Mordred were used to generate 3D chemical descriptors and molecular fingerprints. ChemBERTa was used to generate embeddings to represent the molecular descriptors. The data was split into a training set and a test set. For classification with neural networks, the training set was further split into a validation set – during the training of neural networks – to prevent bias. Three instances each of LGBM and XGBoost were trained with different combinations of features to establish a baseline. Subsequently, a feedforward network and a one-dimensional convolutional neural network (1D CNN) were trained on the embeddings and fingerprints feature set. The 1D CNN model achieved results comparable to the traditional methods used previously, with performance metrics including an accuracy of 89.7%, specificity of 85.3%, sensitivity of 92.5%, F1 score of 92.2%, Matthew’s correlation coefficient (MCC) of 0.78, AUC-ROC of 95.95%, and AUC-PRC of 97.65%.

----------------------------------------------------------------------------------------------------------------------------------------------
# Usage Notes 
1- Import the BBB_Test Notebook <br> 
2- Run until the line when importing the .pth model <br> 
3- Replace the path from google colab to the cnn_bbb_entire_model.pth that is present in the repo <br> 
4- Choose the SMILE you want and input the string into the cell <br> 
5- Run the notebook till the end and check the result <br> 
