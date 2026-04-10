## TP-01 : Site web de portfolio personnel (HTML5 + CSS3 + Bootstrap 5)

Ce dépôt contient un site web statique réalisé dans le cadre du cours INF16107 - Introduction à l'Internet à l'UQAR (campus de Lévis). Le travail consiste à concevoir un portfolio personnel en équipe de deux, présentant nos compétences, projets et informations de contact.

Le site est composé de quatre pages HTML reliées entre elles par une barre de navigation commune. Chaque page possède sa propre feuille de style CSS. La mise en page repose uniquement sur le système de grille de Bootstrap 5, sans utilisation d'autres composants du framework, ce qui était une contrainte imposée par le professeur.

### Pages

- `home.html` — Présentation des deux membres de l'équipe avec photo et description
- `projects.html` — Galerie de projets avec images, descriptions et liens
- `skills.html` — Grille de compétences avec les logos officiels des technologies
- `contact.html` — Coordonnées, carte Google Maps intégrée via iframe, et formulaire de contact avec validation HTML5

### Technologies

- HTML5 pour la structure des pages
- CSS3 pour la mise en forme (feuilles de style externes, flexbox, effets hover)
- Bootstrap 5, système de grille uniquement (`container-fluid`, `row`, `col-*`)
- Font Awesome pour les icônes
- Google Maps Embed pour la carte sur la page contact

### Structure du projet

```
portfolio-web-inf16107/
├── home.html
├── projects.html
├── skills.html
├── contact.html
├── css/
│   ├── home.css
│   ├── projects.css
│   ├── skills.css
│   └── contact.css
└── img/
```

### Utilisation

Aucune installation requise. Il suffit d'ouvrir `home.html` dans un navigateur. Une connexion internet est nécessaire pour charger Bootstrap, Font Awesome et les logos des technologies depuis leurs CDN.

### Auteurs

Simon Kasongo Musangu (KASS27309809) et Parfait Nansi Sinkam (NANP13299806)

Cours INF16107 — UQAR, Automne 2023
