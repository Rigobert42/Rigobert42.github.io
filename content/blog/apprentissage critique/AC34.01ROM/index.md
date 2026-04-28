---
title: "AC34.01ROM — Administrer/superviser les infrastructures et les services télécom"
summary: "Administrer/superviser les infrastructures et les services télécom"
date: 2026-04-27
tags:
  - ROM
  - Apprentissage critique
  - Portfolio
authors:
  - me
featured: true
status: "Live"
---

## Ce que demande l’apprentissage
Cet apprentissage consiste à administrer et superviser des infrastructures télécom et les services associés.

## Contexte
Dans cette partie, j’ai travaillé sur un environnement plus orienté opérateur et services, avec des éléments comme un pare-feu virtuel, FreePBX, DNS, DHCP et de la supervision. J’ai aussi découvert que certaines logiques opérateur ressemblent à ce qu’on fait en entreprise, mais avec un besoin plus fort de disponibilité, de supervision et de cohérence globale.

## Réalisation
J’ai participé à la mise en place et à l’administration de services réseau et télécom autour d’une architecture virtualisée. J’ai travaillé sur des services comme DNS et DHCP, sur la mise en place d’un pare-feu virtuel, et sur FreePBX pour la partie téléphonie / services unifiés. J’ai aussi surveillé le comportement des services avec des outils de supervision pour vérifier que tout restait joignable et cohérent.

J’ai essayé de garder une logique proche de l’exploitation réelle : vérifier que les services démarrent, que les flux passent correctement, que les clients obtiennent bien leurs paramètres, et que les incidents éventuels remontent rapidement. Cela m’a permis de mieux comprendre le lien entre configuration et supervision.

## Difficultés rencontrées
Le plus compliqué a été de comprendre l’ensemble des dépendances entre les services. Par exemple, un problème de DNS ou de pare-feu peut donner l’impression que plusieurs choses sont cassées alors que la cause est ailleurs. J’ai aussi vu qu’en environnement virtualisé, il faut bien suivre les interfaces, les flux et les services pour ne pas se perdre.

## Résultats obtenus
J’ai réussi à mettre en place un environnement de services plus structuré et plus exploitable. Les tests m’ont permis de vérifier que la distribution des adresses, la résolution de nom et les services de communication répondaient correctement. J’ai aussi mieux compris l’intérêt d’avoir une supervision cohérente plutôt que de réagir seulement quand ça ne marche plus.

## Écrit réflexif — modèle de Gibbs
### 1. Description
J’ai administré des services télécom et réseau dans un environnement virtualisé avec pare-feu, FreePBX, DNS et DHCP.

### 2. Ressenti
Je me suis rendu compte que ce genre d’environnement demande beaucoup de rigueur, parce que plusieurs couches dépendent les unes des autres. C’était intéressant, mais aussi assez exigeant à déboguer.

### 3. Analyse
Ce travail m’a appris que l’administration de services télécom ne consiste pas seulement à installer des briques techniques. Il faut comprendre les relations entre elles, surveiller les dépendances et vérifier en permanence que les services restent opérationnels.

### 4. Conclusion
Je retiens qu’un service mal supervisé peut sembler fonctionnel jusqu’au moment où un incident révèle tout le reste. Si je devais refaire ce projet, je documenterais davantage les dépendances entre chaque composant.

### 5. Plan d’action
Pour la suite, je veux améliorer ma vision globale des services, être plus à l’aise avec les outils de supervision, et mieux anticiper les impacts d’un changement de configuration.

## Bilan : **5/5  
J’ai appris tout ce qu’il y avait à apprendre sur cet apprentissage critique. J’ai compris comment administrer et superviser des infrastructures télécom avec des services comme DNS, DHCP, FreePBX et un pare-feu virtuel. Je considère donc cet apprentissage comme acquis.