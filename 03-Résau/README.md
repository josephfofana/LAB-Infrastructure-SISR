# 03 – Réseau

## LAB-Infrastructure-SISR — UniService

## 1. Présentation

Cette section présente la conception et la configuration réseau du laboratoire UniService.

L'objectif est de permettre aux différentes machines virtuelles de communiquer entre elles et d'obtenir automatiquement les paramètres nécessaires à leur fonctionnement.

Le réseau est conçu pour reproduire une infrastructure d'entreprise tout en restant isolé de l'environnement réel.

---

# 2. Technologie de virtualisation réseau

Le laboratoire utilise **VirtualBox** comme hyperviseur.

Le réseau des machines virtuelles repose sur le mode :

**Réseau interne**

Ce mode permet aux machines virtuelles appartenant au même réseau interne de communiquer entre elles sans exposer directement le laboratoire au réseau réel.

### Objectifs

- Isoler le laboratoire
- Permettre la communication entre les VMs
- Tester les services réseau
- Éviter d'interférer avec le réseau réel

---

# 3. Plan d'adressage IPv4

Le laboratoire utilise un réseau IPv4 privé.

```text
Réseau : 192.168.1.0/24
Masque : 255.255.255.0

---

# 4. DHCP

Le service DHCP est utilisé afin d'attribuer automatiquement les paramètres réseau aux machines du laboratoire.

Le serveur DHCP est hébergé sur **DC1**.

### Configuration prévue

```text
Réseau : 192.168.1.0/24
Plage DHCP : 192.168.1.100 → 192.168.1.200
```

Les principaux paramètres étudiés sont :

* Étendue DHCP
* Plage d'adresses
* Exclusions
* Réservations
* Durée des baux
* Passerelle
* Serveur DNS

### Durée du bail

Une durée de bail de **7 jours** est retenue pour le laboratoire.

Ce choix permet de conserver une adresse IP suffisamment longtemps pour éviter des renouvellements trop fréquents, tout en permettant au DHCP de récupérer progressivement les adresses qui ne sont plus utilisées.

---

# 5. DNS

Le service DNS permet d'assurer la résolution des noms dans l'infrastructure UniService.

Le DNS est hébergé sur **DC1** et est intégré à Active Directory.

Il permet notamment :

* La résolution du domaine `uniservice.local`
* La résolution des noms des machines
* La localisation des services du domaine
* La communication entre les différents systèmes

---

# 6. Tests réseau

Différents outils seront utilisés afin de vérifier le fonctionnement du réseau.

### Commandes Windows

```text
ipconfig
ipconfig /all
ping
tracert
nslookup
arp -a
netstat -an
```

Ces commandes permettent notamment de vérifier :

* La configuration IP
* L'adresse attribuée par DHCP
* La connectivité
* La résolution DNS
* Les communications réseau
* Les connexions et ports utilisés

---

# 7. État

| Élément                 | État        |
| ----------------------- | ----------- |
| VirtualBox              | 🟢 Terminé  |
| Réseau interne          | 🟢 Terminé  |
| Plan d'adressage IPv4   | 🟢 Terminé  |
| Réseau `192.168.1.0/24` | 🟢 Terminé  |
| DHCP                    | 🟡 En cours |
| Étendue DHCP            | 🟡 En cours |
| Plage DHCP              | 🟡 En cours |
| Durée du bail           | 🟢 Terminé  |
| Réservations DHCP       | 🔵 Prévu    |
| DNS                     | 🟡 En cours |
| Tests de connectivité   | 🟡 En cours |
| Tests DNS               | 🔵 Prévu    |
| Analyse réseau          | 🔵 Prévu    |


