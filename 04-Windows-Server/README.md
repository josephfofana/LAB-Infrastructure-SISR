# 04 – Windows Server

## LAB-Infrastructure-SISR — UniService

## 1. Présentation

Cette section présente la mise en place et l'administration de l'environnement Windows Server de l'infrastructure UniService.

Les services principaux étudiés sont :

- Active Directory Domain Services
- DNS
- DHCP
- Group Policy
- Gestion des utilisateurs
- Gestion des groupes
- Organisation des unités d'organisation (OU)
- Administration centralisée

---

## 2. Domaine Active Directory

Le domaine utilisé dans le laboratoire est :

`uniservice.local`

Le domaine permet de centraliser l'authentification et l'administration des utilisateurs et des ordinateurs.

---

## 3. DC1

DC1 constitue le serveur principal de l'infrastructure Windows.

### Rôles prévus

- Active Directory Domain Services
- DNS
- DHCP

DC1 constitue le point central de gestion du domaine.

---

## 4. Organisation Active Directory

L'organisation de l'annuaire doit refléter la structure de l'entreprise.

Les principales OU prévues sont :

- Direction
- Administration
- Commercial
- Informatique
- Ressources-Humaines

Cette organisation permet notamment de faciliter l'application des stratégies et la gestion des comptes.

---

## 5. Utilisateurs

Les comptes utilisateurs sont créés selon l'organisation de l'entreprise.

Chaque utilisateur dispose d'un compte permettant son authentification sur le domaine.

Les comptes doivent respecter des règles de sécurité adaptées.

---

## 6. Groupes de sécurité

Les groupes permettent de gérer les autorisations plus efficacement.

Le principe retenu est de donner les permissions aux groupes plutôt qu'aux utilisateurs individuellement lorsque cela est pertinent.

---

## 7. GPO

Les Group Policy Objects permettent de centraliser certaines configurations de sécurité et d'administration.

Les GPO pourront notamment être utilisées pour :

- Politiques de mots de passe
- Restrictions utilisateur
- Configuration système
- Paramètres de sécurité
- Configuration des postes

Chaque GPO devra être testée avant d'être considérée comme validée.

---

## 8. DHCP

Le service DHCP permet l'attribution automatique des paramètres réseau aux postes clients.

Le serveur DHCP est prévu sur DC1.

La configuration détaillée est documentée dans :

`03-Reseau`

---

## 9. DNS

DNS est indispensable au fonctionnement du domaine Active Directory.

Le service permet notamment :

- La résolution des noms
- La résolution du domaine
- La localisation des services Active Directory

---

## 10. Tests

Les principales vérifications comprennent :

```text
ipconfig /all
nslookup
ping
whoami
gpupdate /force
gpresult
