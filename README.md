# Assignment1: Classification
##### By Mohammad Saif Anwer
##### BMC201614

Language used : Python

Packages imported :

	* pandas

	* scikit-learn

		-model_selection.KFold

		-tree.DecisionTreeClassifier

		+naive_bayes.Multinomial

Classifiers built :

	* Decision Tree
	
	* Naive Bayes
	
	* Support Vector Machine

The code reads a file __connect-4.data__ from the same folder using read_csv. We use __pandas.get_dummies(,drop_first=True)__ to One Hot encode the feature matrix, which we output alongside the target vector. This occurs in the function __preprocess( )__.

The three classifiers are applied using three functions __DecisionTree( )__, __NBayesian( )__, and __SVMachine( )__. Each of these take 3 arguments i.e. the feature matrix : X, target vector : Y, and a generator from splitting X using __KFold().split( )__ say kfg. Each of these classifiers perform 10-Fold CrossValidation on X and print out the test indices, their prediction, and accuracies for each "Fold", and conclude with the average accuracy.


