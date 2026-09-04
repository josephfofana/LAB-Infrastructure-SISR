# 02 – Architecture

## LAB-Infrastructure-SISR — UniService

## 1. Architecture du laboratoire

Cette section présente l'architecture générale du laboratoire **LAB-Infrastructure-SISR — UniService**.

L'objectif est de définir l'organisation des machines virtuelles, du réseau et des principaux services de l'infrastructure.

---

## 2. Virtualisation

Le laboratoire utilise **VirtualBox** comme hyperviseur.

Les principales machines virtuelles prévues sont :

* DC1 — Windows Server
* DC2 — Windows Server
* Windows Client
* Linux Server

---

## 3. Réseau

Les machines virtuelles utilisent un **réseau interne** afin d'isoler le laboratoire du réseau réel.

Le réseau permet aux différentes machines de communiquer entre elles et d'utiliser les services nécessaires à l'infrastructure.

---

## 4. Windows Server

Le serveur **DC1** constitue le serveur principal de l'infrastructure.

Il assure notamment :

* Active Directory
* DNS
* DHCP
* Gestion du domaine

Un second serveur **DC2** est prévu afin d'étudier la redondance et la continuité des services.

---

## 5. Linux Server

Le serveur Linux est intégré à l'environnement afin de développer les compétences d'administration Linux.

Il pourra notamment être utilisé pour :

* L'administration système
* Les services réseau
* SSH
* Les tests
* La supervision
* L'automatisation

---

## 6. Domaine

Le domaine Active Directory utilisé dans le laboratoire est :

`uniservice.local`

---

## 7. Architecture logique

```text
                         Réseau interne
                              │
              ┌───────────────┼───────────────┐
              │               │               │
             DC1             DC2        Windows Client
              │
        ┌─────┼─────┐
        │     │     │
       AD    DNS   DHCP
              │
              │
         Linux Server
```

---

## 8. État

| Élément                         | État        |
| ------------------------------- | ----------- |
| VirtualBox                      | 🟢 Terminé  |
| Réseau interne                  | 🟡 En cours |
| Architecture générale           | 🟡 En cours |
| DC1                             | 🟡 En cours |
| DC2                             | 🔵 Prévu    |
| Windows Client                  | 🟡 En cours |
| Linux Server                    | 🟡 En cours |
| Domaine `uniservice.local`      | 🟡 En cours |
| Services réseau                 | 🟡 En cours |
| Documentation de l'architecture | 🟡 En cours |
