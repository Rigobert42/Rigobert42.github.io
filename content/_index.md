---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

sections:
  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Bonjour, je suis"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "Je peux"
        strings:
          - "configuré et protégé un réseau privé."
          - "configuré un serveur de téléphonie."
          - "développé des sites web."
          - "développé des programmes et application informatiques."
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: Visualiser mes Projets
          url: "#projects"
          icon: arrow-down
        - text: Contact
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]
  
  # Filterable Portfolio - Alpine.js powered project filtering
  - block: portfolio
    id: projects
    content:
      title: "Mes Réalisations"
      subtitle: "Connaissances et projet réalisé"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: Tout
          tag: '*'
        - name: Apprenstissage Critique
          tag: Full-Stack
        - name: Projets en cours
          tag: Frontend
        - name: Pojets en entreprise
          tag: Backend
      default_button_index: 0
      # Archive link auto-shown if more projects exist than 'count' above
      # archive:
      #   enable: false  # Set to false to explicitly hide
      #   text: "Browse All"  # Customize text
      #   link: "/work/"  # Custom URL
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Visual Tech Stack - Icons organized by category
  - block: tech-stack
    id: skills
    content:
      title: "Compétences"
      subtitle: "Mes compétences divisé en plusieurs catégories"
      categories:
        - name: Languages de programmation
          items:
            - name: C
              icon: devicon/c
            - name: JavaScript
              icon: devicon/javascript
            - name: Python
              icon: devicon/python
            - name: HTML/CSS
              icon: /static/uploads/html-css.png
        - name: Réseau
          items:
            - name: Switch
              icon: /static/uploads/switch.png
            - name: Routeur
              icon: /static/uploads/routeur.png
            - name: Pare-feu
              icon: /static/uploads/firewall.png
            - name: TCP/IP
              icon: /static/uploads/tcp-ip.png
        - name: Système d'exploitation
          items:
            - name: Windows
              icon: /static/uploads/windows.png
            - name: Linux
              icon: devicon/linux
        - name: DevOps
          items:
            - name: Docker
              icon: devicon/docker
            - name: Ansible
              icon: devicon/ansible
            - name: VirtualBox
              icon: brands/virtualbox
            - name: Vagrant
              icon: devicon/vagrant
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: Technicien UC et réseaux
          company: Tims Systems
          company_url: ''
          company_logo: ''
          location: Limonest, Rhône, Rhône Alpes Auvergne, France
          date_start: '10-02-2025'
          date_end: ''
          description: |2-
            * Technicien support spécialisé en UC et réseaux, fournissant une assistance technique de haut niveau aux clients.
            * Résolution de problèmes complexes liés aux réseaux, à la téléphonie, et aux systèmes d'information.
            * Assistance à distance et sur site, avec une forte orientation client et une expertise technique approfondie.

    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Recent Blog Posts
  - block: collection
    id: blog
    content:
      title: Recent Posts
      subtitle: 'Thoughts on web development, tech, and more'
      text: ''
      filters:
        folders:
          - blog
        exclude_featured: false
      count: 3
      order: desc
    design:
      view: card
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Contact
      subtitle: "Let's build something amazing together"
      text: |-
        I'm always interested in hearing about new projects and opportunities.
        Whether you're looking to hire, collaborate, or just want to say hi, feel free to reach out!
      email: benoit4dulac@gmail.com
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # CTA Card
  - block: cta-card
    content:
      title: "Mon CV"
      button:
        text: 'Téléchargé'
        url: uploads/resume.pdf
        new_tab: true
    design:
      card:
        # Light mode: soft pastel theme gradient | Dark mode: rich deep gradient
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
