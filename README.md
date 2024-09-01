# Bioactivity Prediction using Deep Neural Networks
## Project Overview
This project aims to predict the bioactivity of molecules using deep neural networks. The prediction model is built upon the BACE dataset from MoleculeNet, which contains information on compounds tested for their ability to inhibit human beta-secretase 1 (BACE-1). The model utilizes various molecular representations, including molecular fingerprints, graph representations, and Tanimoto similarity, to predict bioactivity. The model leverages advanced techniques like L1 and L2 regularization and hyperparameter optimization to enhance prediction accuracy.

## Dataset
The dataset used in this project is the BACE dataset from MoleculeNet. It contains data on various compounds tested for BACE-1 inhibition. The dataset is processed to extract molecular descriptors and fingerprints necessary for building the predictive model.

## Usage
### Exploratory Data Analysis (EDA)
The project includes scripts to perform exploratory data analysis on the BACE dataset. EDA provides insights into the distribution of molecular properties, the correlation between features, and the overall quality of the data.

Tools used: pandas, seaborn, matplotlib

### Molecular representations
This project implements multiple molecular representations to enhance model accuracy:

Molecular Fingerprints: These are binary vectors representing the presence or absence of particular substructures within the molecule.

Graph Representations: Molecules are represented as graphs where atoms are nodes and bonds are edges.

Tanimoto Similarity: A measure of similarity between two molecules based on their fingerprint representation.

Tools used: rdkit, networkx

### Model training
The core of this project is the deep neural network model for bioactivity prediction. The model is built using tensorflow and deepchem, and it incorporates:

-L1 and L2 Regularization: To prevent overfitting, L1 and L2 regularization techniques are applied.
-Training and Validation: The model is trained on a subset of the data, and its performance is validated on a separate validation set.

### Hyperparameter optimization
Hyperparameter tuning is performed to identify the best set of parameters for the model. Techniques like grid search or random search are implemented to optimize:

-Learning rate
-Batch size
-Number of layers and neurons
-Regularization coefficients

### Evalution
The model's performance is evaluated using metrics such as Mean Squared Error (MSE) and R-squared (R²). These metrics provide a comprehensive understanding of how well the model predicts bioactivity.
