# **TP 1 Docker**
## 6. Builder une image
c. La procédure est plus facile d'utilisation et ne nécessite pas de reconstruire l'image à chaque changement de fichier. En revanche, le conteneur dépend de fichiers sur le système hôte, ce qui pose des problèmes de portabilité. Si les fichiers locaux sont déplacés, le conteneur ne fonctionne plus. 
La procédure 6 est portable et offre une meilleure gestion des versions. Toutefois, sa configuration est légèrement plus complexe et un temps de construction supplémentaire est nécessaire à chaque modification du contenu.
## 8. Utilisant un fichier docker-compose.yml
a. Le fichier 'docker-compose.yml' permet de définir et de gérer plusieurs conteneurs avec une seule commande.
b. Les variables d'environnement peuvent être spécifiées dans ce fichier, nous permettant ainsi de configurer facilement le conteneur MySQL.
## 9. Observation de l’isolation réseau entre 3 conteneurs
b.
c. Cette configuration est utilisée pour isoler les différentes parties d'une application en fonction de leurs rôles et des besoins en sécurité. Par exemple, pour une application web avec une base de données, le frontend est accessible au public et sert le contenu statique, le backend traite la logique de l'application et son accès est restreint aux utilisateurs internes uniquement, et la base de données stocke les données de l'application et est accessible uniquement par le backend.
