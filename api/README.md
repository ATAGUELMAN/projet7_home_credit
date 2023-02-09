# Project - API

API permettant de :
- Charger les données clients
- Charger le modèle de prédiction
- Prédire le scoring d'un client
- Produire les valeurs SHAP pour expliquer la prédiction

## Dépendances
- Flask
- Flask-Cors
- Flask-RESTful
- Pandas
- Pickle
- Numpy
- Shap
- Imblearn

## Routes

### `/`
Cette route renvoie une page d'accueil qui décrit brièvement les fonctionnalités de l'API.

### `/data`
Cette route renvoie les données clients sous forme de dictionnaire en format JSON.

### `/data/client/<client_id>`
Cette route prend en entrée l'ID d'un client et renvoie les données de ce client, sa prédiction et les valeurs SHAP pour expliquer la prédiction. Les données sont renvoyées sous forme de dictionnaire en format JSON.

## Comment utiliser
- Clonez ce repository.
- Installez les dépendances en utilisant `pip install -r requirements.txt`.
- Chargez les données clients dans un fichier csv `data_sample.csv`.
- Chargez le modèle de prédiction dans un fichier pickle `model.pkl`.
- Démarrez le serveur en exécutant `python app.py`.
- Vous pouvez maintenant accéder à l'API en utilisant l'une des routes décrites ci-dessus.

## Déploiment heroku
L'api est accessible à distance via l'url : https://my-app-flask.herokuapp.com/ 
