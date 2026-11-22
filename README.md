# PlantEvo Viewer

**Projet pédagogique – Digital Farming School**  
Site web statique d’exploration de l’évolution des végétaux.

---

## Description

**PlantEvo Viewer** est une application web statique destinée à la présentation synoptique et interactive de l’évolution de l’appareil végétatif et des modes de reproduction des végétaux.

Le site raconte, à travers six groupes emblématiques, comment les plantes sont passées de l’eau à la terre ferme, ont développé des vaisseaux, des graines puis des fleurs, et sont devenues le moteur de la vie sur Terre.

Il s’agit d’un outil pédagogique conçu pour une exposition sur l’agriculture, à destination du grand public, des élèves et des visiteurs d’un stand.

---

## Groupes de végétaux présentés

| Groupe              | Fichier                  | Points         clés                                      | Apparition approximative |
|---------------------|--------------------------|--------------------------------------------------|--------------------------|
| Algues              | `Algues.html`            | Thalle, vie aquatique, photosynthèse             | > 1 milliard d’années    |
| Mousses             | `Mousse.html`            | Cuticule, stomates, rizhoïdes                    | ≈ 470 Ma – Ordovicien    |
| Fougères            | `Fougère.html`           | Vaisseaux, lignine, racines, spores              | ≈ 430 Ma – Silurien      |
| Conifères           | `Conifère.html`          | Pollen, graines nues, cônes                      | ≈ 370 Ma – Dévonien      |
| Graminés            | `Graminé.html`           | Monocotylédones, pollinisation par le vent       | Angiospermes             |
| Dicotylédones       | `Dicotylédone.html`      | Fleurs colorées, pollinisation par les insectes  | Angiospermes             |

---

## Structure du projet

```
PlantEvo-Viewer/
├── index.html                
├── Algues.html
├── Mousse.html
├── Fougère.html                # Page d’accueil
├── Conifère.html
├── Graminé.html
├── Dicotylédone.html
├── css/
│   ├── style.css             
│   ├── Algue.css
│   ├── Mousse.css               # Styles de la page d’accueil
│   ├── Fougère.css
│   ├── Conifère.css
│   ├── Graminé.css
│   └── Dicotylédone.css
├── image/
│   ├── PlantEvo.png           # Logo
│   ├── Algue_verte.jpg
│   ├── Algue_brune.jpg
│   ├── Algue_rouge.jpg
│   ├── gamete_spore.webp
│   ├── Mousse1.jpg
│   ├── rizhoide.jpg
│   ├── sporophyte.jpg
│   ├── cycle_mouuse.jpeg
│   ├── Fougères1.jpg
│   ├── fougere_arborescente.jpg
│   ├── sores_fougère.webp
│   ├── cycle_fougere.jpeg
│   ├── conifère.jpg
│   ├── cone_femelle.jpg
│   ├── cones_male.jpg
│   ├── cone_aiguille.jpg
│   ├── Graminés1.jpg
│   ├── epillet.jpg
│   ├── maïs.jpg
│   ├── vent_graminé.png
│   ├── Dicotylédones.jpg
│   ├── abeille.jpg
│   ├── tomate.png
│   ├── haricot2.webp
│   └── Carte 1.png            # Carte de géolocalisation
├── README.md
├── RAPPORT.md                 # Rapport technique et agronomique complet
└── USER_STORIES.md            # Personas et user stories
```

---

## Fonctionnalités

- **Page d’accueil** : présentation du projet, intérêt pédagogique et accès aux six groupes de végétaux.
- **Menu de navigation** cohérent sur toutes les pages (liens hypertexte vers chaque groupe + retour au menu).
- **Pages thématiques** : chaque groupe dispose de 4 images illustratives + textes synthétiques (objectif 80 % images / 20 % texte).
- **Bloc d’informations** : appareil végétatif + reproduction pour chaque groupe.
- **Section « Sur le terrain »** : carte de géolocalisation des observations (SIG).
- **Design responsive** via meta viewport et CSS dédié.

---

## Technologies utilisées

- HTML
- CSS (feuilles de style séparées par page)
- Aucun framework JavaScript (site 100 % statique)
- Images optimisées (formats JPG, PNG, WEBP, JPEG)

## Installation et utilisation

1. Cloner ou télécharger le dépôt :
   ```bash
   git clone <url-du-depot>
   cd PlantEvo-Viewer
   ```

   ## Compétences visées (selon le brief)

- C1N1 : Installer et configurer son environnement de travail
- C2N1 : Maquetter des interfaces utilisateur web
- C3N1 : Réaliser des interfaces utilisateur statiques web

### Agronomie
- Évolution des végétaux et physiologie végétale (AG1)
- Comprendre un système de production végétale (AG6)

### SIG & TD
- SIGTD1 : Repérage par GPS

---

## Auteur

Projet réalisé dans le cadre de la formation **Digital Farming School** – 2026.
