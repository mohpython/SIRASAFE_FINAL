# SIRASAFE

Nous sommes tous passés par là : un feu passe au vert et la voiture devant vous ne bouge pas.
Ou, un véhicule auparavant banal ralentit soudainement et commence à dévier d'un côté à l'autre.

Lorsque vous dépassez le conducteur fautif, qu'attendez-vous de voir ?
Vous n'êtes certainement pas surpris lorsque vous apercevez un conducteur qui envoie des SMS, apparemment ravi par les médias sociaux,
ou dans une conversation animée à main levée sur leur téléphone.

![modèle](./graph/1.PNG)

Les 10 classes à prévoir sont :

- c0 : conduite normale
- c1 : envoyer des SMS - à droite
- c2 : parler au téléphone - à droite
- c3 : envoyer des SMS - à gauche
- c4 : parler au téléphone - gauche
- c5 : fonctionnement de la radio
- c6 : boire
- c7 : tendre derrière
- c8 : coiffure et maquillage
- c9 : parler au passager

![modèle](./graph/2.PNG)
![modèle](./graph/3.PNG)

### Dépendance

Les principaux packages Python :
- [Opencv](http://opencv.org/)
- [NumPy] (http://www.numpy.org/)
- [TensorFlow](http://tensorflow.org)
- [Keras](https://keras.io)

L'environnement d'exécution est [Jupyter Notebook](https://jupyter.org/install.html).

### Données

L'ensemble de données est fourni par [Kaggle State Farm](https://www.kaggle.com/c/state-farm-distracted-driver-detection/submissions?sortBy=date&group=successful&page=1). Vous pouvez télécharger l'ensemble de données après avoir créé un compte.

Le répertoire doit être nommé "capserver". Sous ce répertoire, il devrait y avoir trois dossiers : "data", "cache", "subm".

Le dossier "data" est utilisé pour le jeu de données. Le cache est créé pour le stockage des poids et des données. Et le fichier de soumission ".csv" sera créé dans le dossier subm.

### Run

Dans la ligne de commande, assurez-vous que vous êtes dans le dossier "capserver", puis exécutez la commande comme ci-dessous :

```bash
jupyter notebook final.ipynb
```

Il démarrera le cahier jupyter et ouvrira le fichier de projet dans votre navigateur

Le temps d'exécution total sera d'environ 12 heures dans le serveur AWS P2.xlarge. Le résultat de l'exécution peut être vu dans le fichier .ipynb.

### Application

L'application de caméra en temps réel est intégrée dans le fichier .py.
