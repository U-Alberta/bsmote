# CMPUT 701 : Capstone Project
# In-Domain Claim Identification for Imbalance Datasets using Oversampling Techniques:
A claim is a declaration or insistence that something is true, made without offering any supporting data or proof. Claim Identification is a crucial precondition for fact-checking. There are two kinds of claim identification process: one variant is called In-Domain Claim Identification, where the dataset is trained on the same domain on which it will be tested, and Cross-Domain Claim Identification, where the testing dataset might not be of the same domain the model is trained. We have discussed In-Domain Claim Identification for imbalance datasets because, from understanding the previous work, there are a few limitations: 1) It is not always possible to find the source of the dataset and extract more data to make it balanced, and 2) Undersampling leads to loss of essential data. This paper addresses both problems. We have selected two imbalanced datasets, named Persuasive Essays (PE) and Wiki Data Claim (WDC), and balanced them using five pre-built synthetic data generation techniques and one statistic variant of Borderline-SMOTE (BSMOTE). The statistical variant of BSMOTE improves the claim identification process by 17.6\%. The experiment results are promising, and overall, the F1 score of the new balancing technique outperforms the previous work's results.


# Dataset
We have used two imbalanced datasets with target labels, Claims and Premises. Premises are in significantly higher numbers compared to that Claims. The two datasets are: 1) Argument Annotated Persuasive Essay (PE), and 2) Wiki Data Claim (WDC). 
PE and Micro Text (MT)  yielded the best results for the in-domain experiments because these two datasets have higher proportions of claims, 21.6% and 24.9% respectively, if compared to the remaining datasets such as Web Discourse (WD) with 5.4% or Online Comments (OC) with 7.8%.

The second dataset Wiki Data Claim (WDC), is not publicly available. We have created it by combing the claims of UKP Aspect Corpus with the facts extracted from Wikipedia using WikiData API.


# Environment

* OS: MacOS 7

* GPU stat: GeForce RTX 2080 (X4)

* libraries
1. Keras : `pip install keras`
2. Sentence Transformer : `pip install sentence-transformers` 
3. Wikipedia Api: `pip install Wikipedia-API`

# How to run Codes

Please download the dataset first from here: [Dataset](https://drive.google.com/drive/u/2/folders/1jvdz3hNuyuqJckclLMFv7nZiht5dXotU). Unzip the file in the directory. Since we provide pickle files to save your time for data preprocessing, the directory size is almost 10GB.

## Dataset
* Location: processed_dataset/


## Wiki Data Claim Python Notebook
* Location: Data Exploration Wiki Data.ipynb

* WDC Data Exploration: You can run the code step by step from jupyter notebook named *Data Exploration Wiki Data.ipynb*

## Persuasive Essay
*Location: Data Exploration Persuasive Essay.ipynb
* Persuasive Essay: You can run the code step by step from jupyter notebook named *Data Exploration Persuasive Essay.ipynb*

# Results


# Email us!

If you have any question, or if the codes doesn't work, please let us know through email: bspatel@ualberta.ca
