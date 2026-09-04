# 00 – Projet

## LAB-Infrastructure-SISR — UniService

### 📌 Présentation

**LAB-Infrastructure-SISR** est un laboratoire personnel de mise en pratique consacré à l'administration des systèmes, des réseaux et de l'infrastructure informatique.

Le laboratoire reproduit l'environnement informatique d'une PME fictive nommée **UniService**.

L'objectif est de construire progressivement une infrastructure cohérente, fonctionnelle, sécurisée et documentée, en appliquant les connaissances acquises dans le cadre du **BTS SIO SISR**.

---

## 🏢 Entreprise fictive : UniService

UniService est une PME de services composée d'environ **20 utilisateurs** répartis dans plusieurs services :

| Service             | Nombre d'utilisateurs |
| ------------------- | --------------------: |
| Direction           |                     2 |
| Administration      |                     5 |
| Commercial          |                     6 |
| Informatique        |                     4 |
| Ressources Humaines |                     3 |
| **Total**           |                **20** |

Cette organisation sert de base à la conception de l'infrastructure informatique.

---

## 🎯 Objectifs

Le laboratoire a pour objectifs de :

* Concevoir une infrastructure informatique d'entreprise
* Déployer des systèmes Windows et Linux
* Mettre en place un domaine Active Directory
* Centraliser l'authentification des utilisateurs
* Fournir automatiquement les paramètres réseau
* Assurer la résolution des noms
* Organiser les utilisateurs et les ordinateurs
* Mettre en place des politiques de sécurité
* Contrôler les accès aux ressources
* Tester la connectivité et les services
* Automatiser progressivement certaines tâches
* Documenter les configurations et les procédures

---

## 🖥️ Environnement de laboratoire

Le laboratoire est réalisé dans un environnement virtualisé avec :

**Hyperviseur :**

* VirtualBox

**Systèmes :**

* Windows Server
* Windows Client
* Linux Server

L'environnement est volontairement isolé afin de permettre la réalisation de tests sans impact sur un réseau réel.

---

## 🏗️ Architecture générale

L'infrastructure est construite progressivement autour de plusieurs composants :

```text
                    LAB-Infrastructure-SISR
                              │
                         UniService
                              │
                 ┌────────────┴────────────┐
                 │                         │
          Windows Server              Linux Server
                 │
        ┌────────┼─────────┐
        │        │         │
       AD       DNS       DHCP
        │
       GPO
        │
 Utilisateurs / Ordinateurs
```

---

## 📊 État

| Élément                       | État        |
| ----------------------------- | ----------- |
| Définition du projet          | 🟢 Terminé  |
| Présentation d'UniService     | 🟢 Terminé  |
| Définition des objectifs      | 🟢 Terminé  |
| Définition de l'environnement | 🟢 Terminé  |
| Architecture générale         | 🟡 En cours |
| Infrastructure Windows        | 🟡 En cours |
| Infrastructure Linux          | 🟡 En cours |
| Active Directory              | 🟡 En cours |
| DNS                           | 🟡 En cours |
| DHCP                          | 🟡 En cours |
| Sécurité                      | 🔵 Prévu    |
| Supervision                   | 🔵 Prévu    |
| Automatisation                | 🔵 Prévu    |
| Tests                         | 🔵 Prévu    |
| Documentation                 | 🟡 En cours |
| Bilan du projet               | 🔵 Prévu    |
