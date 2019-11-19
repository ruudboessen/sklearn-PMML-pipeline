# sklearn-PMML-pipeline
Demo of a scikit-learn classification pipeline and its conversion to the PMML format.

The Jupyter Notebook presented here includes a concise demo of a scikit-learn pipeline and its conversion to the Predictive Model Markup Language (PMML) format in Python. PMML is an XML-based predictive model interchange format. It provides a way for analytic applications to describe and exchange predictive models. PMML is adopted by major analytic vendors including IBM, SAS, FICO, Zementis and many others, as well as various open-source platforms. Much more on the PMML format [here](https://en.wikipedia.org/wiki/Predictive_Model_Markup_Language) and [here](http://dmg.org/pmml/v4-3/GeneralStructure.html). 

The data for this demo came from: https://archive.ics.uci.edu/ml/datasets/census+income. It is also included in a ready-to-use comma separated text file. 

The pipeline includes pre-processing steps for categorical variables (one-hot encoding) and numerical variables (median imputation and scaling), K-best feature selection and a Multi-layer Perceptron (MLP) classifier. Other classifiers work as well (e.g. random forest or regression models). All the other elements of the pipeline can also be tuned and modified. The actual conversion to PMML was done using the [sklearn2pmml](https://github.com/jpmml/sklearn2pmml) Python package. 
