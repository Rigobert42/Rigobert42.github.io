---
title: "AC32.04 — Permettre aux collaborateurs de se connecter de manière sécurisée"
summary: "Permettre aux collaborateurs de se connecter de manière sécurisée au système d’information de l’entreprise."
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
Cet apprentissage consiste à mettre en place un accès distant sécurisé au système d’information, avec des mécanismes adaptés comme le VPN et le filtrage.

## Contexte
J’ai travaillé sur des solutions d’accès distant basées sur du VPN IPsec et du SSL VPN, en lien avec un pare-feu. L’objectif était de permettre à des utilisateurs de se connecter à distance tout en gardant un niveau de sécurité correct et une gestion claire des droits d’accès. J’ai essayé de penser le besoin comme un vrai cas d’usage d’entreprise : télétravail, accès nomade ou connexion à une ressource interne.

## Réalisation
J’ai mis en place des tunnels VPN en fonction du scénario, puis j’ai configuré le pare-feu pour contrôler ce qui pouvait entrer ou sortir. J’ai vérifié les règles de filtrage, les routes nécessaires, et la cohérence entre l’authentification et les services réellement accessibles. J’ai également testé plusieurs cas de connexion pour voir si les utilisateurs accédaient uniquement à ce qui était prévu.

J’ai dû faire attention à ne pas seulement “faire marcher le VPN”, mais à le faire fonctionner de façon propre et sécurisée. Dans ce cadre, j’ai aussi observé comment les paramètres de chiffrement, de politique de sécurité et de filtrage interagissent entre eux.

## Difficultés rencontrées
La difficulté principale était que le moindre oubli peut casser la connexion ou au contraire ouvrir trop large. Il fallait donc bien comprendre le rôle du pare-feu, des politiques IPsec et SSL, et des routes associées. J’ai aussi vu qu’un VPN peut être techniquement opérationnel tout en restant mal adapté si la sécurité n’est pas bien pensée.

## Résultats obtenus
Au final, j’ai obtenu un accès distant stable et cohérent avec les droits attendus. J’ai mieux compris la différence entre les solutions IPsec et SSL VPN selon le contexte d’utilisation. Ce travail m’a aussi montré qu’un accès distant sécurisé est autant une question de design réseau que de configuration technique.

## Écrit réflexif — modèle de Gibbs
### 1. Description
J’ai configuré des accès distants sécurisés avec VPN IPsec, SSL VPN et pare-feu.

### 2. Ressenti
J’ai trouvé la mise en place intéressante parce qu’elle mélange sécurité et fonctionnement concret. En même temps, j’ai vite vu qu’il fallait être très rigoureux, parce qu’un petit détail peut empêcher toute la connexion.

### 3. Analyse
Ce projet m’a appris qu’un accès distant sécurisé ne se résume pas à créer un tunnel. Il faut gérer l’accès, les règles, les routes, les politiques de sécurité et les besoins réels de l’utilisateur. C’est là que le pare-feu prend une place centrale.

### 4. Conclusion
Je retiens qu’il faut toujours valider le service dans son ensemble et pas seulement la partie tunnel. Si je devais refaire le projet, je structurerais encore mieux mes tests par scénario utilisateur.

### 5. Plan d’action
Pour la suite, je veux mieux maîtriser les différences entre IPsec et SSL VPN, être plus précis sur les règles de filtrage, et gagner en autonomie sur le dépannage des accès distants.

## Bilan : 
5/5 - J’ai appris tout ce qu’il y avait à apprendre sur cet apprentissage critique. J’ai compris comment sécuriser un accès distant avec VPN IPsec, SSL VPN et pare-feu, et j’ai su mettre en place un accès cohérent avec les besoins de l’entreprise. Je considère donc cet apprentissage comme acquis.