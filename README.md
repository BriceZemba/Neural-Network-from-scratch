# Deep Learning From Scratch: ANN, CNN & RNN

Ce dépôt contient l'implémentation complète, sans frameworks de haut niveau (comme TensorFlow ou PyTorch), des trois architectures fondamentales du Deep Learning. L'objectif est de comprendre l'algèbre linéaire et les algorithmes d'optimisation qui se cachent derrière les neurones artificiels.

## Architectures Implémentées

### 1. Artificial Neural Networks (ANN) - Perceptron Multicouche

* **Concepts** : Dense layers, fonctions d'activation (Sigmoid, ReLU, Softmax).
* **Optimisation** : Descente de gradient stochastique (SGD) et calcul manuel de la perte (Cross-Entropy).
* **Usage** : Classification de données tabulaires.

### 2. Convolutional Neural Networks (CNN)

* **Concepts** : Couches de convolution (kernels/filters), Padding, Stride et Max Pooling.
* **Technique** : Transformation d'images en volumes de caractéristiques spatiales.
* **Usage** : Reconnaissance de formes et classification d'images (ex: MNIST).

### 3. Recurrent Neural Networks (RNN)

* **Concepts** : Cellules récurrentes, état caché (hidden state), gestion des séquences temporelles.
* **Défi** : Implémentation de la **BPTT** (Backpropagation Through Time).
* **Usage** : Analyse de séries temporelles ou prédiction de texte.

## Ce que j'ai appris

* **Calcul des gradients** : Dérivation manuelle des chaînes de gradients pour chaque couche.
* **Initialisation des poids** : Importance des méthodes Xavier/He pour éviter la disparition du gradient.
* **Vectorisation** : Optimisation des calculs matriciels avec NumPy pour traiter des "batches" de données.

## Structure du projet

```text
├── main.ipynb             # Notebook principal avec les implémentations et tests
├── data/                  # Datasets utilisés (MNIST, Fashion-MNIST, etc.)
├── models/                # Sauvegarde des poids entraînés (fichiers .npy)
└── Rapport_Technique.pdf  # Analyse théorique des algorithmes

```

---

## Rapport Technique

Pour comprendre les détails mathématiques de l'implémentation, notamment les équations de mise à jour des poids pour le CNN et la gestion de la mémoire des RNN, consultez le rapport complet :

**[Télécharger le Rapport Technique (PDF)](./rapport_technique.pdf)** 

## Installation

```bash
git clone https://github.com/votre-username/deep-learning-from-scratch.git
pip install numpy matplotlib
jupyter notebook main.ipynb

```
