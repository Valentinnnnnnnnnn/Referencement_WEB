# Composition d'une page Web

3 endroits **stratégiques** pour placer les **mots-clés** :
 - **Entete de la page (HEAD)** : Invisible pour l'utilisateur, mais visible pour les moteurs de recherche. Contient les informations sur la page (titre, description, mots-clés).

- **Le corps de la page (BODY)** : Contenu visible pour l'utilisateur.

- **URL** : L'adresse de la page, claire et concise, peut inclure des mots-clés.

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