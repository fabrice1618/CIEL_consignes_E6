# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Nature du dépôt

Ce dépôt ne contient pas de code : c'est un dossier de documentation pour l'épreuve **E6** (projet) du BTS CIEL option A (Informatique et Réseaux), année 2 (apprentis). Il n'y a ni build, ni lint, ni tests. Le contenu est en français.

## Fichiers

- `consignes.md` : consignes de l'enseignant aux étudiants (calendrier des livrables, règles de format, conseils). Source de vérité pour les contraintes de rendu.
- `evaluation_projet.md` : grille d'évaluation de la **fiche de présentation** du projet (phase préliminaire, pas le rapport final). Notée par compétence : C01 (communiquer), C03 (gérer un projet), C08 (coder), C10 (exploiter un réseau). Elle sert aussi de prompt d'évaluation.
- `fiche présentation projet e6-ir apprentissage.docx` : modèle officiel de la fiche. Le `.md` du même nom en est une conversion brute (faite avec un script Python, pas pandoc, qui n'est pas installé) ; les images, en-têtes et pieds de page sont perdus.
- `grille_auto_eval-1.pdf` : grille d'auto-évaluation.
- `exemples_presentation/` : fiches d'étudiants d'années précédentes, en PDF. Ce dossier est dans `.gitignore` ; certains fichiers sont en lecture seule et nominatifs, ne pas les republier ni les citer.

## Règles à respecter pour tout contenu produit pour les étudiants

Elles viennent de `consignes.md` :

- Seuls des fichiers **Markdown versionnés sur GitHub** sont relus. Ne jamais produire de livrable Word ou PowerPoint comme version de référence : les `.docx` et `.pptx` finaux sont générés à partir du Markdown puis mis en page à la main.
- Les présentations sont au format **Marp** (il existe un skill `marp-export-pdf` pour l'export).
- Schémas modifiables avec **draw.io** ; sinon **mermaid.js** ou **plantUML**.
- Style de rédaction technique, précis, concis et professionnel (pas de style « IA »).
- Les corrections sont consignées dans les issues GitHub.

## Conventions de modification

- Les règles globales de `~/.claude/CLAUDE.md` s'appliquent : modifications partielles par remplacement ciblé (Edit), jamais de réécriture complète, et orthographe, accents et encodage du texte existant inchangés (y compris les fautes d'origine de `consignes.md`).
- Pour convertir un `.docx` : l'extraction se fait en lisant `word/document.xml` (voir ci-dessus), sans pandoc ni python-docx.
