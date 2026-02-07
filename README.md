#  Ultimate Password Generator

###  Description
Ce projet est un outil en **Langage C** conçu pour générer des mots de passe à haute sécurité. Contrairement aux générateurs basiques, cet outil maximise la complexité en intégrant des symboles spéciaux et en utilisant le temps système comme source d'aléa (entropie).

###  Fonctionnalités
* **Complexité Maximale :** Inclut majuscules, minuscules, chiffres et symboles (`!@#$%^&*`).
* **Hasard Réel :** Utilisation de `srand(time(NULL))` pour éviter les patterns prévisibles.
* **Interface Colorée :** Sortie console stylisée pour une meilleure expérience utilisateur.
* **Flexible :** Longueur personnalisable selon les besoins de sécurité.

###  Détails Techniques
Le programme utilise l'arithmétique modulaire sur un jeu de caractères étendu :
* **Algorithme :** `index = rand() % charset_length`
* **Bibliothèques :** `stdlib.h`, `time.h`

