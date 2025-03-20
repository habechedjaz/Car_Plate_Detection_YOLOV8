**Détection de plaques d\'immatriculation européennes avec YOLOv8**

**Description du projet**

Ce projet vise à détecter et lire automatiquement les plaques
d\'immatriculation européennes à partir d\'images en utilisant le modèle
YOLOv8 (YOLO version 8, taille Large). L\'objectif principal est de
fournir une solution robuste et précise pour identifier les plaques
d\'immatriculation dans différents contextes, tels que les systèmes de
surveillance, les parkings intelligents, ou les contrôles automatisés.

**Technologies utilisées**

-   **YOLOv8** : Modèle avancé de détection d\'objets

-   **Roboflow** : Annotation et augmentation de données

-   **Kaggle** : Source originale du dataset

-   **Python** : Langage principal pour l\'implémentation

-   **Jupyter Notebook** : Environnement de développement interactif

**Dataset**

Le jeu de données original a été obtenu sur Kaggle, contenant des images
variées de plaques européennes. Il a été annoté précisément à l\'aide de
l\'outil Roboflow pour assurer une haute qualité d\'apprentissage pour
notre modèle YOLOv8.

**Annotation et Augmentation des Données**

Pour améliorer la robustesse et généraliser le modèle, plusieurs
techniques d\'augmentation des données ont été appliquées via Roboflow,
telles que :

 **Rotation** : Between -15° and +15°

 **Grayscale** : Apply to 25% of images

>  **Brightness** : Between -25% and +25%

 **Blur** : Up to 2.5px

 **Noise** : Up to 1.97% of pixelsCes transformations permettent au
modèle de mieux gérer les situations réelles variées, comme les
changements d\'angle, l\'éclairage différent et les conditions
météorologiques diverses.

**Installation des dépendances**

Pour installer les dépendances nécessaires, utilisez :

pip install ultralytics opencv-python matplotlib numpy

**Utilisation du modèle**

Vous pouvez utiliser le notebook Nat_EU_code_x.ipynb fourni dans ce
repository pour :

-   Charger et préparer les données

-   Entraîner le modèle YOLOv8

-   Évaluer et visualiser les performances du modèle

-   Effectuer la détection de plaques d\'immatriculation sur de
    nouvelles images

**Structure du Repository**

├── Nat_EU_code_x.ipynb

├── data

│ ├── images (dossier d\'images)

│ └── labels (annotations)

└── README.md

**Exemples de Résultats**

Les résultats obtenus montrent une précision élevée, permettant une
détection fiable des plaques d\'immatriculation européennes dans divers
scénarios, même sous conditions difficiles (luminosité variable,
orientation de la caméra, plaques partiellement visibles).
