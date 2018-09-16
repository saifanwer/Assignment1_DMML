# Assignment1: Classification
##### By Mohammad Saif Anwer (BMC201614)

Language used : Python

Packages imported :

	pandas

	scikit-learn

		model_selection.KFold

		tree.DecisionTreeClassifier

		naive_bayes.Multinomial

Classifiers built :

	Decision Tree
	
	Naive Bayes
	
	Support Vector Machine

The data first undergoes a function called _preprocess()_. Here _connect-4.data_ is read using pandas.read_csv. The resulting DataFrame is used to construct __y__, the target vector and, after a One Hot Encoding with _pandas.get_dummies(,drop_first = True)_
, the feature matrix X.
Then, we use KFold_
