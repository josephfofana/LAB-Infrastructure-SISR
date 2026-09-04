# 02 – Architecture

## LAB-Infrastructure-SISR — UniService

## 1. Présentation

Cette section présente l'architecture technique du laboratoire UniService.

L'infrastructure est réalisée dans un environnement virtualisé avec **VirtualBox**. Elle reproduit progressivement une infrastructure informatique de PME comprenant des serveurs, des postes clients et différents services d'infrastructure.

L'objectif est de construire une architecture cohérente, administrable, sécurisée et évolutive.

---

## 2. Architecture générale

L'infrastructure repose sur plusieurs machines virtuelles ayant chacune un rôle défini.

```text
                         LAB-Infrastructure-SISR
                                  │
                              UniService
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
                  DC1                         DC2
                    │                           │
          ┌─────────┼─────────┐              AD/DNS
          │         │         │
         AD        DNS       DHCP
          │
          │
     ┌────┴─────┐
     │          │
 CLIENT1    Utilisateurs
     │
     │
 SRV-LINUX
