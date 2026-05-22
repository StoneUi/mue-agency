Socle tech projet


Notre solution n'est pas décidé, 
Les critères sont définis indépendamment de la solution

Environnement idéale

- Next.js
- Tailwind
- PostgreSQL via Docker
- Vercel

Critères de sélection pour la stack technique de la MVP

Aucun temps d'apprentissage n'est requis pour l'équipe.
Capacité de déploiement d'une démonstration rapide.
Contrainte budgétaire nulle (coût d'infrastructure initial de zéro).


Pour un développement rapide,  les stacks : listés et notation /5


| Critères                   | Next.js | Vue.js / Node.js | React / Node.js | NoCode |
|----------------------------|:-------:|:----------------:|:---------------:|:------:|
| Maîtrise                   |    5    |        3         |        4        |   3    |
| Rapidité de développement  |    4    |        3         |        4        |   3    |
| Facilité de déploiement    |    5    |        3         |        4        |   4    |
| Flexibilité                |    5    |        4         |        4        |   3    |
| **Score total**            |  **19** |      **13**      |     **16**      | **13** |

Solution retenue : Next.js. Ce choix est justifié par une maîtrise totale de la technologie par l'équipe, un déploiement simplifié via Vercel et une parfaite adéquation pour la création de web apps, de tableaux de bord et de pages d'atterrissage.

Note : La stack technique pourra faire l'objet d'ajustements ultérieurs en fonction de l'évolution des besoins fonctionnels et de la nature de la solution finale.


A envisager 

  Puissance relationnelle et géographique :   L'utilisation de PostgreSQL en arrière-plan permet d'activer facilement l'extension   PostGIS   pour les requêtes de géolocalisation (calcul de distance entre profils), une fonctionnalité indispensable pour une application de rencontres.

  Chatbot  
  Commande vocale  
     

Structure de développement
 Organisation du repo

  /src
  ├── frontend/
  ├── backend/api                                                                                                                                              
  ├── .env   
  └── README.md


Lien Utils : 

Github https://github.com/StoneUi/mue-agency.git

Branch :

main → 
agence→ site de l’agence
projet → Pour le projet lui même
Elea → branch de travail
Giovani → branch de travail
