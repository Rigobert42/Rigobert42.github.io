---
title: "AC32.02 — Déployer un réseau d’accès sans fil"
summary: "Déployer un réseau d’accès sans fil pour le réseau d’entreprise en intégrant les enjeux de la sécurité."
date: 2026-04-26
tags:
  - ROM
  - Cyber
  - Apprentissage critique
authors:
  - me
featured: true
status: "Live"
---

## Ce que demande l’apprentissage
Il faut être capable de déployer un réseau Wi-Fi d’entreprise en tenant compte de la sécurité, de l’authentification et de la qualité de service.

## Contexte
Dans mon cas, j’ai travaillé sur une solution Cisco avec controller, dans une logique de déploiement centralisé du Wi-Fi. Le but était d’offrir un accès sans fil propre pour les utilisateurs, tout en gardant un contrôle fort sur l’authentification et sur la séparation des usages. J’ai notamment intégré un serveur RADIUS pour gérer les accès de façon plus sécurisée.

## Réalisation
J’ai d’abord étudié comment organiser les SSID et les profils d’accès selon les besoins des utilisateurs. Ensuite, j’ai configuré la partie controller Cisco pour centraliser la gestion du Wi-Fi et j’ai relié l’authentification à un RADIUS. J’ai aussi vérifié la cohérence entre la segmentation réseau, les règles de sécurité et la manière dont les clients se connectent.

J’ai fait plusieurs tests de connexion pour m’assurer que les équipements se comportaient correctement, que les utilisateurs autorisés pouvaient bien s’authentifier, et que les flux étaient correctement séparés. Je me suis aussi intéressé au comportement du Wi-Fi en mobilité, parce que dans un vrai environnement d’entreprise, les utilisateurs ne restent pas fixes sur un point d’accès.

## Difficultés rencontrées
Le plus compliqué a été de trouver le bon équilibre entre sécurité et simplicité d’utilisation. Si on verrouille trop, l’accès devient pénible pour les utilisateurs. Si on ouvre trop, on perd le contrôle sur le réseau. J’ai aussi vu que la partie sans fil demande beaucoup d’attention sur les paramètres de configuration, car un détail mal réglé peut vite dégrader l’expérience globale.

## Résultats obtenus
À la fin, j’ai réussi à obtenir un réseau Wi-Fi fonctionnel, centralisé et mieux sécurisé. L’authentification via RADIUS m’a permis de voir concrètement l’intérêt d’un contrôle d’accès plus propre qu’un simple mot de passe partagé. J’ai aussi mieux compris comment un controller simplifie l’administration au quotidien.

## Écrit réflexif — modèle de Gibbs
### 1. Description
J’ai déployé un réseau Wi-Fi d’entreprise avec un controller Cisco et une authentification RADIUS.

### 2. Ressenti
Au départ, j’avais une vision assez simple du Wi-Fi, mais j’ai compris que la partie sans fil est très liée à la sécurité et à l’organisation du réseau. J’ai aussi trouvé intéressant de voir que la connexion d’un utilisateur dépend de plusieurs éléments en même temps.

### 3. Analyse
Ce projet m’a appris que le Wi-Fi d’entreprise ne se limite pas à “mettre un point d’accès”. Il faut penser aux profils, à l’authentification, à la séparation des réseaux et à l’administration centralisée. Le RADIUS apporte une vraie logique d’entreprise, parce qu’on contrôle mieux qui a accès à quoi.

### 4. Conclusion
Je retiens que le Wi-Fi doit être conçu comme un service à part entière, pas juste comme un accès annexe. Si je devais refaire le projet, je prendrais encore plus de temps sur la validation des scénarios de connexion et sur les tests de mobilité.

### 5. Plan d’action
Pour progresser, je veux mieux maîtriser les paramètres avancés du controller Cisco, comprendre plus finement les mécanismes d’authentification, et être plus méthodique dans les tests de couverture et de roaming.

## Bilan : **5/5
J’ai appris tout ce qu’il y avait à apprendre sur cet apprentissage critique. J’ai compris comment déployer un réseau Wi-Fi d’entreprise sécurisé avec un controller Cisco et un serveur RADIUS, et j’ai su relier la partie technique aux besoins des utilisateurs. Je considère donc cet apprentissage comme acquis.