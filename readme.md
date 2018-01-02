# HTML5 Video Player

*par Rémi de Juvigny*

## Inspiration

* **Keyboard shortcuts** are the same as on YouTube:
  * `Space` or `K` to pause
  * `Left` and `right` arrow keys to skip and go back by 5 seconds
  * `J` and `L` to skip and go back by 10 seconds
  * `F` to ~~pay respect~~ toggle fullscreen

* **Design** : Inspired by Microsoft's [Fluent Design System](https://fluent.microsoft.com/), and Apple's QuickTime Player

## Fonctionnalités

* Changer la vitesse de lecture.
* Activer et désactiver la lecture automatique.
* L'icône de volume donne une indication de la valeur de ce réglage.
* Glisser-déposer sur les barres de volume et de temps.
* La barre de contrôles disparaît si la souris est inactive.
* Mode nuit pour réduire la fatigue oculaire. Le fond passe en noir pur (idéal pour les écrans OLED), et un filtre rouge est appliqué pour atténuer la lumière bleue qui nuit au sommeil.
* Paramètres gardés en mémoire : tous les changements faits dans la barre de contrôle sont appliqués lors des futures visites de la page.

## Difficultés

* Obtenir l'effet de l'arrière-plan flouté a posé problème, la propriété `backdrop-filter` n'étant toujours qu'expérimentale.
* Compatibilité : l'usage de la propriété CSS `pointer-events` rend le player incompatible avec les versions d'IE inférieures à 10.
* Débogage : une grande partie du code est dédiée à la prévention de bugs dans des cas d'enchainements d'actions particuliers.