# Projet de construction d'environnements avec Ansible

## Auteurs
- Daniel Lucas - p2201983

## Commandes pour lancer les playbooks
```sh
ansible-playbook -i inventories/hosts.yaml production.yaml
ansible-playbook -i inventories/hosts.yaml staging.yaml
```

## Description
Ce projet vise à automatiser la création de deux environnements distincts (production et staging) en utilisant Ansible. Les environnements incluent un serveur web (nginx), une base de données (mysql) et PHP. Une page PHP affichant "Hello world!" et établissant une connexion à la base de données est déployée pour vérifier le bon fonctionnement de l'environnement. Les mot de passe sont en dur dans les group_vars car je n'ai pas réussit à mettre en place un vault.