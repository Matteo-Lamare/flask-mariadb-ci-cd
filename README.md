
# Flask MariaDB Application

## Description

Application web développée avec Flask et Python.
Elle vérifie la connexion à une base de données MariaDB
et affiche son état sur la page d'accueil.

## Technologies

- Python 3.13
- Flask 3.1.3
- PyMySQL 1.2.4
- MariaDB
- Docker

## Installation

Cloner le dépôt :

```bash
git clone https://github.com/Matteo-lamare/flask-mariadb-ci-cd
cd flask-mariadb-ci-cd
```

Créer un environnement virtuel :

```bash
python -m venv venv
```

Activer l'environnement virtuel :

Linux / macOS :

```bash
source venv/bin/activate
```

Windows :

```bash
venv\Scripts\activate
```

Installer les dépendances :

```bash
pip install -r requirements.txt
```

## Configuration

Configurer les variables d'environnement :

```bash
export DB_HOST=localhost
export DB_USER=root
export DB_PASSWORD=your_password
export DB_NAME=test
```

## Démarrage

Lancer l'application :

```bash
python app.py
```

Ouvrir dans le navigateur :

http://localhost:5000

## Résultat attendu

Si la connexion à MariaDB fonctionne :

Database Connection Status: Connected

Sinon :

Database Connection Status: Disconnected

## Docker

Construire l'image :

```bash
docker build -t flask-mariadb-ci-cd .
```

Lancer le conteneur :

```bash
docker run -p 5000:5000 flask-mariadb-ci-cd
```

Test de protection de la branche main.
