# Optimisation SEO & Structure du projet

## Arborescence du site

```text
/
├── index.html
├── services/
│   ├── creation-jardin-ecologique.html
│   ├── entretien-ecologique.html
│   └── conseil-formation.html
├── realisations/
│   └── index.html
├── blog/
│   └── index.html
├── contact/
│   └── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
└── img/
    └── ...
```

## Points clés de l’optimisation

1. **Utilisation de la sémantique HTML5**  
   - Balises `<section>`, `<header>`, `<main>`, `<footer>`…  
   - Hiérarchisation des titres (`<h1>` à `<h6>`).

2. **Balises meta & title**  
   - Balises `<meta name="description" …>` et `<title>` uniques pour chaque page.  

3. **Liens internes**  
   - Maillage interne cohérent : liens entre les pages (Services ↔ Blog ↔ Réalisations ↔ Contact).

4. **Accessibilité & SEO technique**  
   - Attribut `alt` pour toutes les images.  
   - Lazy loading : `loading="lazy"` pour différer le chargement des images.  
   - `srcset` et `sizes` pour adapter la résolution d’images selon l’écran.  
   - Noms de fichiers d’images explicites (ex. `allee-de-jardin-fleurie-400x225.jpeg`).

5. **Données réelles**  
   - Adresse, numéro de téléphone, email : assurent la crédibilité et favorisent le SEO local.

6. **Fichiers auxiliaires**  
   - `robots.txt` : gestion de l’indexation par les robots des moteurs de recherche.
   - `sitemap.xml` : liste de toutes les URLs du site pour une meilleure indexation.

7. **Nom de domaine & HTTPS**  
   - Utilisation d’un **domaine sécurisé** (HTTPS).  
   - Exemple de sous-domaine pour des questions de budget :  
     [https://maison-verte.infinityfreeapp.com](https://maison-verte.infinityfreeapp.com)
