/mue-agency/main/README.md = socle technique Principal générale
/mue-agency/projet/readmeproject.md = socle technique


## Socle Technique

> **NB :** Les critères sont définis indépendamment de la solution.

### Critères de sélection pour la stack technique de la MVP

- Aucun temps d'apprentissage n'est requis pour l'équipe.
- Capacité de déploiement d'une démonstration rapide.
- Contrainte budgétaire nulle (coût d'infrastructure initial de zéro).

---

### Comparatif des stacks ? notation /5

| Critères                   | Next.js | Vue.js / Node.js | React / Node.js | NoCode |
|----------------------------|:-------:|:----------------:|:---------------:|:------:|
| Maîtrise                   |    5    |        3         |        4        |   3    |
| Rapidité de développement  |    4    |        3         |        4        |   3    |
| Facilité de déploiement    |    5    |        3         |        4        |   4    |
| Flexibilité                |    5    |        4         |        4        |   3    |
| **Score total**            |  **19** |      **13**      |     **16**      | **13** |

---

### Solution retenue : Next.js

Ce choix est justifié par une maîtrise totale de la technologie par l'équipe, un déploiement simplifié via Vercel et une parfaite adéquation pour la création de web apps, de tableaux de bord et de pages d'atterrissage.

> **Note :** La stack technique pourra faire l'objet d'ajustements ultérieurs en fonction de l'évolution des besoins fonctionnels et de la nature de la solution finale.

---

## Structure de développement

### Organisation du repo

```
/src
frontend/        
backend/
.env
README.md
```

---

## Liens utiles

- **GitHub :** [https://github.com/StoneUi/mue-agency.git](https://github.com/StoneUi/mue-agency.git)

### Branches

| Branche   | Usage                    |
|-----------|--------------------------|
| `main`    | Production               |
| `agence`  | Site de l'agence         |
| `projet`  | Pour le projet lui-même  |
| `Elea`    | Branche de travail       |
| `Giovani` | Branche de travail       |
