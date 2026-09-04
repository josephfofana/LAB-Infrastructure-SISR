# 01 – Cahier des charges

## LAB-Infrastructure-SISR — UniService

## 1. Présentation

Cette section présente le cahier des charges du laboratoire **LAB-Infrastructure-SISR — UniService**.

L'objectif est de définir les besoins de l'entreprise fictive afin de déterminer les fonctionnalités et les services nécessaires à la mise en place de son infrastructure informatique.

---

## 2. Entreprise

UniService est une PME de services composée d'environ **20 utilisateurs** répartis dans plusieurs services :

| Service             | Nombre d'utilisateurs |
| ------------------- | --------------------: |
| Direction           |                     2 |
| Administration      |                     5 |
| Commercial          |                     6 |
| Informatique        |                     4 |
| Ressources Humaines |                     3 |
| **Total**           |                **20** |

---

## 3. Besoins identifiés

L'infrastructure doit permettre :

* L'authentification des utilisateurs
* La gestion centralisée des comptes
* L'attribution automatique des paramètres réseau
* La résolution des noms
* La gestion des postes informatiques
* L'organisation des utilisateurs par service
* La gestion des groupes
* Le contrôle des accès aux ressources
* La sécurisation des systèmes
* La supervision de l'infrastructure
* L'automatisation de certaines tâches
* La réalisation de tests

---

## 4. Services nécessaires

Les principaux services prévus sont :

* Active Directory
* DNS
* DHCP
* Windows Server
* Linux Server
* Services de fichiers
* Services réseau
* Services de supervision

---

## 5. Contraintes

Le laboratoire doit respecter plusieurs contraintes :

* Utilisation d'un environnement virtualisé
* Isolation du réseau de laboratoire
* Utilisation de ressources matérielles limitées
* Possibilité de reproduire les configurations
* Documentation des manipulations
* Possibilité de faire évoluer l'infrastructure

---

## 6. Sécurité

La sécurité doit être intégrée progressivement dans l'infrastructure.

Les principaux éléments étudiés seront :

* Les politiques de mots de passe
* Les groupes de sécurité
* Les permissions
* Les GPO
* Le principe du moindre privilège
* La sécurisation des serveurs
* La surveillance des événements

---

## 7. État

| Élément                          | État        |
| -------------------------------- | ----------- |
| Présentation de l'entreprise     | 🟢 Terminé  |
| Identification des utilisateurs  | 🟢 Terminé  |
| Identification des besoins       | 🟢 Terminé  |
| Identification des services      | 🟡 En cours |
| Identification des contraintes   | 🟢 Terminé  |
| Besoins de sécurité              | 🟡 En cours |
| Besoins de supervision           | 🔵 Prévu    |
| Besoins d'automatisation         | 🔵 Prévu    |
| Validation du cahier des charges | 🟡 En cours |
