# Sign-Language-Translator

Ceci est notre traducteur de language des signes en temps réel. 
En exécutant interface.ipynb, une interface se lance pour permettre à l'utilisateur de commencer la détection des signes. Des boutons permettent d'effacer une lettre, de supprimer le texte, d'ajouter un espace et d'arrêter la détection. Lorsque des signes sont reconnus, ils s'affichent sur l'interface. Un dernier bouton permet de générer une voix qui lit le texte qui a été détecté. 

Deux dossiers J et Z correspondent à la base de données de ces lettres qui ne sont pas présentes dans la base de données de Kaggle utilisée pour la Random Forest. Ces dossiers doivent être ajoutés dans le répertoire contenant le reste de la base de données (":C/users/username/.cache/kagglehub/datasets/signnteam/asl-sign-language-pictures-minus-j-z/versions/1/asl_dataset").
L'image Acceuil.png est utilisée pour l'interface comme menu d'acceuil.

Les fichiers random.joblib et asl_model_final.keras correspondent aux modèles de Random Forest et de CNN entraînés pour ne pas perdre de temps pour la détection.
Le fichier randomForest.ipynb contient le pré traitement de la base de données avec Mediapipe, la conversion des coordonnées dans un fichier CSV, l'entraînement du modèle Random Forest ainsi que la détection des signes en temps réel.
Le fichier CNN.ipynb contient l'entraînement du modèle de réseau de neuronnes ainsi que la détection des signes.
Le fichier interface.ipynb récupère les modèles entraînés et lance l'interface et la détection avec deux parties, une pour le CNN et une pour la Random Forest.
