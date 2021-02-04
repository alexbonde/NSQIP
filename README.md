# Deep Learning in Surgery
Code accompanying the paper "Deep Learning in Surgery - Assessing The Utility of Deep Neural Networks in Predicting Postoperative Surgical Complications: A Retrospective Study"

<a href="http://example.com/" target="_blank">Hello, world!</a>


We have published five Jupyter notebooks: [one for data preprocessing](http://google.com){:target="_blank"}, one for each of the three models, and one for calculating personalized risk predictions. 
For privacy- and security reasons, we have chosen not to publish the identification numbers of the cases in our test set.

The interactive notebooks can be run using the IPython software at https://jupyter.readthedocs.io/en/latest/install/notebook-classic.html

The ACS NSQIP database can be requested through the American College of Surgeons website at https://facs.org

### Background
Early detection of postoperative complications (PCs), including developing organ failure, is pivotal in engaging targeted treatment strategies aimed at attenuating organ damage, i.e. broad-spectrum antibiotics for infections, fluid therapy for renal failure, high dose anticoagulants for venous thrombosis etc. In an era of increasing health-care costs and limited financial resources, identifying high-risk surgical patients as well as providing personalized precision-medicine based treatment strategies, provides an
obvious pathway for reducing patient morbidity and mortality. The objective of this study, is to assess whether recent advances in artificial intelligence and deep learning can be leveraged to train models on structured electronic health care data for surgical risk prediction

### Methods
This prognostic study obtained data from the 2012 – 2018 American College of Surgeons (ACS) National Surgical Quality Improvement Program (NSQIP) database, spanning more than 5.8 million adult surgical cases. We developed three deep neural network models with increasing levels of complexity. In line with the TRIPOD guidelines, we created an independent dataset for final model testing. This was achieved by identifying all patients that were treated at a large Midwestern United States academic medical center (n = 13,771, 0.02% of the adult NSQIP database) and excluding them from the base dataset. The remaining 5,868,110 cases (99,08 %) were randomly split into a training set (79.8%) and a validation set (20%). Output variables included mortality and any of 18 PCs. Model performance was evaluated on the test data, from the single academic medical center, using the area under the receiver operating characteristic curves (ROC AUC). 

### Model structure
![alt text](https://github.com/alexbonde/NSQIP/blob/main/model_structure.png?raw=true)

### Findings
The dataset included 5,881,881 cases with 2941 unique Current Procedural Terminology codes. The mean ROC AUCs of each model outperformed previously published metrics from other models, with a direct correlation between increasing model complexity and performance.

### Interpretation
We have developed a unified prediction model, based on deep neural networks, for the development of surgical postoperative complications. The model is generally superior
to previously published surgical risk prediction tools and appears robust to changes in the underlying patient population.

