[![Render and Publish](https://github.com/EricMarcon/Memoire_BioGET/actions/workflows/quarto-publish.yml/badge.svg)](https://github.com/EricMarcon/Memoire_BioGET/actions/workflows/quarto-publish.yml)

# Modèle de mémoire BioGET

Modèle de mémoire de stage rédigé avec R et Quarto pour le master BEE BioGET.

## Utilisation

Télécharger le zip : Bouton vert *Code*, choisir *Download zip*.
Le décompresser dans un dossier de travail.
Ouvrir le projet (`memoire_BioGET.Rproj`) avec RStudio.

De préférence : passer le projet sous contrôle de source et le pousser sur GitHub.

## Paramétrage

Le fichier `_quarto.yml` décrit la structure et la forme du mémoire.
Il doit être complété:

- `book:` contient l'essentiel des informations comme le titre, le nom de l'auteur... Suivre les indications données par les commentaires. En particulier:
  - `chapters:` liste les fichiers qui constituent les chapitres du mémoire. Sauf exception, ne pas la modifier.
  - `appendices:` liste des annexes, à adapter.
  - `repo-url:` est l'adresse du dépôt GitHub de votre mémoire.
  - `site-url:` est l'adresse de la page d'accueil de la version HTML du mémoire.
- `lot` et `lof` permettent de produire la liste des tableaux et des figures.

## Couverture

La page de couverture du mémoire est au format Word dans le dossier `couverture`.

Compléter son contenu dans le fichier `couverture.docx` (français) ou `cover.docx` (anglais) et supprimer l'autre fichier et sa version pdf.
Exporter le fichier au format pdf (`couverture.pdf` pour la version française).

## Mémoire en anglais

Penser à modifier `_quarto.yml` si le mémoire est écrit en anglais:

- `pdftitlepage: couverture/cover.pdf`
- `lang: en-EN` ou `en-US` au choix.
- Supprimer l'option spécifique au français:
  - `language:`
    - `crossref-tbl-title: "Tableau"`
