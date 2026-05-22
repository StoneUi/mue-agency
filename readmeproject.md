## Socle tech projet

Notre solution n'est pas décidé, 
L'environnement idéale pour un MVP, 
Pour aller vite et selon nos connaissances

## Environnement idéale
- React
- Tailwind
- Supabase
- Vercel


```
npm create vite@latest . -- --template react
npm install
```
```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```
```
npm install @supabase/supabase-js
```
```
npm install -g vercel
vercel login
vercel
```


## La Stack Technique
### Frontend & Interface
*   **React :** Moteur visuel configuré en *Single Page Application* (SPA). 
La logique de navigation et d'affichage est exécutée directement côté client, offrant des performances fluides et une réactivité de type "application native"
*   **Tailwind CSS :** Framework utilitaire permettant un prototypage d'interface ultra-rapide. 
Le moteur de *build* purge automatiquement le CSS inutilisé, garantissant un fichier final extrêmement léger et un temps de chargement minimal.

### Backend & Données (Serverless Architecture)
*   **Supabase :** Solution *Backend-as-a-Service* qui élimine le besoin de concevoir et de maintenir une API dédiée (type Express/Node.js). Le SDK client est intégré directement dans React.

    *   **Base de données :** PostgreSQL natif, idéal pour gérer les relations complexes (Profils, Likes, Matchs).
    *   **Sécurité :** Sécurisation des données au niveau de la base via les **Row Level Security (RLS)** de PostgreSQL.
    *   **Stockage :** Gestion native des images de profil via les *Buckets de Stockage* intégrés.

### Hébergement & Infrastructure
*   **Vercel :** Déploiement continu et hébergement des fichiers statiques (HTML/JS/CSS) sur un réseau mondial de serveurs (CDN). Garantit un *Time to First Byte* (TTFB) quasi instantané et une disponibilité maximale.

---

## Étude Comparative : Pourquoi cette architecture ?

Pour ce MVP, l'architecture **React + Supabase** a été préférée aux approches traditionnelles ou hybrides pour des raisons d'agilité et d'efficacité technique :

Critères techniques 
La Stack *(React + Supabase)*
Stack Traditionnelle *(React + Express + Render)* 
Stack Hybride *(Next.js + Prisma)* 

**Complexité de code** 
**Basse** (1 seul projet Frontend à maintenir) | **Haute** (2 projets distincts : Front + API Back) | **Moyenne** (1 projet unifié mais concepts SSR complexes)

**Gestion Serveur**
**Zéro** (Entièrement managé) | **Manuelle** (Monitoring et maintenance du serveur) | **Zéro** (Entièrement managé)

**Infrastructure / Coût** 
**0 € (MVP)** (Offres gratuites très larges) | **Payant rapidement** (Mise en veille des serveurs gratuits) | **0 € (MVP)** (Limites de calcul strictes) 

**Vitesse de mise en production** 
**Ultra-Rapide** | **Moyenne** (Plomberie API à coder) | **Rapide** 

### Les Avantages Clés

**Réduction de la surface de code de 30% à 40% :** 
En éliminant la couche d'API intermédiaire (Express), la vitesse d'itération est maximale. La logique métier (recherche de profils, création de matchs) s'appuie directement sur la puissance du SDK Supabase.





### A envisager 

**Puissance relationnelle et géographique :** L'utilisation de PostgreSQL en arrière-plan permet d'activer facilement l'extension **PostGIS** pour les requêtes de géolocalisation (calcul de distance entre profils), une fonctionnalité indispensable pour une application de rencontres.

**Chatbot**
**Commande vocale**
** **