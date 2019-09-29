# Perspectives

*Aurélie GALEA, Loïc GARNIER, Pauline SCHMITT et Kaloyan VESELINOV*

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

**Perspectives** est un jeu qui vous permet de vous rendre compte de la multitude de choix à laquelle nous devons faire face au cours d’une vie, et de l’impact que peut avoir Internet dans la prise de décision.

## Table des matières

- [Perspectives](#perspectives)
  - [Table des matières](#table-des-mati%c3%a8res)
  - [Structure du repo](#structure-du-repo)
    - [src](#src)
      - [src/Cartes](#srccartes)
        - [src/Cartes/Templates_arriere](#srccartestemplatesarriere)
        - [src/Cartes/Templates_avant](#srccartestemplatesavant)
        - [src/Cartes/Perspectives_cartes_\*.docx](#srccartesperspectivescartesdocx)
      - [src/Logo](#srclogo)
      - [src/Perspectives_regles_du_jeu.docx](#srcperspectivesreglesdujeudocx)
      - [src/Perspectives_plateau_de_jeu.docx](#srcperspectivesplateaudejeudocx)
    - [pdf](#pdf)
    - [print](#print)
      - [print/Fichiers_individuels_cartes](#printfichiersindividuelscartes)
      - [print/Perspectives_cartes_arriere.pdf](#printperspectivescartesarrierepdf)
      - [print/Perspectives_cartes_avant.pdf](#printperspectivescartesavantpdf)
      - [print/Perspectives_plateau_de_jeu.pdf](#printperspectivesplateaudejeupdf)
      - [print/Perspectives_regles_du_jeu.pdf](#printperspectivesreglesdujeupdf)
  - [Consignes d'impression](#consignes-dimpression)
  - [Consignes de contribution](#consignes-de-contribution)
  - [Crédits](#cr%c3%a9dits)
    - [Crédit logo](#cr%c3%a9dit-logo)

---

## Structure du repo

### src

Le dossier `src` contient toutes les ressources nécessaires pour le jeu dans un format modifiable :
- `.docx` pour les fichiers texte ; ces fichiers ont été créés avec Word 2019, mais vous pourrez les modifier avec LibreOffice ou OpenOffice (le seul risque c'est d'avoir des problèmes de formattage) ;
- `.pdn` pour les fichiers image ; vous pouvez utiliser [Paint.net](https://www.getpaint.net/download.html) pour modifier ces fichiers.

#### src/Cartes

Le dossier `Cartes` contient toutes les cartes du jeu. 

##### src/Cartes/Templates_arriere

Il s'agit des templates utilisés pour les dos des cartes ; il y en a un pour chaque type de carte (voir les règles du jeu pour plus de détails).

##### src/Cartes/Templates_avant

Il s'agit des templates utilisés pour la face avant des cartes. Ce sont des images `.jpg` à intégrer dans les documents word avec un habillage "Derrière le texte".

##### src/Cartes/Perspectives_cartes_\*.docx

Il s'agit des faces avant de toutes les cartes, avec le template intégré. **Toutes les cartes sont au format A7.**

#### src/Logo

Ce dossier contient les différents logos, avec les projets [GIMP](https://www.gimp.org/downloads/) dans le dossier `Projet_GIMP` et les exports dans le dossier `PNG`.

#### src/Perspectives_regles_du_jeu.docx

Il s'agit du livret qui contient les règles du jeu, ainsi que les conséquences possibles des différentes cartes choix (un peu comme dans un livre dont vous êtes le héros).

#### src/Perspectives_plateau_de_jeu.docx

Il s'agit du plateau utilisé pour le jeu.

---

### pdf

Le dossier `pdf` contient un export des différents documents Word utilisés.

---

### print

#### print/Fichiers_individuels_cartes
 
Il s'agit de fichiers d'impression pour chaque type de carte. Puisque les cartes sont au format A7, il y a 8 cartes par page A4.

Pour les dos de cartes, il s'agit d'une matrice complète de 8 dos de cartes A7. Vous pouvez utiliser ce fichier pour imprimer le bon nombre de dos de cartes pour le jeu (par multiples de 8).

#### print/Perspectives_cartes_arriere.pdf

Il s'agit du fichier d'impression pour les dos de cartes (il y a le bon nombre de de pages pour le nombre courant de cartes). Pour générer ce fichier, nous avons utilisé [pdfmerge](https://www.pdfmerge.com/), en mettant le bon nombre de fois chaque fichier de dos de cartes.

#### print/Perspectives_cartes_avant.pdf

Il s'agit du fichier d'impression pour toutes les faces avant des cartes. Pour générer ce fichier, on avons utilisé [pdfmerge](https://www.pdfmerge.com/), en unissant les différents fichiers `_avant.pdf` du dossier `Fichiers individuels`.

#### print/Perspectives_plateau_de_jeu.pdf

Plateau de jeu au format pdf. À imprimer au **format A3**.

#### print/Perspectives_regles_du_jeu.pdf

Règles du jeu. À imprimer au **format A4**.

---

## Consignes d'impression
Les fichiers `Perspectives_cartes_arriere.pdf`, `Perspectives_cartes_avant.pdf` et `Perspectives_plateau_de_jeu.pdf` sont à imprimer en face unique. 
Le fichier `Perspectives_regles_du_jeu.pdf` est à imprimer en recto verso. 
Tous les fichiers sont à imprimer en couleur 

---

## Consignes de contribution

Si vous voulez ajouter/modifier des cartes du jeu, la procédure est la suivante :
- modifier le document Word correspondant dans le dossier `src/Cartes` ;
- exporter ce document en pdf en allant dans **Fichier > Exporter > Créer un document PDF/XPS** (la procédure est disponible [ici](https://support.office.com/fr-fr/article/enregistrer-ou-convertir-au-format-pdf-ou-xps-d85416c5-7d77-4fd6-a216-6f4bf7c7c110?ui=fr-FR&rs=fr-FR&ad=FR) ; vous devez sauvegarder ce nouveau fichier dans le dossier `pdf` ;
- ouvrir ce nouveau fichier pdf avec Acrobat Reader, appuyer sur **Imprimer**, et choisissez une matrice 4 par 2 pages par feuille, avec ordre des pages Horizontal, avec Impression du contour, et Orientation Paysage ; le format de page choisi est A4 ; sauvegarder ce nouveau fichier dans `print/Fichiers_individuels` ; vous pouvez ensuite imprimer uniquement ce nouveau fichier (si vous avez déjà imprimé le reste du jeu) ;
- regénérez les documents d'impression globaux avec [pdfmerge](https://www.pdfmerge.com/).

---

## Crédits

### Crédit logo

Anita Ponne/ Shutterstock (<https://www.shutterstock.com/fr/image-vector/human-brain-creativity-intellect-eps10-vector-201704261>)

