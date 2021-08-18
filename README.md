![car-care1](https://user-images.githubusercontent.com/51690586/129973696-5943e04f-8ab5-44ba-9175-939acf67c8b3.png)
# Car-Damage-Toolkit

Car-Damage-Toolkit est une application pour aider les compagnies d'assurances à faire rapidement les constats lors d'accident de véhicule de leurs clients.

En gros l'idée du projet était de faciliter le travail des compagnies d'assurance en cas d'accident de véhicule d'un client. Il suffit d'uploader sur le site les images de la voiture et laisser le reste du travail à l'algorithme qui fait son travail en plusieurs étapes :

- d'abord il utilise du transfer learning en partant du modèle VGG16 pour s'assurer que l'image est bien une voiture
- ensuite via un modèle de regression logistique il vérifie si la voiture est endommagée ou pas
- ensuite il détermine la localisation des dégâts suivant trois classes : Front, Rear, Side
- Enfin il évalue le degré de sévérité des dégâts suivant trois classes : Severe, Moderate, Minor

A la fin un rapport complet de l'état de la voiture est renvoyer à l'utilisateur

L'application est développée en django.

Pour lancer l'application , ouvrez le dossier cardamage dans un terminal et lancez la commande **python manage.py runserver** 

L'application est disponible par défaut sur le port 8000

