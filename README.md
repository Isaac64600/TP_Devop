# **TP 1 Docker**
## 6. Builder une image
c. La procédure est plus facile d'utilisation et ne nécessite pas de reconstruire l'image à chaque changement de fichier. En revanche, le conteneur dépend de fichiers sur le système hôte, ce qui pose des problèmes de portabilité. Si les fichiers locaux sont déplacés, le conteneur ne fonctionne plus. 
La procédure 6 est portable et offre une meilleure gestion des versions. Toutefois, sa configuration est légèrement plus complexe et un temps de construction supplémentaire est nécessaire à chaque modification du contenu.
## 8. Utilisant un fichier docker-compose.yml
a. Le fichier 'docker-compose.yml' permet de définir et de gérer plusieurs conteneurs avec une seule commande.
b. Les variables d'environnement peuvent être spécifiées dans ce fichier, nous permettant ainsi de configurer facilement le conteneur MySQL.
## 9. Observation de l’isolation réseau entre 3 conteneurs
b. ![Pasted image (5)](https://github.com/Isaac64600/TP_Devop/assets/95350729/69ba7502-fff7-40ad-bf18-526d9051f9b0)
![Pasted image (6)](https://github.com/Isaac64600/TP_Devop/assets/95350729/38306adb-ae0f-468b-899d-698378fad65c)

Ces sections montrent que web est connecté uniquement au réseau frontend et db uniquement au réseau backend, expliquant pourquoi ils ne peuvent pas se pinguer l'un l'autre.


c. Cette configuration est utilisée pour isoler les différentes parties d'une application en fonction de leurs rôles et des besoins en sécurité. Par exemple, pour une application web avec une base de données, le frontend est accessible au public et sert le contenu statique, le backend traite la logique de l'application et son accès est restreint aux utilisateurs internes uniquement, et la base de données stocke les données de l'application et est accessible uniquement par le backend.
