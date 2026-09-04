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
