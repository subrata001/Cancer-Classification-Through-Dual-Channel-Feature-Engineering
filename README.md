# Cancer-Classification-Through-Dual-Channel-Feature-Engineering

Dataset Type: External Test Set (Public) & Internal Test Set (Private).
Abbreviation: H for Hematoxylin and E for Eosin.
ROC: Receiver Operating Characteristic.

The Repository performs a classification task using test datasets on the trained models. The AI techniques used in this study for binary classification (benign vs. malignant and low-grade vs. high-grade) are support vector machine (SVM), logistic regression (LR), bagging tree, boosting tree, and dual-channel bidirectional long short-term memory (DC-BiLSTM) network. 
The regions of interest (ROIs) of H&E tissue samples extracted from whole slide images (WSIs) were used for generating the non-overlapping patches of size 64 × 64 pixels, and stain deconvolution technique was used to separate the Hematoxylin and Eosin channels.
For the private dataset of benign and malignant, we extracted 8000 patches from 500 ROIs of size 256 × 256 pixels. Out of these, 5120 for training, 1280 for validation, and 1600 for testing. Moreover, within the malignant tissues, 1600 patches were extracted separately from 100 ROIs (grade3=50 and grade5=50) to validate the performance of the trained classifiers in distinguishing between low-grade and high-grade disease. On the other hand, for the external test set, we extracted 10,240 patches from 10 ROIs of size 2048 × 2048 pixels, of which the best 8000 patches excluding background were selected for model validation in distinguishing between benign and malignant tissues.
