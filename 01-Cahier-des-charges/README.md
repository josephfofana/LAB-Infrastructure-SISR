# 01 – Cahier des charges

## LAB-Infrastructure-SISR — UniService

## 1. Présentation de l'entreprise

**UniService** est une PME fictive spécialisée dans les services aux entreprises.

L'entreprise compte environ **20 utilisateurs** répartis dans plusieurs services :

| Service | Utilisateurs |
|---|---:|
| Direction | 2 |
| Administration | 5 |
| Commercial | 6 |
| Informatique | 4 |
| Ressources Humaines | 3 |
| **Total** | **20** |

L'entreprise souhaite disposer d'une infrastructure informatique permettant aux collaborateurs d'accéder aux ressources nécessaires à leur activité tout en assurant une administration centralisée et un niveau de sécurité adapté.

---

# 2. Problématique

L'infrastructure doit permettre de répondre à plusieurs besoins :

- Identifier et authentifier les utilisateurs
- Administrer les comptes de manière centralisée
- Attribuer automatiquement les paramètres réseau
- Permettre la résolution des noms de machines et de services
- Organiser les utilisateurs et les ordinateurs
- Contrôler l'accès aux ressources
- Appliquer des politiques de sécurité
- Faciliter l'administration du parc informatique
- Vérifier le fonctionnement des différents services
- Prévoir des mécanismes de sauvegarde et de continuité
- Documenter les procédures d'administration

---

# 3. Besoins fonctionnels

## 3.1 Authentification

Les utilisateurs doivent pouvoir s'authentifier sur un domaine centralisé.

La solution retenue est :

**Active Directory Domain Services (AD DS)**

Le domaine du laboratoire est :

```text
uniservice.local
