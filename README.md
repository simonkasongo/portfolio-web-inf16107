# 🌐 Portfolio Web – Site Statique Multi-pages

> **Cours :** INF16107 – Introduction à l'Internet | **Université du Québec à Rimouski (UQAR) – Campus de Lévis**
> **Session :** Automne 2023 | **Équipe :** Simon Kasongo Musangu & Parfait Nansi Sinkam

---

## 🎯 Aperçu du projet

Site web **statique multi-pages** de type portfolio personnel, conçu et développé dans le cadre du **Travail Pratique 1 (TP1)** du cours d'introduction à l'Internet. Le projet démontre une maîtrise complète du développement front-end sans framework JavaScript, en utilisant uniquement **HTML5**, **CSS3** et le **système de grille Bootstrap 5**.

---

## 📋 Objectifs pédagogiques (travail demandé)

Le professeur demandait de réaliser un site web de portfolio personnel comprenant :

| Exigence | Description |
|---|---|
| **4 pages HTML** | Accueil, Projets, Compétences, Contact |
| **Bootstrap 5 (grille uniquement)** | Utiliser *exclusivement* le système de grille – aucun autre composant Bootstrap |
| **Font Awesome** | Utilisation d'un pack d'icônes SVG |
| **Navigation fonctionnelle** | Menu reliant toutes les pages entre elles |
| **Page Projets** | Galerie avec images, descriptions et **liens** vers chaque projet |
| **Page Contact** | Formulaire avec **validations HTML5** + carte **Google Maps via `<iframe>`** |
| **Qualité du code** | Structure propre, CSS externe, organisation en dossiers |

---

## 🛠️ Technologies utilisées

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="40" title="HTML5"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="40" title="CSS3"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" width="40" title="Bootstrap 5"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="40" title="Git"/>
</p>

- **HTML5** – Structure sémantique des pages (`<nav>`, `<main>`, `<footer>`, `<section>`, `<iframe>`)
- **CSS3** – Feuilles de style externes personnalisées (une par page), flexbox, hover effects
- **Bootstrap 5** – Système de grille responsive (`container-fluid`, `row`, `col-*`) uniquement
- **Font Awesome 6** – Icônes vectorielles (FontAwesome CDN)
- **Devicons CDN** – Logos officiels SVG des technologies (compétences)
- **Google Maps Embed API** – Intégration cartographique via `<iframe>`

---

## 📁 Structure du projet

```
portfolio-web/
│
├── home.html          # Page d'accueil – présentation des membres
├── projects.html      # Page des projets – galerie avec liens
├── skills.html        # Page des compétences – logos officiels
├── contact.html       # Page de contact – carte + formulaire validé
│
├── css/
│   ├── home.css       # Styles page d'accueil
│   ├── projects.css   # Styles page des projets
│   ├── skills.css     # Styles page des compétences
│   └── contact.css    # Styles page de contact
│
└── img/
    ├── logo.jpg       # Logo du portfolio (navbar)
    ├── PXL_*.jpg      # Photo membre 1
    ├── 0dcc*.jpg      # Photo membre 2
    └── projet.png     # Image de projet
```

---

## 🧩 Compétences démontrées

### ✅ HTML5
- Utilisation correcte des **balises sémantiques** : `<nav>`, `<main>`, `<footer>`, `<article>`, `<h1>`–`<h3>`, `<p>`, `<ul>`, `<li>`
- **Formulaire complet** avec types de champs variés : `text`, `email`, `radio`, `select`, `textarea`
- **Validations HTML5 natives** : `required`, `minlength`, `maxlength`, `type="email"` (validation de format automatique)
- Intégration d'une **carte Google Maps** via `<iframe>` avec attributs `allowfullscreen`, `loading="lazy"`, `referrerpolicy`
- **Liens hypertextes** internes (navigation entre pages) et externes (`target="_blank"`)
- Attributs d'accessibilité : `alt`, `title`, `lang="fr"`

### ✅ CSS3
- **Architecture multi-fichiers** : une feuille de style par page (séparation des responsabilités)
- **Flexbox** : mise en page de la navbar, du footer, des cartes, du formulaire
- **Variables CSS** (`:root`) pour une palette de couleurs centralisée
- **Pseudo-classes** : `:hover`, `:focus`, `:invalid` pour les interactions utilisateur
- **Transitions CSS** : effets visuels sur hover (arrondi d'image, couleur de bordure)
- Mise en page responsive avec les **media queries Bootstrap** (`col-12 col-md-6 col-lg-4`)
- Styles de **formulaire personnalisés** : focus, validation visuelle

### ✅ Bootstrap 5 – Système de grille
- Utilisation correcte et **exclusive** du système de grille (contrainte imposée par le professeur)
- Grille fluide avec `container-fluid`, `row`, colonnes `col-12 col-md-4 col-lg-2`
- **Navbar entièrement en CSS pur** (sans composants Bootstrap) pour respecter la contrainte

### ✅ Intégration d'outils tiers
- **Font Awesome 6** via CDN (kit personnalisé) : icônes de navigation, footer, sections
- **Devicons via jsDelivr CDN** : logos SVG officiels des langages (HTML5, CSS3, JS, Python, Java, PHP, Git, Linux, SQL, Bootstrap)
- **Google Maps Embed** : iframe intégré avec coordonnées réelles du campus UQAR Lévis

### ✅ Bonnes pratiques de développement web
- **Séparation structure / présentation** : HTML pour le contenu, CSS pour le style (0 style inline)
- **Organisation en dossiers** : `css/`, `img/` (structure professionnelle)
- **Titres de pages distincts** par `<title>` (SEO de base)
- **Attributs `alt`** sur toutes les images (accessibilité)
- **Liens de navigation actifs** visuellement identifiés (classe `.active`)
- **Formulaire de newsletter** dans le footer sur toutes les pages (cohérence)
- **Liens vers les réseaux sociaux** avec `target="_blank"` et attribut `title`

---

## 📄 Pages du site

### 🏠 Accueil (`home.html`)
- Présentation des deux membres du binôme avec photo et description
- Layout en deux colonnes (grille Bootstrap) : texte gauche, photo droite
- Photo avec effet `border-radius` au survol (transition CSS)

### 🗂️ Projets (`projects.html`)
- Galerie de 3 projets en 3 colonnes
- Chaque carte contient : image, titre, description, **lien cliquable**
- Bouton stylisé "Voir le projet" avec couleur et hover

### ⭐ Compétences (`skills.html`)
- Grille de 10 compétences en 2 rangées
- **Logos officiels SVG** des technologies (via Devicons CDN)
- Effet hover sur les cartes (changement de fond + bordure bleue)

### 📬 Contact (`contact.html`)
- Coordonnées complètes de l'établissement (adresse, téléphone, courriel)
- **Carte Google Maps** intégrée via `<iframe>` (UQAR Campus Lévis)
- Formulaire avec **6 champs** : Nom, Prénom, Genre (radio), Courriel, Fonction (select), Message
- Validations HTML5 : `required`, `minlength`, format email

---

## 🎓 Critères d'évaluation (barème du professeur)

| Critère | Points |
|---|---|
| Les différentes pages (les éléments) | 4.0 |
| L'en-tête (barre de navigation et logo) | 2.5 |
| Le pied de page (newsletter + réseaux sociaux) | 2.5 |
| Inclusion de la carte Google Maps | 1.5 |
| Agencement et disposition des éléments | 3.5 |
| Qualité du code | 3.5 |
| Contenu du rapport et présentation | 1.5 |
| Qualité du français | 1.0 |
| **Total** | **20 points** |

---

## 🚀 Comment ouvrir le projet

Aucune installation requise – ouvrir directement dans un navigateur :

```bash
# Cloner le dépôt
git clone https://github.com/simonkasongo/portfolio-web-inf16107.git

# Ouvrir la page d'accueil
open home.html   # macOS
start home.html  # Windows
```

> **Note :** Une connexion internet est nécessaire pour charger Bootstrap, Font Awesome et les logos Devicons depuis leurs CDN respectifs.

---

## 👥 Auteurs

| Nom | Code permanent |
|---|---|
| **Simon Kasongo Musangu** | KASS27309809 |
| **Parfait Nansi Sinkam** | NANP13299806 |

**Cours :** INF16107 – Introduction à l'Internet  
**Université :** UQAR – Campus de Lévis  
**Session :** Automne 2023

---

*Projet académique réalisé dans le cadre du baccalauréat en informatique à l'UQAR.*
