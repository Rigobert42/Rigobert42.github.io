---
title: Compétences
type: landing
sections:
  - block: features
    content:
      title: Apprentissages Critiques
      text: Portfolio de compétences BUT R&T ROM – S5/S6
      items:

        - name: Configuration VLAN & Routage
          icon: router
          description: |
            ## Compétence
            CCA – Administrer les réseaux et Internet

            ## Apprentissage critique
            Configurer les fonctions de base du réseau local (Ethernet, IPv4, VLANs, routage statique)

            ## Contexte
            Réalisation d’une SAE de conception d’infrastructure réseau pour une PME multi-services nécessitant une segmentation réseau.

            ## Savoirs mobilisés
            VLAN, adressage IPv4, routage inter-VLAN, sécurité réseau de base

            ## Savoir-faire
            Configuration de switches Cisco, création de VLANs, configuration de trunks, routage sur routeur

            ## Savoir-être
            Rigueur, autonomie, travail en équipe, documentation technique

            ## Résultats
            Mise en place d’un réseau segmenté fonctionnel avec communication contrôlée entre services.

            ## Difficultés rencontrées
            Erreurs de configuration trunk et problème de passerelle par défaut.

            ## Solutions apportées
            Analyse des tables MAC, vérification des interfaces, tests ping/traceroute.

            ## Auto-évaluation
            Niveau intermédiaire acquis : autonomie sur la configuration et le dépannage de base.

---

        - name: Déploiement ToIP – 3CX
          icon: phone
          description: |
            ## Compétence
            ROMB – Gérer les communications unifiées

            ## Apprentissage critique
            Administrer un service de téléphonie pour l’entreprise

            ## Contexte
            Mise en place d’un IPBX 3CX dans le cadre d’un projet de téléphonie d’entreprise.

            ## Savoirs mobilisés
            SIP, VoIP, IPBX, QoS, téléphonie sur IP

            ## Savoir-faire
            Installation serveur 3CX, configuration extensions SIP, postes IP, règles d’appels

            ## Savoir-être
            Organisation, communication technique, méthode

            ## Résultats
            Téléphonie interne fonctionnelle avec appels inter-postes et gestion des utilisateurs.

            ## Difficultés rencontrées
            Problèmes NAT et enregistrement SIP.

            ## Solutions apportées
            Vérification des ports, configuration firewall, analyse des logs SIP.

            ## Auto-évaluation
            Bonne maîtrise opérationnelle, besoin d’approfondissement sur la sécurisation avancée.

---

        - name: Automatisation par Script Python
          icon: code
          description: |
            ## Compétence
            CCC – Créer des outils et applications informatiques pour les R&T

            ## Apprentissage critique
            Automatiser l’administration système avec des scripts

            ## Contexte
            Développement d’un script Python pour automatiser la sauvegarde et la supervision de serveurs Linux.

            ## Savoirs mobilisés
            Python, SSH, Linux, scripts d’administration

            ## Savoir-faire
            Développement de scripts, exécution automatisée, génération de logs

            ## Savoir-être
            Analyse, autonomie, amélioration continue

            ## Résultats
            Réduction du temps d’administration manuelle et meilleure traçabilité.

            ## Difficultés rencontrées
            Gestion des erreurs SSH et permissions utilisateurs.

            ## Solutions apportées
            Ajout de gestion d’exceptions et sécurisation des accès.

            ## Auto-évaluation
            Niveau satisfaisant avec capacité à industrialiser des tâches simples.

---
title: "WeatherNow - Real-Time Weather App"
date: 2024-06-10
summary: "Beautiful weather application with real-time data, 7-day forecasts, and interactive maps"
tags:
  - Frontend
  - React
  - API Integration
  - PWA
tech_stack:
  - React
  - TypeScript
  - OpenWeather API
  - Mapbox
  - Tailwind CSS
  - Vite
featured: false
status: "Live"
role: "Solo Developer"
duration: "3 weeks"
team_size: 1
highlights:
  - "PWA with offline support"
  - "5000+ monthly active users"
  - "Lighthouse score: 100"
---

A fast, beautiful weather application that provides real-time weather data, forecasts, and interactive maps. Built as a Progressive Web App with offline support.

## Overview

WeatherNow started as a weekend project to learn PWA development. It evolved into a fully-featured weather app used by thousands of people daily.

## Features

### Weather Data
- **Current Conditions** - Real-time weather for any location
- **7-Day Forecast** - Detailed daily forecasts with hourly breakdown
- **Weather Alerts** - Severe weather notifications
- **Historical Data** - Past weather data and trends

### User Experience
- **Location Detection** - Automatic location based on GPS or IP
- **Search** - Find weather for any city worldwide
- **Favorites** - Save frequently checked locations
- **Units** - Toggle between metric and imperial
- **Dark Mode** - Automatic or manual theme switching

### Progressive Web App
- **Offline Support** - Access cached data without internet
- **Install** - Add to home screen like a native app
- **Fast** - Optimized for performance (Lighthouse 100)
- **Responsive** - Perfect on any device

## Technical Highlights

### Performance
- Achieved **100/100 Lighthouse score** across all categories
- Implemented service workers for offline functionality
- Optimized bundle size: < 150KB gzipped
- Lazy loading for images and components
- Prefetching for instant navigation

### Data Management
- Smart caching strategy with stale-while-revalidate
- Background sync for updated forecasts
- Efficient API usage with request batching
- Local storage for user preferences

### UI/UX
- Smooth animations with Framer Motion
- Interactive weather map with Mapbox
- Weather icons that match current conditions
- Accessible (WCAG AA compliant)

## API Integration

Integrated multiple weather APIs for comprehensive data:

```typescript
// Example: Fetching weather data
const fetchWeather = async (lat: number, lon: number) => {
  const response = await fetch(
    `https://api.openweathermap.org/data/2.5/weather?lat=${lat}&lon=${lon}&appid=${API_KEY}`
  )
  return response.json()
}
```

## Architecture

```
┌─────────────┐     ┌──────────────┐
│  React App  │────▶│ OpenWeather  │
│   (Vite)    │     │     API      │
└──────┬──────┘     └──────────────┘
       │
       │            ┌──────────────┐
       └───────────▶│   Mapbox     │
                    │     API      │
                    └──────────────┘
```

## Challenges

### Challenge: API Rate Limits
**Solution**: Implemented intelligent caching and request batching to stay within free tier limits while maintaining data freshness

### Challenge: Offline Experience
**Solution**: Service workers with cache-first strategy for UI, network-first for data with graceful fallbacks

### Challenge: Performance on Slow Networks
**Solution**: Image optimization, code splitting, and Progressive rendering for instant perceived performance

## Results

- 📈 **Users**: 5000+ monthly active users
- ⚡ **Performance**: 100 Lighthouse score
- 📱 **PWA**: 40% of users installed as app
- 🌍 **Global**: Users from 50+ countries
- ⭐ **Rating**: 4.8/5 average user rating

## Tech Stack

**Frontend**
- React 18
- TypeScript
- Tailwind CSS
- Framer Motion
- Vite (build tool)

**APIs**
- OpenWeather API
- Mapbox GL JS
- IP Geolocation API

**Tools**
- Workbox (PWA)
- React Query (data fetching)
- Zustand (state management)

**Hosting**
- Netlify
- Cloudflare CDN

## Open Source

This project is open source and welcomes contributions!

**License**: MIT  
**GitHub**: [alexjohnson/weather-now](https://github.com/alexjohnson/weather-now)

## Lessons Learned

1. **PWAs are powerful**: Service workers enable app-like experiences on the web
2. **Performance matters**: Users notice and appreciate fast apps
3. **Caching strategy**: Critical for offline support and API cost management
4. **Simplicity wins**: Started with core features, added more based on user feedback

## Future Plans

- [ ] Weather widgets for websites
- [ ] Social features (share weather conditions)
- [ ] Weather photography integration
- [ ] Apple Watch & Android Wear apps
- [ ] Premium features (ad-free, extended forecasts)

---

**Status**: ✅ Live & Maintained  
**Try it**: [weathernow-demo.netlify.app](https://weathernow-demo.netlify.app)  
**GitHub**: [@alexjohnson/weather-now](https://github.com/alexjohnson/weather-now)
