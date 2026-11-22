# Personas & User Stories – PlantEvo Viewer

---

## 1. Personas

### Persona 1 – Maêve, 14 ans – Élève de 3e / collégienne curieuse

- **Âge** : 14 ans  
- **Contexte** : Visite scolaire d’une exposition sur l’agriculture et les sciences du vivant.  
- **Objectifs** : Comprendre rapidement pourquoi les plantes sont importantes et comment elles ont évolué, sans lire de longs textes.  
- **Frustrations** : Les sites trop textuels, les termes scientifiques non expliqués, les menus compliqués.  
- **Besoins** : Beaucoup d’images, des textes courts, une navigation claire et un parcours guidé.

### Persona 2 – Konan Florent, 26 ans – Enseignant de SVT / professeur de biologie

- **Âge** : 26 ans  
- **Contexte** : Prépare une séance ou une sortie pédagogique sur l’évolution des plantes.  
- **Objectifs** : Trouver un support clair, scientifiquement correct, utilisable en classe ou en autonomie par les élèves.  
- **Frustrations** : Contenu approximatif, manque de structure chronologique, absence de lien avec le terrain.  
- **Besoins** : Fiabilité des informations, structure progressive (algues → angiospermes), carte de terrain, possibilité de revenir facilement au menu.

### Persona 3 – Koffi Victoire, 27 ans – Visiteuse d’exposition / grand public

- **Âge** : 27 ans  
- **Contexte** : Découvre le stand PlantEvo Viewer lors d’un salon ou d’une journée portes ouvertes.  
- **Objectifs** : Passer un moment agréable, apprendre quelque chose d’intéressant en peu de temps.  
- **Frustrations** : Interfaces surchargées, navigation peu intuitive, contenu trop scolaire.  
- **Besoins** : Design attractif, découverte rapide par les images, possibilité d’approfondir si envie.

### Persona 4 – Anglovia, 22 ans – Apprenant Digital Farming School / futur agronome

- **Âge** : 22 ans  
- **Contexte** : Travaille sur le projet ou l’utilise comme support de révision.  
- **Objectifs** : Relier les connaissances agronomiques (appareil végétatif, reproduction) à une présentation claire.  
- **Besoins** : Exactitude scientifique, distinction claire entre groupes, lien avec la production végétale (graminées, dicotylédones).

---

## 2. User Stories

### Epic 1 – Découverte et navigation

| ID     | User Story                                                                 | Priorité | Critères d’acceptation |
|--------|----------------------------------------------------------------------------|----------|------------------------|
| US-01  | En tant que visiteur, je veux accéder rapidement à une présentation claire du projet afin de comprendre l’intérêt du site. | Haute | La page d’accueil contient un titre fort, un sous-titre explicatif et un bouton « Commencer l’exploration ». |
| US-02  | En tant que visiteur, je veux un menu de navigation visible sur toutes les pages afin de me déplacer librement entre les groupes de végétaux. | Haute | Menu présent sur index + 6 pages thématiques avec liens vers chaque groupe et « Retour au menu ». |
| US-03  | En tant que visiteur, je veux pouvoir revenir facilement à la page d’accueil depuis n’importe quelle page thématique. | Haute | Lien « Retour au menu » fonctionnel sur toutes les pages de détail. |

### Epic 2 – Consultation des contenus pédagogiques

| ID     | User Story                                                                 | Priorité | Critères d’acceptation |
|--------|----------------------------------------------------------------------------|----------|------------------------|
| US-04  | En tant qu’élève, je veux voir principalement des images avec de courts textes afin de rester engagé et de retenir l’essentiel. | Haute | Chaque page thématique contient 4 images + légendes + un bloc d’informations synthétique (≈ 80 % images / 20 % texte). |
| US-05  | En tant qu’enseignant, je veux que chaque groupe présente clairement l’appareil végétatif et le mode de reproduction. | Haute | Bloc « Appareil végétatif » + « Reproduction » présent sur chaque page thématique. |
| US-06  | En tant que visiteur, je veux comprendre la progression évolutive (de l’eau vers la terre, puis les graines et les fleurs). | Haute | Les groupes sont présentés dans un ordre chronologique logique et les dates d’apparition sont indiquées. |
| US-07  | En tant qu’apprenant, je veux des informations biologiquement exactes afin de pouvoir m’y référer en confiance. | Haute | Contenu validé sur les points clés : thalle, cuticule, vaisseaux, pollen, graines nues, fruits, cotylédons, pollinisation. |

### Epic 3 – Lien avec le terrain (SIG)

| ID     | User Story                                                                 | Priorité | Critères d’acceptation |
|--------|----------------------------------------------------------------------------|----------|------------------------|
| US-08  | En tant que visiteur ou enseignant, je veux voir où les observations ont été réalisées afin de faire le lien entre théorie et terrain. | Moyenne | Section « Sur le terrain » avec carte de géolocalisation et crédit de l’auteur. |
| US-09  | En tant qu’apprenant, je veux pouvoir accéder à la carte des positions GPS des espèces observées. | Moyenne | Lien / image « Voir les positions GPS » présent et fonctionnel. |

### Epic 4 – Expérience utilisateur et accessibilité

| ID     | User Story                                                                 | Priorité | Critères d’acceptation |
|--------|----------------------------------------------------------------------------|----------|------------------------|
| US-10  | En tant que visiteur mobile, je veux que le site s’affiche correctement sur mon téléphone. | Haute | Meta viewport présente + CSS responsive. |
| US-11  | En tant que visiteur, je veux une navigation simple et rapide sans avoir besoin de JavaScript. | Haute | Site 100 % HTML/CSS, pas de dépendance JS pour les fonctionnalités de base. |
| US-12  | En tant qu’utilisateur, je veux que le site charge rapidement (images optimisées, CSS léger). | Moyenne | Formats d’image adaptés (webp, jpg, png) et CSS séparé par page. |

---

## 3. Parcours utilisateurs typiques

### Parcours Maêve (élève)
1. Arrive sur la page d’accueil via lien partagé.  
2. Lit le titre et clique sur « Commencer l’exploration ».  
3. Clique sur « Algues » → regarde les images → lit les légendes.  
4. Utilise le menu pour passer aux Mousses, puis Fougères.  
5. Revient au menu et regarde rapidement les Graminés (lien avec l’alimentation).

### Parcours KONAN Florent (enseignant)
1. Ouvre le site pour préparer une séance.  
2. Parcourt l’ensemble des pages pour vérifier l’exactitude scientifique.  
3. Utilise la section « Sur le terrain » pour illustrer le lien observation / théorie.  
4. Propose aux élèves de naviguer librement pendant 10–15 minutes puis de répondre à des questions.

### Parcours KOFFI Victoire (grand public)
1. S’arrête au stand, regarde l’écran ou le tablet.  
2. Clique sur les cartes les plus colorées (Dicotylédones, Algues).  
3. Lit les légendes et le bloc d’informations.  
4. Quitte avec une idée claire : « Les plantes à fleurs sont les plus récentes et les plus évoluées ».

---

## 4. Critères de succès globaux (liés aux user stories)

- Navigation fluide entre tous les groupes.  
- Contenu majoritairement visuel.  
- Exactitude des informations biologiques.  
- Présence d’un retour au menu systématique.  
- Lien avec le terrain (carte GPS).  
- Expérience agréable sur desktop et mobile.
