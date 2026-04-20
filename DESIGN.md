# Okuden — Design System

> Version 1.0

---

## Table des matières

1. [Brand Identity](#1-brand-identity)
2. [Brand Values](#2-brand-values)
3. [Brand Personality](#3-brand-personality)
4. [Color System](#4-color-system)
5. [Typography](#5-typography)
6. [Logo](#6-logo)
7. [Iconography & Visual Elements](#7-iconography--visual-elements)
8. [Voice & Tone](#8-voice--tone)
9. [Assets](#9-assets)

---

## 1. Brand Identity

**Okuden** est un cabinet de conseil Digital & Data, fondé à Paris en 2020
par Aurélien et Arnaud — deux entrepreneurs admirateurs du Japon et de ses valeurs
d'excellence, de sens de l'effort collectif, de pragmatisme et de loyauté.

Le cabinet accompagne les entreprises dans la conception et la mise en œuvre
de leurs projets de transformation, avec une expertise sectorielle affirmée :
Assurance & Services Financiers, Transport & Mobilité, Sport, Esport & Gaming.

### Mission

Aider les entreprises à progresser sereinement dans l'univers toujours en mouvement
du Digital & de la Data — avec anticipation stratégique, rigueur dans l'action
et agilité dans la performance.

### Positionnement

Okuden n'est ni un généraliste, ni un intégrateur.
C'est un cabinet indépendant, pluri-expert, qui intervient comme contre-poids expert
entre les équipes internes et les partenaires technologiques —
pour challenger, cadrer, prioriser, et défendre les intérêts métiers avec exigence.

### Nom

Okuden est un terme issu des arts martiaux traditionnels japonais.
Il désigne un pratiquant expérimenté, à l'avant-dernier niveau du système Menkyo.
Ce degré marque le début du travail véritable — non sa fin.
C'est cette philosophie qui fonde l'ambition du cabinet :
viser et atteindre le niveau supérieur, toujours en quête de l'excellence.

### Produit phare

**Aikoz** — plateforme IA Voice of Customers, développée par Okuden.
Elle transforme les avis clients en levier business pour les grandes marques en réseau.

---

## 2. Brand Values

### Excellence — Maîtrise

Okuden ne survole pas les sujets. Le cabinet s'engage en profondeur,
avec la même exigence que le pratiquant qui affine ses techniques jusqu'au niveau ultime.

> Traduction visuelle : précision géométrique, peu d'éléments mais chacun justifié,
> aucun ornement superflu.

### Pragmatisme — Rationalité

Pas de dogmatisme. Pas de solutions toutes faites.
Les bonnes méthodes, les bons outils, au bon moment — au service d'un résultat mesurable.

> Traduction visuelle : hiérarchie claire, densité d'information maîtrisée,
> grilles rigoureuses.

### Convivialité — Humanité

Les clients disent d'Okuden que ses équipes sont enthousiastes,
et qu'il est très facile de travailler avec elles.
"Work hard, play harder" — l'expertise n'exclut pas la chaleur humaine.

> Traduction visuelle : happy-teal comme accent d'énergie et de bienveillance,
> espaces respirants, ton jamais froid.

---

## 3. Brand Personality

**Archétype principal (70%) : Sage**

Okuden résout les problèmes avec expertise et recul.
Le cabinet apporte de la clarté dans des environnements complexes —
avec des recommandations libres de tout conflit d'intérêt,
fondées sur la connaissance sectorielle et la rigueur analytique.

**Archétype secondaire (30%) : Explorer**

Okuden reste en mouvement. Curieux des nouvelles méthodes,
des nouveaux secteurs, des nouvelles technologies.
Le cabinet explore en permanence pour rester à la pointe —
sans jamais perdre de vue l'impact opérationnel concret.

---

## 4. Color System

### Philosophie

La palette Okuden repose sur trois couleurs de marque,
chacune à rôle défini — primaire, secondaire, accent.
Aucune ne rivalise avec les autres.
Ensemble, elles forment un système sobre, contrasté et cohérent.

Les couleurs sont toujours utilisées à travers les tokens sémantiques.
Les valeurs brutes des primitives ne sont jamais consommées directement en production.

### Couleurs de marque

| Nom           | Hex       | Rôle                                                        |
|---------------|-----------|-------------------------------------------------------------|
| Deep-space-blue | `#002037` | Couleur primaire — identité, navigation principale, hero sections |
| Sky-blue        | `#0270EB` | Couleur secondaire — actions, liens, CTAs, focus ring       |
| Happy-teal      | `#00BAA9` | Accent — highlights, badges, éléments décoratifs, énergie   |

### Règles d'usage

- **Deep-space-blue** structure et ancre — c'est la couleur de la maîtrise.
  Elle domine les surfaces sombres, les en-têtes, les moments de marque forts.

- **Sky-blue** active — c'est la couleur de l'action.
  Boutons primaires, liens, états interactifs, focus ring.
  Ne jamais l'utiliser pour des surfaces larges.

- **Happy-teal** accentue — c'est la couleur de l'énergie et de la chaleur.
  Badges, indicateurs, micro-éléments. Toujours en touches légères.

- **Blanc et neutres** constituent la majorité des surfaces.
  La couleur est réservée aux moments qui le méritent.

### Tokens

Les palettes complètes (teintes 50 à 1000) sont définies dans `primitives.json`.
Les rôles sémantiques (brand, surface, text, border, status) sont dans `semantics.json`.

> Toujours référencer les tokens sémantiques en production.
> Les primitives sont la source de vérité, pas des valeurs à consommer directement.

---

## 5. Typography

### Famille typographique

Okuden utilise une seule famille : **Century Gothic**.

Century Gothic est géométrique, claire et architecturale.
Ses formes circulaires parfaites et ses proportions régulières
évoquent la rigueur sans la froideur — cohérente avec l'identité du cabinet.

```
font-family: "Century Gothic", CenturyGothic, AppleGothic, sans-serif;
```

### Grammages disponibles

| Poids   | Valeur | Usage                                      |
|---------|--------|--------------------------------------------|
| Regular | 400    | Corps de texte, paragraphes, labels légers |
| Bold    | 700    | Titres, labels, emphases, CTAs             |

> Century Gothic ne dispose pas de variante Medium native.
> Ne jamais simuler un poids intermédiaire via l'émulation logicielle (faux gras).
> Utiliser uniquement Regular et Bold.

### Échelle typographique

| Token       | Taille | Usage principal                    |
|-------------|--------|------------------------------------|
| Display     | 72px   | Hero / splash — une seule fois     |
| H1          | 48px   | Titre principal de page            |
| H2          | 36px   | Titre de section                   |
| H3          | 30px   | Titre de sous-section              |
| H4          | 24px   | Titre de carte / panneau           |
| Body lg     | 18px   | Paragraphes d'introduction         |
| Body md     | 16px   | Corps de texte standard            |
| Body sm     | 14px   | Texte secondaire                   |
| Label lg    | 14px Bold | Étiquettes, navigation          |
| Label md    | 12px Bold | Badges, onglets                 |
| Caption     | 12px   | Légendes, horodatages              |

### Règles d'usage

- Tracking serré (`-0.02em`) sur les grands titres — jamais sur le corps.
- Tracking large (`+0.05em`) sur les labels — améliore la lisibilité en petit.
- Hauteur de ligne : `1.5` pour le corps, `1.15` pour les titres.
- Jamais de texte en majuscules complètes sur plus de 3 mots.

---

## 6. Logo

### Philosophie

Le logo Okuden est la marque de la maîtrise.
Il doit toujours apparaître avec clarté, espace et intention.
Jamais compressé, jamais altéré, jamais sur un fond qui nuit à sa lisibilité.

### Versions disponibles

| Version     | Usage principal                                              |
|-------------|--------------------------------------------------------------|
| Horizontal  | Usage standard — en-têtes, documents, supports print        |
| Vertical    | Formats carrés, couvertures, supports événementiels         |
| Symbole     | Favicon, icône app, signature réduite                       |

Chaque version est disponible en deux colorimétries :

| Colorimétrie | Contexte d'usage                                          |
|--------------|-----------------------------------------------------------|
| Blue (dark)  | Sur fond blanc ou clair — usage par défaut               |
| White        | Sur fond deep-space-blue ou toute surface sombre          |

### Zone d'exclusion

La zone d'exclusion autour du logo est égale à la hauteur de la lettre "O" du logotype.
Aucun élément graphique ne pénètre cette zone.

### Ce qu'il ne faut jamais faire

- Modifier les proportions ou étirer le logo
- Appliquer une couleur différente des versions officielles
- Ajouter un ombre, un contour ou un effet quelconque
- Placer le logo sur un fond qui crée un contraste insuffisant
- Utiliser une version basse résolution ou reconstruite

### Formats

Tous les logos sont fournis en **SVG uniquement**.
Pour les exports PNG ou autres formats dérivés,
générer depuis les SVG sources — ne jamais retravailler un export comme source.

---

## 7. Iconography & Visual Elements

### Philosophie visuelle

L'identité visuelle d'Okuden s'inspire de l'esthétique fonctionnaliste :
formes géométriques pures, grilles rigoureuses, équilibre entre vide et plein.

L'ornement n'existe pas pour lui-même — chaque élément visuel a une fonction.
Les compositions privilégient la clarté architecturale :
alignements forts, marges généreuses, typographie qui respire.

Les formes sont réduites à leur essence — carrés, cercles, lignes droites.
Pas de dégradés complexes, pas d'ombres décoratives, pas d'illustrations illustratives.
La profondeur vient des contrastes de couleur et de taille, pas des effets.

### Iconographie

Okuden utilise des icônes linéaires, trait unique, à coin légèrement arrondi.
Aucune icône remplie sur fond coloré, sauf pour des états d'action actifs.

Source de référence : **Material Symbols** (Google Fonts) — style Outlined.

### Photographie

Les visuels photographiques montrent toujours des personnes réelles dans des contextes réels.
Pas de stock photo générique. Pas de mise en scène artificielle.
L'équipe, les clients, les lieux — authentiques et non retouchés au-delà du recadrage.

### Grille et espacement

Le système d'espacement repose sur une base de `4px` (voir `primitives.json`).
Les mises en page privilégient des marges larges — au minimum `48px` sur mobile,
`96px` sur desktop — pour préserver le sentiment d'espace et de maîtrise.

---

## 8. Voice & Tone

### Personnalité éditoriale

Okuden écrit comme ses consultants parlent :
avec expertise, sans posture, et avec un sens assumé de la réalité terrain.

Ni le jargon lisse du grand cabinet, ni l'enthousiasme startup.
Quelque chose entre les deux : rigoureux, direct, humain.
On sait de quoi on parle. On le dit clairement. Et on reste lucides.

---

### Traits de voix

| Trait                 | Ce que ça veut dire concrètement                                        |
|-----------------------|-------------------------------------------------------------------------|
| **Expert**            | On cite des cas réels, des noms, des chiffres. Pas de généralités.      |
| **Direct**            | On dit ce qu'on pense. Pas de langue de bois, pas de sur-nuancement.   |
| **Lucide**            | On célèbre sans se glorifier. On reconnaît les limites sans s'excuser.  |
| **Humain**            | L'équipe compte. On accueille les gens, on court sous la pluie ensemble.|
| **Légèrement décalé** | Une touche d'humour au bon moment — jamais forcé, jamais déplacé.      |

---

### Exemples de reformulations

| ❌ Éviter                                               | ✅ Préférer                                              |
|---------------------------------------------------------|----------------------------------------------------------|
| "Notre approche holistique garantit des résultats"      | "On rééquilibre les rapports de force. Concrètement."   |
| "Nous sommes ravis de partager cette belle nouvelle"    | "187ème au FT 1000. On reste lucides — mais quand même."|
| "Nos experts pluridisciplinaires vous accompagnent"     | "Une équipe de spécialistes, impliquée de A à Z."       |
| "Le passage à l'échelle est un enjeu stratégique"       | "Le proof of concept est passé de mode. Le temps presse."|
| "Notre solution révolutionnaire transforme votre CX"    | "Résultat : un projet CRM maîtrisé, délivré."           |

---

### Selon le support

| Support         | Ton                                                                       |
|-----------------|---------------------------------------------------------------------------|
| Blog / article  | Expert et terrain. Structuré, assertions tranchées, exemples clients nommés. |
| LinkedIn        | Direct, chaleureux sur les personnes, affirmé sur les convictions.        |
| Slides client   | Concis, orienté impact. Une slide = une idée forte.                       |
| Site web        | Affirmatif, orienté ambition, sans sur-vendre.                            |
| Onboarding RH   | Chaleureux, fidèle à "l'esprit Okuden" — l'humain avant le rôle.         |
| Emails          | Professionnel, personnalisé, toujours orienté vers une action concrète.   |

---

## 9. Assets

### Structure du repository

```
okuden-design/
├── DESIGN.md
├── Logo/
│   ├── Horizontal/
│   │   ├── logo_horizontal_blue.svg
│   │   └── logo_horizontal_white.svg
│   ├── Symbol/
│   │   ├── logo_symbol_blue.svg
│   │   └── logo_symbol_white.svg
│   └── Vertical/
│       ├── logo_vertical_blue.svg
│       └── logo_vertical_white.svg
└── Design tokens/
    ├── primitives.json
    └── semantics.json
```

---

### Tokens

| Fichier           | Contenu                                                              |
|-------------------|----------------------------------------------------------------------|
| `primitives.json` | Couleurs brutes, typographie, spacing, radius, shadows, border-width |
| `semantics.json`  | Tokens sémantiques — couleurs par rôle UI, typographie par usage,   |
|                   | radius et shadows nommés                                             |

> Toujours référencer les tokens sémantiques en production.
> Les primitives sont la source de vérité, pas des valeurs à consommer directement.

---

### Formats de logo

Tous les logos sont fournis en **SVG uniquement**.
Pour les exports PNG ou autres formats dérivés,
générer depuis les SVG sources — ne jamais retravailler un export comme source.

---

### Ressources externes

| Ressource        | Lien                                                     |
|------------------|----------------------------------------------------------|
| Material Symbols | [fonts.google.com/icons](https://fonts.google.com/icons) |
| Century Gothic   | Native Windows / macOS — inclus dans Microsoft Office    |

---

### Versionning

Ce fichier suit le versionning du repository.
Toute modification de guidelines doit être accompagnée
d'une mise à jour de `DESIGN.md` dans le même commit.

| Version | Description      |
|---------|------------------|
| 1.0     | Version initiale |
