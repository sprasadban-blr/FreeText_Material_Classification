# Free Text Material Classification
Analysis on Free Text Material classification

Prerequisite:
  * Install Python 3.6 https://www.python.org/downloads/release/python-368/ 
	* Install needed python libraries
		- python -m pip install --upgrade pip
		- pip install numpy
		- pip install pandas
		- pip install seaborn		
		- pip install sklearn
		- pip install matplotlib
		
Step 1: Clone git
  * $SRC_DIR>git clone https://github.wdf.sap.corp/I050385/freetext_material_classification
  
Step 2: Jupyter notebook "Free Text Material Classification.ipynb" contains algorithms tried out 
  * Tried Multinomial Naive Bayes algorithm 
  * Tried Support Vector Machine (SVM) algorithm
  * Tried Multiclass Logistic Regression
  * Tried K-Nearest Neighbour (KNN) algorithm

* Highlights:
	- Used NLP data preprocessing techniques to clean up material description
	- Used TF-IDF features on material description, BoW is another option we can look out.
	- Used above mentioned algorithms to test the training and test set prediction accuracy.
	- On comparision with test set accuracy, SVM performs better algorithm for the given data set

* About Dataset:
	1. Data collection is skewed, some classes have only one or two samples
    2. Data is imbalanced, all class labels must have equal propotion of samples
    3. Data cleanup is required, empty description or 1 or 2 character descriptions are considered noise
    4. Tried with TF-IDF metrics as features, we can use other metrics such as BoW.
    5. Data columns such as extsourcesystem, companycode and plant all are same and doesn't contribute much for target variable 'materialgroup'
    6. Identify right set of other features which contributes target variable material group
