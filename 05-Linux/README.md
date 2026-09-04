# 05 – Linux

## LAB-Infrastructure-SISR — UniService

## 1. Présentation

Le serveur Linux fait partie de l'infrastructure informatique de l'entreprise fictive UniService.

Cette machine virtuelle permet de mettre en pratique l'administration d'un système Linux dans un environnement d'entreprise : configuration du système, gestion des utilisateurs et permissions, administration des services, configuration réseau et sécurisation du serveur.

---

## 2. Serveur

Nom prévu :

`SRV-LINUX`

Le serveur est virtualisé avec VirtualBox.

---

## 3. Compétences travaillées

* Installation d'un système Linux
* Configuration réseau
* Administration en ligne de commande
* Gestion des utilisateurs
* Gestion des permissions
* Gestion des services
* Gestion des paquets
* Analyse des journaux
* Sécurisation du système

---

## 4. Commandes étudiées

Exemples :

```text
ip
ping
ss
systemctl
journalctl
apt
sudo
chmod
chown
ls
cd
cp
mv
rm
```

---

## 5. Configuration réseau

Le serveur Linux doit être intégré au réseau du laboratoire afin de pouvoir communiquer avec les autres machines virtuelles.

Les éléments étudiés comprennent :

* Configuration de l'adresse IP
* Configuration du masque réseau
* Configuration de la passerelle
* Configuration du serveur DNS
* Vérification de la connectivité
* Tests de communication avec les autres machines

---

## 6. Gestion des utilisateurs et permissions

L'administration Linux comprend la création et la gestion des utilisateurs et des groupes.

Les permissions permettent de contrôler l'accès aux fichiers et aux répertoires.

Les éléments étudiés comprennent :

* Utilisateurs
* Groupes
* Permissions
* Propriétaire
* Groupe propriétaire
* Droits de lecture, écriture et exécution
* Utilisation de `sudo`

---

## 7. Gestion des services

Les services Linux sont administrés principalement avec `systemctl`.

Les opérations étudiées comprennent :

* Démarrer un service
* Arrêter un service
* Redémarrer un service
* Vérifier l'état d'un service
* Activer un service au démarrage
* Désactiver un service

---

## 8. Gestion des paquets

La gestion des logiciels repose sur le gestionnaire de paquets du système.

Les opérations étudiées comprennent :

* Recherche de paquets
* Installation
* Mise à jour
* Suppression
* Vérification des paquets installés

Le gestionnaire `apt` est notamment utilisé.

---

## 9. Journaux système

Les journaux permettent d'analyser l'activité et les événements du serveur.

La commande `journalctl` est utilisée pour consulter les journaux du système et des services.

Cette analyse permet notamment de :

* Identifier des erreurs
* Vérifier le fonctionnement d'un service
* Rechercher des événements système
* Participer au diagnostic d'un problème

---

## 10. Sécurisation

La sécurisation du serveur Linux porte notamment sur :

* La gestion des comptes utilisateurs
* Les permissions
* L'utilisation de `sudo`
* La gestion des services
* Les mises à jour du système
* La sécurisation des accès
* La surveillance des journaux

---

## 11. Tests

Les principales vérifications comprennent :

```text
ip
ping
ss
systemctl status
journalctl
```

Ces commandes permettent notamment de vérifier :

* La configuration réseau
* La connectivité
* Les ports et services en écoute
* L'état des services
* Les événements système

---

## 12. État

| Élément              | État        |
| -------------------- | ----------- |
| Installation Linux   | 🟡 En cours |
| `SRV-LINUX`          | 🟡 En cours |
| Configuration réseau | 🟡 En cours |
| Connectivité réseau  | 🔵 Prévu    |
| Utilisateurs         | 🔵 Prévu    |
| Groupes              | 🔵 Prévu    |
| Permissions          | 🔵 Prévu    |
| Services             | 🔵 Prévu    |
| Gestion des paquets  | 🔵 Prévu    |
| Journaux système     | 🔵 Prévu    |
| Sécurisation         | 🔵 Prévu    |
| Tests Linux          | 🔵 Prévu    |

