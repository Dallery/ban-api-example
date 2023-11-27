# ban-api-example
Démonstration de l'utilisation de l'[API BAN](https://adresse.data.gouv.fr/api-doc/adresse) (Base Adresse Nationale) pour rechercher des adresses et afficher le résultat sur une carte interactive.

Le fichier [index.html](index.html) contient l'ensemble du code HTML, CSS et JS, mais aussi les données spatiales utilisées pour délimiter la zone de travail, la commune de Villeneuve-d'Ascq.

Dans le champs en dessous de la carte, vous pouvez indiquer une adresse, sans préciser le code postal ni la ville (c'est effectué dans le code pour s'assurer de rechercher des adresses sur la commune uniquement).
En effet, si vous forcez une adresse en dehors de celle-ci, la bibliothèque [Turf.js](https://turfjs.org/) va venir vérifier que les coordonnées retournée par l'API BAN de l'adresse saisie se trouvent bien dans la commune, auquel cas vous aurez un message d'erreur.

Ainsi, en modifier les bonnes portions de code, vous pouvez faire la même chose sur votre commune.

## TODO
- Ajouter la recherche d'une adresse selon des coordonnées acquises en cliquant sur la carte
