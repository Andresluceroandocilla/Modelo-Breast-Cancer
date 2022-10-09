# Modelo-Breast-Cancer
Modelos de Machine Learning para predecir si un tumor es maligno  o  benigno

Se utiliza Jupyter Notebook y las librerías de Python para trabajar con tablas (Pandas), modelos de machine learning (Sklearn) y graficas (Matplotlib), el objetivo es poner a prueba diferentes modelos de aprendizaje supervisado con un dataset que contiene información de las dimensiones físicas de tumores.  Se obtiene el dataset directamente del repositorio de https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data. El propio repositorio explica que hay 32 atributos, los nombres lode los atributos se obtuvieron de Kaggle https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data.

El objetivo es lograr la mayor exactitud posible en los resultados malignos ya que un falso positivo no es tan grave como un falso positivo.
Se probaron 4 modelos:  sklearn.linear_model.SGDClassifier, sklearn.neighbors.KNeighborsClassifier, sklearn.tree.DecisionTreeClassifier y sklearn.ensemble.RandomForestClassifier
Resultados:
sklearn.linear_model.SGDClassifier
•	Accuracy score train 91%
•	Accuracy score test 93%
•	Precision score malignant 94%
•	Precision score benignant 92%
sklearn.neighbors.KNeighborsClassifier
•	Accuracy score train 94%
•	Accuracy score test 93%
•	Precision score malignant 95%
•	Precision score benignant 92%
sklearn.tree.DecisionTreeClassifier
•	Accuracy score train 97%
•	Accuracy score test 96%
•	Precision score malignant 94%
•	Precision score benignant 92%
sklearn.ensemble.RandomForestClassifier
•	Accuracy score train 97%
•	Accuracy score test 98%
•	Precision score malignant 98%
•	Precision score benignant 98%
Se elige al modelo de Random forest como el mejor modelos ya que se obtiene un 98% de precisión en evaluación test minimizando el riesgo de falsos negativos. La variable más importante para la clasificación es el perimeter_worst.
