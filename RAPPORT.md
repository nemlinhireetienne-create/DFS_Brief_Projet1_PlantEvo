# Rapport complet – PlantEvo Viewer

**Projet 1 – Digital Farming School**  
**Période** : 16 – 22 novembre 2026  
**Type** : Projet individuel  
**Durée** : 7 jours  

---

## Table des matières

1. [Introduction et contexte](#1-introduction-et-contexte)
2. [Objectifs du projet](#2-objectifs-du-projet)
3. [Analyse des exigences](#3-analyse-des-exigences)
4. [Conception et architecture](#4-conception-et-architecture)
5. [Réalisation technique](#5-réalisation-technique)
6. [Contenu agronomique – Évolution des végétaux](#6-contenu-agronomique--évolution-des-végétaux)
7. [Lien avec le terrain (SIG)](#7-lien-avec-le-terrain-sig)
8. [Livrables](#8-livrables)
9. [Critères de performance et auto-évaluation](#9-critères-de-performance-et-auto-évaluation)
10. [Conclusion et perspectives](#10-conclusion-et-perspectives)
11. [Annexes](#11-annexes)

---

## 1. Introduction et contexte

Dans le cadre de la formation Digital Farming School, le projet **PlantEvo Viewer** consiste à développer une page web statique destinée à la présentation synoptique et interactive de l’évolution de l’appareil végétatif et des modes de reproduction des végétaux.

Le site s’inscrit dans le contexte d’une exposition sur l’agriculture. Il doit servir d’outil pédagogique pour les visiteurs d’un stand, leur permettant de comprendre comment et pourquoi les végétaux ont colonisé tous les milieux et sont devenus le moteur de la vie sur Terre.

Les apprenants, à la fois développeurs débutants et apprentis agronomes, doivent donc mobiliser des compétences en développement web et en agronomie.

---

## 2. Objectifs du projet

### 2.1 Objectifs fonctionnels (brief)

- Une page d’accueil simple présentant le projet et son intérêt.
- Un menu statique avec des liens hypertexte vers les différents types de végétaux.
- Un lien de retour au menu depuis chaque page de détail.
- Pour chaque type de plante : images illustratives + petits textes explicatifs (objectif **80 % d’images / 20 % de texte**).

### 2.2 Compétences visées

**Développeur Web et Web Mobile DWWM**
- C1N1 : Installer et configurer son environnement de travail
- C2N1 : Maquetter des interfaces utilisateur web ou web mobile
- C3N1 : Réaliser des interfaces utilisateur statiques web ou web mobile

**Agronomie**
- Évolution des végétaux et physiologie des végétaux (AG1)
- Comprendre un système de production végétale (AG6)

**SIG & TD**
- SIGTD1 : Repérage par GPS

---

## 3. Analyse des exigences

### 3.1 Exigences fonctionnelles

| Exigence | Description | Couverture |
|----------|-------------|------------|
| EF1 | Page d’accueil présentant le projet | `index.html` – section hero + « Pourquoi ce projet ? » |
| EF2 | Menu de navigation vers les groupes | Présent sur toutes les pages |
| EF3 | Lien de retour au menu | Classe `.retour` sur chaque page thématique |
| EF4 | Contenu majoritairement image | 4 images + légendes par page thématique |
| EF5 | Textes synthétiques | Blocs « Appareil végétatif » et « Reproduction » |

### 3.2 Exigences non fonctionnelles

- Site 100 % statique (pas de backend).
- Compatible navigateurs modernes.
- Responsive (meta viewport).
- Images optimisées.
- Code commenté et organisé.
- Minimisation des liens externes et de la taille des CSS.

---

## 4. Conception et architecture

### 4.1 Architecture générale

Le site est organisé autour d’une **page d’accueil** (`index.html`) qui sert de point d’entrée et de hub de navigation. Six pages thématiques correspondent aux grands groupes de végétaux choisis pour illustrer la conquête de la Terre par les plantes :

1. Algues  
2. Mousses  
3. Fougères  
4. Conifères  
5. Graminés (monocotylédones)  
6. Dicotylédones  

### 4.2 Structure d’une page thématique

Chaque page suit le même patron :

- **Header** : logo PlantEvo + menu de navigation
- **Main** :
  - Titre principal
  - Paragraphe d’introduction
  - Grille de 4 cartes image (dont une dédiée au cycle ou à un détail clé)
  - Bloc d’informations (appareil végétatif + reproduction)
- **Footer** : titre du projet, sous-titre pédagogique, copyright

### 4.3 Maquette et choix UX

- Navigation horizontale claire et cohérente.
- Cartes cliquables sur la page d’accueil (groupes).
- Priorité visuelle aux images (objectif 80/20).
- Textes courts, en français accessible.
- Ordre chronologique des groupes pour raconter une histoire évolutive.

---

## 5. Réalisation technique

### 5.1 Technologies

- **HTML** sémantique (`header`, `main`, `nav`, `figure`, `figcaption`, `footer`, `section`).
- **CSS** : une feuille de style principale (`style.css`) + une feuille par page thématique pour une maintenance claire et une taille de fichier maîtrisée.
- Aucun JavaScript (respect de la simplicité et de la performance).
- Images en formats optimisés (JPG, PNG, WEBP).

### 5.2 Organisation du code

- Séparation claire contenu / présentation.
- Noms de fichiers cohérents et en français (avec accents gérés).
- Commentaires HTML pour structurer les sections (HEADER, CONTENU PRINCIPAL, FOOTER).
- Classes CSS réutilisables (`.card`, `.info-box`, `.logo`, `.retour`…).

### 5.3 Points techniques notables

- Meta charset UTF-8 et viewport pour le responsive.
- Utilisation de `<figure>` et `<figcaption>` pour associer image et légende de façon sémantique.
- Footer identique sur toutes les pages pour renforcer l’identité du projet.

### 5.4 Difficultés rencontrées et solutions

| Difficulté | Solution apportée |
|------------|-------------------|
| Gestion des accents dans les noms de fichiers | Conservation des accents (Conifère.html, etc.) |
| Équilibre 80 % images / 20 % texte | Limitation volontaire des textes + 4 images par page |
| Cohérence visuelle entre pages | Structure HTML identique + CSS dédiés mais partagés conceptuellement |
| Lien avec le terrain | Section dédiée + image de carte GPS |

---

## 6. Contenu agronomique – Évolution des végétaux

Le fil narratif du site suit la grande histoire de la conquête des continents par les plantes.

### 6.1 Algues (Chlorophytes) – Les premiers végétaux dans l’eau

- **Appareil végétatif** : simple thalle, sans vraies racines, tiges ni feuilles. L’eau soutient et nourrit l’algue.
- **Reproduction** : spores et gamètes libérés dans l’eau, souvent avec alternance de générations.
- **Importance évolutive** : les algues vertes sont les ancêtres des plantes terrestres.
- **Illustrations** : algue verte (ulve), algue brune (laminaire), algue rouge, cycle spores/gamètes.

### 6.2 Mousses (Bryophytes) – La sortie de l’eau

- **Appareil végétatif** : pas de vaisseaux conducteurs → petite taille. Cuticule pour limiter la perte d’eau, stomates (sur le sporophyte), rizhoïdes de fixation.
- **Reproduction** : par spores dispersées par le vent. La fécondation nécessite encore de l’eau (gamètes mâles nageurs).
- **Apparition** : ≈ 470 Ma (Ordovicien).
- **Illustrations** : coussin de mousse, rizhoïdes, sporophyte (soie + capsule), cycle de vie.

### 6.3 Fougères (Ptéridophytes) – Les premières plantes à vaisseaux

- **Appareil végétatif** : vrais vaisseaux conducteurs (lignine), racines, tige (rhizome), grandes feuilles (frondes).
- **Reproduction** : par spores. L’eau reste nécessaire à la fécondation.
- **Apparition** : ≈ 430 Ma (Silurien).
- **Illustrations** : fronde déroulée (crosse), fougère arborescente, sores, cycle spores → prothalle → œuf → fougère.

### 6.4 Conifères (Gymnospermes) – Pollen et graines nues

- **Appareil végétatif** : arbres au bois solide, racines profondes, feuilles en aiguilles, résine protectrice.
- **Reproduction** : pollen transporté par le vent jusqu’à l’ovule. Fécondation indépendante de l’eau. Graine « nue » (non enfermée dans un fruit), souvent portée par des cônes.
- **Apparition des graines** : ≈ 370 Ma (Dévonien).
- **Illustrations** : forêt de conifères, cône femelle, cônes mâles, aiguilles.

### 6.5 Graminés (Monocotylédones – Angiospermes)

- **Appareil végétatif** : racines fasciculées, feuilles longues à nervures parallèles, croissance à la base (résistance au pâturage).
- **Reproduction** : fleurs réduites, pollinisation par le vent, fruit = caryopse (grain).
- **Importance agronomique** : blé, riz, maïs, canne à sucre → base de l’alimentation humaine.
- **Illustrations** : herbe de prairie, épillet, maïs, pollinisation par le vent.

### 6.6 Dicotylédones (Eudicotylédones – Angiospermes)

- **Appareil végétatif** : racine pivotante, feuilles à nervures ramifiées, deux cotylédons dans la graine.
- **Reproduction** : fleurs souvent colorées et parfumées, pollinisation principalement par les insectes (coévolution), double fécondation, fruit qui enferme et disperse les graines.
- **Remarque** : on parle aujourd’hui plutôt d’eudicotylédones.
- **Illustrations** : fleur colorée, abeille, fruit charnu (tomate), graine à deux cotylédons (haricot).

### 6.7 Synthèse évolutive

| Innovation clé              | Groupe associé     | Conséquence majeure                          |
|-----------------------------|--------------------|----------------------------------------------|
| Photosynthèse dans l’eau    | Algues             | Production d’O₂, base des chaînes alimentaires |
| Cuticule + stomates         | Mousses            | Première adaptation à la vie aérienne        |
| Vaisseaux + lignine         | Fougères           | Grande taille possible                       |
| Pollen + graine nue         | Conifères          | Indépendance de l’eau pour la fécondation    |
| Fleur + fruit               | Angiospermes       | Protection et dispersion optimisées des graines |
| Pollinisation animale       | Dicotylédones      | Coévolution plantes-insectes                 |
| Pollinisation anémophile    | Graminés           | Colonisation des milieux ouverts             |

---

## 7. Lien avec le terrain (SIG)

La section « Sur le terrain » de la page d’accueil présente une carte de géolocalisation des différents groupes observés.

- Image : `image/Carte 1.png`
- Légende : « Carte de géolocalisation des différents groupes de l’évolution de la plante »
- Crédit : Carte réalisée par HIRE ETIENNE NEMLIN

Cette partie répond à l’exigence SIGTD1 (repérage par GPS) et permet de relier les connaissances théoriques à des observations concrètes.

---

## 8. Livrables

Conformément au brief :

| Livrable | Description | Statut |
|----------|-------------|--------|
| Code source | Dépôt GitHub contenant l’ensemble des fichiers HTML, CSS et images | Livré |
| Documentation technique | Le présent rapport + README | Livré |
| Contenu agronomique | Description détaillée de l’évolution + illustrations adaptées | Intégré dans le site et le rapport |
| Rapport SIG | Positions des espèces (carte) | Présent dans le site |
| Personas & User Stories | Document dédié | Livré (`USER_STORIES.md`) |

---

## 9. Critères de performance et auto-évaluation

| Critère | Commentaire | Auto-évaluation |
|---------|-------------|-----------------|
| Fonctionnalité et convivialité de l’interface | Navigation claire, retour au menu systématique, parcours logique | Satisfaisant |
| Pertinence et exactitude des données biologiques | Points clés de l’évolution correctement présentés | Satisfaisant |
| Créativité et adaptabilité | Design simple, centré sur les images, accessible | Correct |
| Code commenté et organisé | Structure HTML cohérente, commentaires de section | Satisfaisant |
| Structure et utilisation efficace des balises | HTML sémantique | Satisfaisant |
| Qualité et optimisation des images | Formats adaptés (webp, jpg, png) | À optimiser davantage si besoin |
| Minimisation des liens externes | Aucun CDN, tout en local | Satisfaisant |
| Taille des fichiers CSS | Feuilles séparées par page | Correct |

---

## 10. Conclusion et perspectives

**PlantEvo Viewer** répond aux exigences du brief en proposant un site web statique clair, pédagogique et visuellement orienté, qui raconte l’histoire de la conquête de la Terre par les végétaux.

Le projet a permis de mobiliser simultanément des compétences de développement web front-end et des connaissances agronomiques sur l’évolution et la physiologie des plantes.

### Perspectives d’amélioration

- Ajout d’une frise chronologique interactive (toujours en HTML/CSS pur ou avec un peu de JS).
- Version bilingue (français / anglais).
- Intégration de données GPS plus précises (coordonnées, légendes cliquables).

---

## 11. Annexes

### Annexe A – Liste des pages

- `index.html` – Accueil
- `Algues.html`
- `Mousse.html`
- `Fougère.html`
- `Conifère.html`
- `Graminé.html`
- `Dicotylédone.html`

### Annexe B – Structure des informations par groupe

Chaque page thématique contient :
1. Titre
2. Introduction (1 paragraphe)
3. 4 images avec légendes
4. Bloc « Appareil végétatif »
5. Bloc « Reproduction »

### Annexe C – Références pédagogiques utilisées

- Programme et brief « Brief projet 1 : PlantEvo Viewer » – Digital Farming School
- Connaissances de base en évolution des plantes (Ordovicien → Angiospermes)
- Observations de terrain (carte GPS fournie)

---

**Document rédigé dans le cadre du projet PlantEvo Viewer**  
Digital Farming School – Novembre 2026
