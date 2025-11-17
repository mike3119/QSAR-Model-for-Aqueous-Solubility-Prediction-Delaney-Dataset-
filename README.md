 **Delaney Solubility Prediction — Machine Learning with RDKit**

This repository contains a complete, reproducible workflow for predicting aqueous solubility (LogS) of organic molecules using classical machine-learning algorithms and molecular descriptors generated with **RDKit**.
The workflow is based on the **Delaney (ESOL)** dataset and is implemented in the included Jupyter notebook:

📄 **`Delaney solubility.ipynb`**

 ⭐ **Project Overview**

This project demonstrates how to:

* Load and analyze the **ESOL (Delaney)** dataset
* Convert SMILES strings into **RDKit molecular descriptors**
* Build and preprocess feature sets using **scikit-learn pipelines**
* Train and evaluate multiple ML models:

  * Linear Regression
  * Random Forest Regressor
  * (Any others added in the notebook)
* Perform:

  * Train/Test split
  * K-Fold cross-validation
  * Feature scaling
  * Feature selection (SelectKBest)
* Evaluate models with:

  * **Mean Absolute Error (MAE)**
  * **R² Score**

📂 **Repository Structure**

📁 Delaney-Solubility-ML
│
├── Delaney solubility.ipynb     # Main Jupyter Notebook
├── README.md                    # Project documentation
└── data/                        # (Optional) ESOL dataset if added later

 🧪 **Requirements**

Install the dependencies below before running the notebook:

pip install pandas numpy matplotlib seaborn rdkit-pypi scikit-learn


> Note: If RDKit installation fails, install via conda:

> conda install -c conda-forge rdkit

 🚀 **How to Use**

1. Clone the repository:

https://github.com/mike3119/QSAR-Model-for-Aqueous-Solubility-Prediction-Delaney-Dataset-

2. Navigate into the folder:

 https://github.com/mike3119/QSAR-Model-for-Aqueous-Solubility-Prediction-Delaney-Dataset-

3. Launch Jupyter Notebook:

jupyter notebook

4. Open **`Delaney solubility.ipynb`** and run all cells.

 🧠 **Methods & Techniques Used**

 **🔬 Molecular Featurization**

* RDKit descriptors
* Molecular weight
* LogP
* Number of hydrogen bond donors/acceptors
* Topological polar surface area
* And more (from rdMolDescriptors)

**📊 Machine Learning Pipeline**

* `train_test_split`
* `StandardScaler`
* `SelectKBest (f_regression)`
* Model training + evaluation

 **📈 Models Implemented**

* **Linear Regression**
* **Random Forest Regressor**
* (Expandable to XGBoost, SVR, Neural Networks)

 📉 **Model Performance**

The notebook includes detailed evaluation metrics, visualizations, and comparison between models:

* Regression scatter plots
* Error distribution plots
* Cross-validation scores
* Feature importance (for tree-based models)

 🎯 **Goals of This Project**

* Provide an easy-to-follow machine learning workflow
* Demonstrate how to work with molecular data
* Serve as a baseline model for solubility prediction research
* Enable further exploration into QSAR and cheminformatics

🤝 **Contributing**

Pull requests and improvements are welcome!
You can contribute by:

* Adding more ML models
* Improving molecular descriptors
* Adding hyperparameter tuning
* Enhancing visualizations

 📜 **License**

MIT 

MIT License ©akosumichaelhemen 2025

📣 **Acknowledgements**

* Delaney, John S. “ESOL: A dataset for aqueous solubility prediction.”
* RDKit (Open-source cheminformatics toolkit)
* scikit-learn (Machine learning library for Python)

