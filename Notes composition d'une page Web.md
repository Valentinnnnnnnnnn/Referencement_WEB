# Composition d'une page Web

## Les mots-clés
3 endroits **stratégiques** pour placer les **mots-clés** :
 - **Entete de la page (HEAD)** : Invisible pour l'utilisateur, mais visible pour les moteurs de recherche. Contient les informations sur la page (titre, description, mots-clés).

- **Le corps de la page (BODY)** : Contenu visible pour l'utilisateur.

- **URL** : L'adresse de la page, claire et concise, peut inclure des mots-clés.

**Indice de densité des mots-clés** : Nombre de fois où un mot-clé apparaît dans le contenu par rapport au nombre total de mots. Il est important de ne pas sur-optimiser (**spamdexing** ou paragraphes trop longs) le contenu, car cela peut être pénalisé par les moteurs de recherche : **blacklisté**, **sandboxé**

En général, il est difficile de d'optimiser une page avec plus de **3 mots-clés**.

Il peut etre utile d'utiliser les mots sous toutes ses formes (pluriel, singulier, conjugaison, etc.).

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale
    <title>Titre de la page</title>
    <meta name="description" content="Description de la page">
    <meta name="keywords" content="mot-clé1, mot-clé2, mot-clé3">
</head>
<body>
    <h1>Titre de la page</h1>
    <p>Contenu de la page</p>
</body>
</html>
```

## La semantique HTML
La semantique HTML permet de structurer le contenu de la page en utilisant des balises sémantiques qui décrivent le rôle des éléments. Cela permet aux moteurs de recherche de mieux comprendre le contenu de la page et d'améliorer le positionnement.

Mdn web docs : https://developer.mozilla.org/fr/docs/Web/HTML/Element

## Les balises
### Head
- Balise **title** : Titre de la page (apparaît dans l’onglet du navigateur et dans les SERP). Il doit contenir les mots-clés principaux et informer l'utilisateur sur le contenu de la page.
    
    Conseils de rédaction : 
    - Clareté et précision
    - Longueur maximale de 50 caractères
    - Inclure le plus de mots-clés possible.
    - Personnaliser le titre de chaque page
    - Essayer de placer les mots-clés principaux au début du titre.
    - Éviter les mots-clés redondants ou trop génériques.

- Balise **meta** : Permet de définir des métadonnées (informations sur la page) qui ne sont pas affichées à l'utilisateur, mais qui sont utilisées par les moteurs de recherche pour indexer la page.
L'évolution des moteurs de recherche a rendu ces balises moins importantes pour le référencement, mais elles restent utiles pour d'autres aspects.
    >Faites les figurer sur toutes les pages en adaptant le contenu.

- Balise **meta description** : Brève description du contenu de la page (affichée dans les SERP). Elle doit être claire, concise, contenir des mots-clés et inciter l'utilisateur à cliquer sur le lien.
    
    Conseils de rédaction : 
    - Longueur maximale de 160 caractères
    - Inclure les mots-clés principaux
    - Personnaliser la description de chaque page
    - Éviter les descriptions trop génériques ou trompeuses.

- Balise **meta keywords** : Liste de mots-clés séparés par des virgules. Elle permettait autrefois d'indiquer les mots-clés principaux de la page, mais elle est aujourd'hui peu utilisée voir ignoré par les moteurs de recherche.

- Balise **meta robots** : Permet de contrôler le comportement des robots d'indexation des moteurs de recherche. Elle peut indiquer aux robots de ne pas indexer la page, de ne pas suivre les liens, etc.
    ```html
    <meta name="robots" content="noindex, nofollow">
    ```
    - **noindex** : Demande aux moteurs de recherche de ne pas indexer la page.
    - **nofollow** : Demande aux moteurs de recherche de ne pas suivre les liens présents sur la page.
    - **nosnippet** : Demande aux moteurs de recherche de ne pas afficher de snippet dans les SERP.
    - **noarchive** : Demande aux moteurs de recherche de ne pas conserver une copie en cache de la page.
    - **unavailable_after** : Indique une date après laquelle la page ne doit plus être indexée

### Les liens
- Balise **a** : Les liens doivent être logiques et clairs (éviter les "voir plus", "cliquez ici", etc.). Ils doivent contenir des mots-clés pertinents pour le référencement.

- Toutes les pages doivent être connectées entre elles pour faciliter la navigation des utilisateurs et des robots d'indexation. Les liens internes permettent de renforcer le mailillage interne.

- Fil d'Ariane : Permet de naviguer facilement entre les différentes pages du site. Chaque page doit contenir un lien cliquable.
Exemple : Accueil > Catégorie > Sous-catégorie > Page

### Les titres
- Balises **h1** à **h6** : Les titres doivent être structurés de manière hiérarchique (h1 pour le titre principal, h2 pour les sous-titres, etc.).

- Balises **strong**, **i**, **b** : Permettent de mettre en valeur certains éléments du texte. Il est recommandé d'utiliser **strong** pour le gras et **i** pour l'italique pour définir ce qui est important.

## Plan de site
Le plan de site est une page qui répertorie l'ensemble des pages du site. Il permet aux utilisateurs et aux robots d'indexation de naviguer facilement entre les différentes pages.

## Les médias
Les navigateurs permettent de se placer à la place d'un utilisateur en simulant une connexion lente ou rapide, un appareil mobile, etc. Cela permet de vérifier la compatibilité du site avec différents appareils et de détecter les problèmes de performance.

### Les images
- Balise **img** : Les images doivent être optimisées pour le web (taille, format, compression). Elles doivent contenir une balise **alt** pour décrire l'image (utile pour le référencement et l'accessibilité). Balise **title** pour ajouter un titre à l'image.
    >Format : PNG, GIF, JPEG ou WebP.
- Taille : Petite (150x150), Moyenne, Grande (à partir de 500x500)

### Les vidéos
- Optimisation SEO : métadonnées, url, bonne qualité
    >Éviter Flash, jQuerry, ect.

### Les fichiers
- **URL** : L'adresse du fichier, claire et concise, peut inclure des mots-clés.
- **Taille** : Limiter la taille des fichiers pour améliorer les performances du site tout en maintenant une qualité optimal.
>Éviter les fichiers editables, les PDF sont préférables

## Robots.txt
Le fichier robots.txt permet de contrôler le comportement des robots d'indexation des moteurs de recherche. Il peut indiquer aux robots de ne pas indexer certaines parties du site, de ne pas suivre les liens, etc.

## Carte Google Maps
La carte Google Maps permet d'afficher l'emplacement de l'entreprise sur le site. Elle peut être intégrée à la page de contact ou à la page d'accueil.