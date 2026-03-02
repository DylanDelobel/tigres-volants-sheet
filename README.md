# tigres-volants-sheet

Fiche de personnage interactive pour le jeu de rôle **Tigres Volants**.
Aucune dépendance, aucun build — un seul fichier HTML à ouvrir dans le navigateur.

## Utilisation

```
Ouvrir index.html dans n'importe quel navigateur moderne.
```

La fiche se sauvegarde automatiquement dans le `localStorage` à chaque modification.

## Fonctionnalités

**Page Statistiques**
- 6 Aspects (ENG, PHY, RES, MEN, ADA, SPI) avec calcul du coût en points de création
- 9 Caractéristiques calculées automatiquement (FO, VO, IF, CO, PE, EQ, AG, IL, IT)
- Réflexes, Force vitale et Niveaux de fatigue (avec tooltip de règle)
- 5 Sens avec répartition libre (PE × 5 pts)
- Talents complets avec CA calculé, filtre de recherche et masquage des talents sans bonus

**Page Personnage**
- Identité, Description et Portrait (glisser-déposer ou clic)
- Avantages / Défauts, Niveau social
- Équipement de base (texte libre)
- Tableaux Armement et Protections à lignes dynamiques (5 initiales, +1 automatique dès que la dernière est remplie)

**Paramètres (bouton ⚙️)**
- Sauvegarde forcée, Export JSON, Import JSON, Réinitialisation
- Indicateur de sauvegarde automatique (point vert)

## Données

| Clé localStorage | Contenu |
|---|---|
| `tv_sheet` | Tous les champs de la fiche (JSON) |
| `tv_portrait` | Portrait encodé en base64 |

Le format d'export JSON inclut les deux clés et peut être réimporté tel quel.

## Structure

```
index.html   ← tout le projet (HTML + CSS + JS, ~1700 lignes)
```

Aucun framework, aucune dépendance externe.
Compatible avec tous les navigateurs modernes (Chrome, Firefox, Edge, Safari).
