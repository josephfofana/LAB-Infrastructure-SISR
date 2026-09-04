# 06 – Sécurité

## LAB-Infrastructure-SISR — UniService

## 1. Sécurité de l'infrastructure

Cette section regroupe les mesures de sécurité mises en place dans le laboratoire UniService.

L'objectif est de sécuriser progressivement les systèmes, les comptes, les accès et les services de l'infrastructure.

---

## 2. Active Directory

La sécurité du domaine **uniservice.local** repose notamment sur :

* La gestion des comptes utilisateurs
* Les groupes de sécurité
* Les unités d'organisation (OU)
* Les stratégies de groupe (GPO)
* Les politiques de mots de passe
* La gestion des comptes administrateurs
* Le principe du moindre privilège

---

## 3. Sécurité des postes Windows

Les postes clients seront sécurisés à travers :

* Les stratégies de sécurité
* Les GPO
* La gestion des droits utilisateurs
* La limitation des privilèges administrateur
* Les paramètres de sécurité Windows
* La vérification de la configuration du poste

---

## 4. Sécurité Linux

La sécurité du serveur Linux sera basée sur :

* La gestion des utilisateurs
* La gestion des groupes
* Les permissions sur les fichiers et répertoires
* La sécurisation de SSH
* La gestion des services
* Les mises à jour du système
* La consultation des journaux système

---

## 5. Sécurité réseau

Le laboratoire étant isolé, plusieurs éléments seront étudiés :

* Isolation du réseau
* Contrôle des communications
* Segmentation du réseau
* Vérification des ports ouverts
* Identification des services accessibles
* Analyse des flux réseau

---

## 6. Vérifications et tests

Des tests seront réalisés afin de vérifier l'efficacité des mesures de sécurité.

Les vérifications porteront notamment sur :

* Les droits d'accès
* Les permissions
* Les comptes utilisateurs
* Les groupes de sécurité
* Les stratégies appliquées
* Les services actifs
* Les ports ouverts
* Les configurations des systèmes

---

## 7. État

| Élément              | État        |
| -------------------- | ----------- |
| Comptes utilisateurs | 🟡 En cours |
| Groupes de sécurité  | 🟡 En cours |
| GPO                  | 🔵 Prévu    |
| Permissions          | 🟡 En cours |
| Sécurité Windows     | 🔵 Prévu    |
| Sécurité Linux       | 🔵 Prévu    |
| Sécurité réseau      | 🔵 Prévu    |
| Durcissement         | 🔵 Prévu    |
| Tests de sécurité    | 🔵 Prévu    |
