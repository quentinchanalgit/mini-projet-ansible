# mini-projet-ansible
Mini-projet Easytraining

Ansible est un outil de Redhat qui permet d'automatiser les déploiements.
Attendu de ce mini-projet :

écrire un role ansible et que ce dernier puisse etre appelé dans un playbook 

image 

Dans ce role, il faut installer apache dans un container docker

système utilisé pour le tp : Centos 7 

Un serveur ansible sur Centos 7 va piloter deux machines clients avec des clés en ssh.
établir une communication par échange de clés ssh avec la commande suivante : 

![image](https://github.com/user-attachments/assets/57507225-7ad2-47af-8be5-9a10e277a9c1)

Il faut ensuite utiliser cette commande pour copier le couple de clés vers les deux machines clientes

![image](https://github.com/user-attachments/assets/2d107a4d-5d0f-408d-aedf-ddc18ee3134e)


pour la deuxième machine 

![image](https://github.com/user-attachments/assets/826848de-5b63-486f-86aa-557a0724da77)


créer un répertoir de travail nommé projet-ansible
![image](https://github.com/user-attachments/assets/96254c01-f0aa-4221-8ce5-add360554f67)

Voici les fichiers du projet :

le fichier ansible.cfg contient l'inventaire et également les roles.

le fichier host.yml se compose comme ceci : un groupe prod et un groupe staging 
Ces deux groupes possèdent une machine cliente chacun comme le montre la capture ci-dessous 

![image](https://github.com/user-attachments/assets/a3258aa8-b3a5-4cca-bd38-69d2f2976325)

Le dossier host_vars se compose de deux fichiers :
client1.yml pour l'adresse ip de la machine cliente 1 
client2.yml pour l'adresse ip de la machine cliente 2


Dans le dossier defaults, le fichier main.yml contient les variables par défaut

![image](https://github.com/user-attachments/assets/f6aca608-b27a-4cae-8202-5e1466a4e8e6)



Pour que ansible puisse utiliser docker, nous allons prendre la version la plus récente de python 3












