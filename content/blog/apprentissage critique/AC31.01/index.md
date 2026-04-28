---
title: "AC31.01 — Concevoir un projet de réseau informatique d’une entreprise"
summary: "Intégrer les problématiques de haute disponibilité, de QoS, de sécurité et de supervision."
date: 2026-04-26
tags:
  - ROM
  - Administrer les réseaux
  - Apprentissage critique
authors:
  - me
featured: true
status: "Live"
---

## Ce que demande l’apprentissage
Cet apprentissage demande de concevoir une architecture réseau cohérente pour une entreprise, en prenant en compte la disponibilité, la sécurité, la QoS et la supervision.

## Contexte
Dans mon projet, j’ai travaillé sur une infrastructure réseau assez complète avec un routeur, un switch, un pare-feu et du routage dynamique. L’idée était de partir d’un besoin proche d’un environnement d’entreprise réel, avec plusieurs sous-réseaux, des contraintes de filtrage, de priorisation des flux et de continuité de service. J’ai aussi essayé de garder une logique simple à maintenir, parce qu’un réseau trop complexe devient vite difficile à dépanner.

## Réalisation
J’ai commencé par construire le schéma logique de l’infrastructure, puis j’ai défini le plan d’adressage et la répartition des VLAN. Ensuite, j’ai mis en place le routage inter-VLAN, le routage dynamique et les règles de pare-feu pour contrôler les échanges entre les zones. J’ai également travaillé sur la QoS pour prioriser certains flux plus sensibles, et sur des mécanismes de résilience comme VRRP et LACP pour améliorer la disponibilité.

J’ai utilisé principalement du matériel et des fonctionnalités Cisco, avec une logique de configuration progressive : d’abord valider la connectivité de base, ensuite ajouter les services, puis tester les cas d’usage. J’ai aussi supervisé certains éléments du projet avec SNMP et Zabbix afin de vérifier que les services remontaient bien et que l’état des équipements restait correct.

## Difficultés rencontrées
La principale difficulté a été de faire cohabiter plusieurs besoins en même temps : sécurité, performance, disponibilité et simplicité d’administration. Par exemple, quand j’ai ajouté les règles de filtrage et la QoS, il a fallu vérifier que ça ne bloquait pas certains flux utiles ou que cela ne cassait pas la communication entre les VLAN. J’ai aussi dû faire plusieurs essais sur le routage dynamique pour stabiliser le comportement de l’infrastructure.

## Résultats obtenus
À la fin, j’ai obtenu une architecture fonctionnelle, avec un découpage propre des réseaux, un contrôle des flux plus clair et une meilleure lisibilité de l’ensemble. Les tests de connectivité, de routage et de supervision m’ont permis de valider que la structure répondait bien au besoin initial. J’ai aussi mieux compris l’intérêt de documenter chaque étape pour éviter de perdre du temps lors des retours en arrière.

## Écrit réflexif — modèle de Gibbs
### 1. Description
J’ai travaillé sur une infrastructure réseau d’entreprise avec routeur, switch, pare-feu, routage dynamique, QoS, VLAN, VRRP et LACP.

### 2. Ressenti
Au début, j’étais plutôt à l’aise avec la partie configuration de base, mais j’ai vite vu que le plus difficile était de garder une vision globale. Quand on touche à plusieurs technologies en même temps, on peut facilement modifier un paramètre sans voir son impact ailleurs.

### 3. Analyse
Ce projet m’a montré qu’un réseau ne se limite pas à faire passer des paquets. Il faut aussi penser à la stabilité, à la supervision, à la sécurité et à l’exploitation. J’ai compris que les mécanismes comme la QoS ou le routage dynamique doivent être testés dans un ordre logique, sinon on perd vite du temps à chercher d’où vient un problème.

### 4. Conclusion
Je retiens que la conception réseau demande autant de méthode que de technique. Si je refaisais ce projet, je prendrais encore plus tôt l’habitude de documenter chaque choix, chaque test et chaque modification pour mieux suivre l’évolution de l’infrastructure.

### 5. Plan d’action
Pour la suite, je veux mieux structurer mes phases de test, mieux anticiper les impacts des changements, et renforcer ma capacité à justifier les choix techniques devant un besoin d’entreprise.

### Bilan : **5/5
J’ai appris tout ce qu’il y avait à apprendre sur cet apprentissage critique. J’ai compris la logique de conception d’une infrastructure réseau avec routage, sécurité, QoS et supervision, et j’ai su la mettre en pratique dans un contexte concret. Je considère donc cet apprentissage comme acquis.