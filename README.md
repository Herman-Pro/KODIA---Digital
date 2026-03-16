# KODIA Agency — Site Vitrine

Site vitrine de l'agence web béninoise KODIA, spécialisée dans la création
de sites sur mesure pour les indépendants, PME et startups béninois.

---

## Aperçu

Site one-page responsive construit en HTML / CSS / JS vanilla, sans framework
ni dépendance externe. Conçu mobile-first, structuré autour d'un kit UI
personnel réutilisable.

---

## Structure du projet
```
KODIA---Digital/
│
├── index.html
│
├── assets/
│   ├── css/
│   │   ├── main.css               ← point d'entrée (imports)
│   │   ├── base/
│   │   │   ├── variables.css      ← tokens de design
│   │   │   ├── reset.css          ← neutralisation navigateur
│   │   │   ├── typography.css     ← styles typographiques
│   │   │   └── helpers.css        ← classes utilitaires
│   │   ├── components/
│   │   │   ├── buttons.css
│   │   │   ├── cards.css
│   │   │   ├── forms.css
│   │   │   ├── header.css
│   │   │   └── footer.css
│   │   ├── layout/
│   │   │   ├── container.css
│   │   │   ├── grid.css
│   │   │   └── section.css
│   │   └── patterns/
│   │       ├── hero.css
│   │       └── home.css
│   │
│   ├── js/
│   │   ├── menu.js                ← hamburger mobile
│   │   ├── form.js                ← validation + envoi Formspree
│   │   ├── animations.js          ← animations au scroll
│   │   └── main.js                ← lien actif navbar
│   │
│   └── images/
│       ├── Logo_KODIA_sur_fond_blanc.png
│       ├── Logo_KODIA_sur_fond_noir.png
│       └── hero-team.png
│
└── pages/                         ← pages secondaires (à venir)
```

---

## Technologies

- HTML5 sémantique
- CSS3 — Mobile-first, variables CSS, BEM
- JavaScript ES6+ — Vanilla, sans jQuery ni framework
- Flaticon Uicons — icônes via CDN
- Formspree — gestion des soumissions du formulaire

---

## Sections

| Section | Description |
|---|---|
| Hero | Titre + description + CTA + image équipe |
| Nos Services | Aperçu 3 services en cards centrées |
| Pourquoi KODIA | 3 arguments avec checkmarks |
| À Propos | Qui sommes-nous, mission, valeurs |
| CTA Banner | Appel à l'action centré |
| Nos Services (complet) | 4 services en grille 2 colonnes |
| Contact | Formulaire + infos de contact |
| Footer | Logo, liens, contact, copyright |

---

## Kit UI

Ce projet est construit sur un kit UI personnel réutilisable.
Les composants sont indépendants du projet KODIA et peuvent
être réutilisés sur n'importe quel autre projet.

**Layouts disponibles :**
- `.two-col` — 2 colonnes asymétriques (texte + image)
- `.two-col-grid` — 2 colonnes égales (cards)
- `.three-col` — grille 3 colonnes responsive

**Composants disponibles :**
- `.btn`, `.btn--primary`, `.btn--full`
- `.icon-card`, `.icon-card--centered`
- `.info-card`
- `.feature-item`
- `.value-list`
- `.form-group`, `.form-input`, `.form-textarea`
- `.link-underline`, `.link-underline--active`
- `.animate` — animation au scroll via IntersectionObserver

---

## Fonctionnalités JS

- Menu hamburger mobile avec aria-expanded
- Validation formulaire en temps réel (blur + input)
- Envoi formulaire via Formspree avec fetch()
- Notification succès / erreur après soumission
- Animations au scroll avec IntersectionObserver
- Lien navbar actif selon la section visible

---

## Démarrage

Aucune installation requise. Ouvrir `index.html` dans un navigateur
ou lancer un serveur local :
```bash
# Avec VS Code Live Server
# Clic droit sur index.html → Open with Live Server
```

---

## Formulaire de contact

Les soumissions sont gérées par **Formspree**.
Configurer l'endpoint dans `index.html` :
```html
<form action="https://formspree.io/f/TONCODE" method="POST">
```

Et dans `assets/js/form.js` — la fonction `simulateSend`
utilise `fetch()` vers cet endpoint.

---

## Auteur

**KODIA Agency**
Cotonou, Bénin 🇧🇯
kodia.digital@gmail.com