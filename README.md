# 🧩 MORCE — Multi-Ordering Rule-based Classifier Ensemble

### 🔀 Same data. Different orders. Different rules. Better predictions.

What if the order in which a classifier sees its training data could become a source of learning diversity?

**MORCE** explores this idea by training multiple RACER classifiers on different random orderings of the same training dataset, then combining their predictions through ensemble learning.

Instead of modifying RACER's original rule-generation mechanism, MORCE exploits its sensitivity to training-instance ordering to create diverse rule sets and improve classification performance.

### 🚀 Key Features

- 🔀 **Multi-Ordering Learning:** Train multiple RACER models using different permutations of the same training data.
- 🧩 **Rule-Based Diversity:** Exploit differences in the generated rule sets as a source of ensemble diversity.
- 🗳️ **Seven Aggregation Strategies:** Compare voting, weighted voting, top-k selection, and stacking approaches.
- 🧠 **Stacking-Based Learning:** Combine RACER predictions using Logistic Regression, Random Forest, and Gradient Boosting.
- 📊 **Comprehensive Evaluation:** Compare performance across 23 datasets using 10-fold cross-validation, accuracy, and F1-score.
- ⚖️ **Classifier Benchmarking:** Evaluate MORCE against RACER, its extensions, and several established machine-learning classifiers.

### 📈 Experimental Highlights

- 23 datasets from UCI and OpenML.
- 30 differently ordered RACER models per experiment.
- Stacking with Gradient Boosting achieves the strongest overall average performance.
- Improves RACER's average accuracy from **74.77% to 76.50%** and F1-score from **75.89% to 76.55%**.

### 🎯 The Core Idea

Turn training-order sensitivity into an advantage: multiple orderings produce diverse rule-based models, and ensemble learning brings their predictions together.

### 🛠️ Built With

`Python` · `NumPy` · `Pandas` · `scikit-learn` · `Joblib`

